# Comparing `tmp/buildbot-www-3.8.0.tar.gz` & `tmp/buildbot-www-v0.9.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buildbot-www-3.8.0.tar", last modified: Mon Apr 17 01:20:32 2023, max compression
+gzip compressed data, was "dist/buildbot-www-v0.9.0b9.tar", last modified: Wed May 11 19:15:34 2016, max compression
```

## Comparing `buildbot-www-3.8.0.tar` & `buildbot-www-v0.9.0b9.tar`

### file list

```diff
@@ -1,41 +1,29 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      238 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      847 2023-04-17 01:17:21.000000 buildbot-www-3.8.0/buildbot_www/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   151076 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/2.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   618634 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/2.js.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18028 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/448c34a56d699c29117adc64c43affeb.woff2
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   165742 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/674f50d287a8c48dc19ba404d20fe713.eot
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    77160 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/af7ae505a9eed503f8b8e6982036873e.woff2
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   165548 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/b06871f281fee6b241d60582ae9369b9.ttf
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      782 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/browser-warning-list.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1472 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/browser-warning.css
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    26146 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/browser-warning.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    45404 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/e18bbf611f2a2e43afc071aa2f4e1512.ttf
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    20127 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/f4769f9bdb7466be65088239c12046d1.eot
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    23424 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/fa2772327f55d8198301fdb8bcfc8158.woff
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    98024 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/fee66e712a8a08eef5805a46892932ad.woff
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/img/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1150 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/img/favicon.ico
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   444379 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/img/fontawesome-webfont.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   108738 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/img/glyphicons-halflings-regular.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21460 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/img/icon.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1180 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/img/icon.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      483 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/img/icon16.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2241 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/img/nobody.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1385 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/index.html
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)  1528947 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/scripts.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)  7856273 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/scripts.js.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   203502 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/styles.css
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   267673 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www/static/styles.css.map
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      238 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1361 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        9 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www.egg-info/requires.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       13 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/buildbot_www.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-04-17 01:20:32.000000 buildbot-www-3.8.0/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1623 2023-04-17 01:17:21.000000 buildbot-www-3.8.0/setup.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       59 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/setup.cfg
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        8 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www/VERSION
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      847 2015-10-24 18:56:13.000000 buildbot-www-v0.9.0b9/buildbot_www/__init__.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www/static/
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www/static/img/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2241 2016-05-11 19:15:18.000000 buildbot-www-v0.9.0b9/buildbot_www/static/img/nobody.png
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1150 2016-05-11 19:15:18.000000 buildbot-www-v0.9.0b9/buildbot_www/static/img/favicon.ico
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)   620986 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www/static/scripts.js
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)   148305 2016-05-11 19:15:20.000000 buildbot-www-v0.9.0b9/buildbot_www/static/tests.js
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1032 2016-05-11 19:15:18.000000 buildbot-www-v0.9.0b9/buildbot_www/static/index.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)   146528 2016-05-11 19:15:18.000000 buildbot-www-v0.9.0b9/buildbot_www/static/d3.min.js
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www/static/fonts/
+-rwxrwxr-x   0 pierre    (1000) pierre    (1000)   141564 2016-05-11 19:15:19.000000 buildbot-www-v0.9.0b9/buildbot_www/static/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    75188 2016-05-11 19:15:18.000000 buildbot-www-v0.9.0b9/buildbot_www/static/fonts/FontAwesome.otf
+-rwxrwxr-x   0 pierre    (1000) pierre    (1000)   253487 2016-05-11 19:15:18.000000 buildbot-www-v0.9.0b9/buildbot_www/static/fonts/fontawesome-webfont.svg
+-rwxrwxr-x   0 pierre    (1000) pierre    (1000)    83760 2016-05-11 19:15:20.000000 buildbot-www-v0.9.0b9/buildbot_www/static/fonts/fontawesome-webfont.woff
+-rwxrwxr-x   0 pierre    (1000) pierre    (1000)    72449 2016-05-11 19:15:18.000000 buildbot-www-v0.9.0b9/buildbot_www/static/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)   130852 2016-05-11 19:15:19.000000 buildbot-www-v0.9.0b9/buildbot_www/static/styles.css
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1577 2016-01-20 20:30:40.000000 buildbot-www-v0.9.0b9/setup.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      220 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/PKG-INFO
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www.egg-info/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       59 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www.egg-info/entry_points.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       13 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www.egg-info/top_level.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       47 2016-04-08 17:23:04.000000 buildbot-www-v0.9.0b9/buildbot_www.egg-info/pbr.json
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      734 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      220 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2016-05-11 19:15:34.000000 buildbot-www-v0.9.0b9/buildbot_www.egg-info/dependency_links.txt
```

### Comparing `buildbot-www-3.8.0/buildbot_www/__init__.py` & `buildbot-www-v0.9.0b9/buildbot_www/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-www-3.8.0/buildbot_www/static/2.js` & `buildbot-www-v0.9.0b9/buildbot_www/static/d3.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7776 +1,7596 @@
-(("undefined" != typeof self ? self : this).webpackJsonpbuildbot_www = ("undefined" != typeof self ? self : this).webpackJsonpbuildbot_www || []).push([
-    [2], {
-        289: function(n, t, e) {
-            var r, i;
-            ! function() {
-                var u = {
-                        version: "3.5.17"
-                    },
-                    o = [].slice,
-                    a = function(n) {
-                        return o.call(n)
-                    },
-                    l = this.document;
-
-                function c(n) {
-                    return n && (n.ownerDocument || n.document || n).documentElement
-                }
-
-                function f(n) {
-                    return n && (n.ownerDocument && n.ownerDocument.defaultView || n.document && n || n.defaultView)
-                }
-                if (l) try {
-                    a(l.documentElement.childNodes)[0].nodeType
-                } catch (n) {
-                    a = function(n) {
-                        for (var t = n.length, e = new Array(t); t--;) e[t] = n[t];
-                        return e
-                    }
-                }
-                if (Date.now || (Date.now = function() {
-                        return +new Date
-                    }), l) try {
-                    l.createElement("DIV").style.setProperty("opacity", 0, "")
-                } catch (n) {
-                    var s = this.Element.prototype,
-                        h = s.setAttribute,
-                        p = s.setAttributeNS,
-                        g = this.CSSStyleDeclaration.prototype,
-                        v = g.setProperty;
-                    s.setAttribute = function(n, t) {
-                        h.call(this, n, t + "")
-                    }, s.setAttributeNS = function(n, t, e) {
-                        p.call(this, n, t, e + "")
-                    }, g.setProperty = function(n, t, e) {
-                        v.call(this, n, t + "", e)
-                    }
-                }
+! function() {
+    function n(n, t) {
+        return t > n ? -1 : n > t ? 1 : n >= t ? 0 : 0 / 0
+    }
 
-                function d(n, t) {
-                    return n < t ? -1 : n > t ? 1 : n >= t ? 0 : NaN
-                }
+    function t(n) {
+        return null === n ? 0 / 0 : +n
+    }
 
-                function y(n) {
-                    return null === n ? NaN : +n
-                }
+    function e(n) {
+        return !isNaN(n)
+    }
 
-                function m(n) {
-                    return !isNaN(n)
+    function r(n) {
+        return {
+            left: function(t, e, r, u) {
+                for (arguments.length < 3 && (r = 0), arguments.length < 4 && (u = t.length); u > r;) {
+                    var i = r + u >>> 1;
+                    n(t[i], e) < 0 ? r = i + 1 : u = i
+                }
+                return r
+            },
+            right: function(t, e, r, u) {
+                for (arguments.length < 3 && (r = 0), arguments.length < 4 && (u = t.length); u > r;) {
+                    var i = r + u >>> 1;
+                    n(t[i], e) > 0 ? u = i : r = i + 1
                 }
+                return r
+            }
+        }
+    }
 
-                function M(n) {
-                    return {
-                        left: function(t, e, r, i) {
-                            for (arguments.length < 3 && (r = 0), arguments.length < 4 && (i = t.length); r < i;) {
-                                var u = r + i >>> 1;
-                                n(t[u], e) < 0 ? r = u + 1 : i = u
-                            }
-                            return r
-                        },
-                        right: function(t, e, r, i) {
-                            for (arguments.length < 3 && (r = 0), arguments.length < 4 && (i = t.length); r < i;) {
-                                var u = r + i >>> 1;
-                                n(t[u], e) > 0 ? i = u : r = u + 1
-                            }
-                            return r
-                        }
-                    }
-                }
-                u.ascending = d, u.descending = function(n, t) {
-                    return t < n ? -1 : t > n ? 1 : t >= n ? 0 : NaN
-                }, u.min = function(n, t) {
-                    var e, r, i = -1,
-                        u = n.length;
-                    if (1 === arguments.length) {
-                        for (; ++i < u;)
-                            if (null != (r = n[i]) && r >= r) {
-                                e = r;
-                                break
-                            } for (; ++i < u;) null != (r = n[i]) && e > r && (e = r)
-                    } else {
-                        for (; ++i < u;)
-                            if (null != (r = t.call(n, n[i], i)) && r >= r) {
-                                e = r;
-                                break
-                            } for (; ++i < u;) null != (r = t.call(n, n[i], i)) && e > r && (e = r)
-                    }
-                    return e
-                }, u.max = function(n, t) {
-                    var e, r, i = -1,
-                        u = n.length;
-                    if (1 === arguments.length) {
-                        for (; ++i < u;)
-                            if (null != (r = n[i]) && r >= r) {
-                                e = r;
-                                break
-                            } for (; ++i < u;) null != (r = n[i]) && r > e && (e = r)
-                    } else {
-                        for (; ++i < u;)
-                            if (null != (r = t.call(n, n[i], i)) && r >= r) {
-                                e = r;
-                                break
-                            } for (; ++i < u;) null != (r = t.call(n, n[i], i)) && r > e && (e = r)
-                    }
-                    return e
-                }, u.extent = function(n, t) {
-                    var e, r, i, u = -1,
-                        o = n.length;
-                    if (1 === arguments.length) {
-                        for (; ++u < o;)
-                            if (null != (r = n[u]) && r >= r) {
-                                e = i = r;
-                                break
-                            } for (; ++u < o;) null != (r = n[u]) && (e > r && (e = r), i < r && (i = r))
-                    } else {
-                        for (; ++u < o;)
-                            if (null != (r = t.call(n, n[u], u)) && r >= r) {
-                                e = i = r;
-                                break
-                            } for (; ++u < o;) null != (r = t.call(n, n[u], u)) && (e > r && (e = r), i < r && (i = r))
-                    }
-                    return [e, i]
-                }, u.sum = function(n, t) {
-                    var e, r = 0,
-                        i = n.length,
-                        u = -1;
-                    if (1 === arguments.length)
-                        for (; ++u < i;) m(e = +n[u]) && (r += e);
-                    else
-                        for (; ++u < i;) m(e = +t.call(n, n[u], u)) && (r += e);
-                    return r
-                }, u.mean = function(n, t) {
-                    var e, r = 0,
-                        i = n.length,
-                        u = -1,
-                        o = i;
-                    if (1 === arguments.length)
-                        for (; ++u < i;) m(e = y(n[u])) ? r += e : --o;
-                    else
-                        for (; ++u < i;) m(e = y(t.call(n, n[u], u))) ? r += e : --o;
-                    if (o) return r / o
-                }, u.quantile = function(n, t) {
-                    var e = (n.length - 1) * t + 1,
-                        r = Math.floor(e),
-                        i = +n[r - 1],
-                        u = e - r;
-                    return u ? i + u * (n[r] - i) : i
-                }, u.median = function(n, t) {
-                    var e, r = [],
-                        i = n.length,
-                        o = -1;
-                    if (1 === arguments.length)
-                        for (; ++o < i;) m(e = y(n[o])) && r.push(e);
-                    else
-                        for (; ++o < i;) m(e = y(t.call(n, n[o], o))) && r.push(e);
-                    if (r.length) return u.quantile(r.sort(d), .5)
-                }, u.variance = function(n, t) {
-                    var e, r, i = n.length,
-                        u = 0,
-                        o = 0,
-                        a = -1,
-                        l = 0;
-                    if (1 === arguments.length)
-                        for (; ++a < i;) m(e = y(n[a])) && (o += (r = e - u) * (e - (u += r / ++l)));
-                    else
-                        for (; ++a < i;) m(e = y(t.call(n, n[a], a))) && (o += (r = e - u) * (e - (u += r / ++l)));
-                    if (l > 1) return o / (l - 1)
-                }, u.deviation = function() {
-                    var n = u.variance.apply(this, arguments);
-                    return n ? Math.sqrt(n) : n
-                };
-                var x = M(d);
+    function u(n) {
+        return n.length
+    }
 
-                function b(n) {
-                    return n.length
-                }
-                u.bisectLeft = x.left, u.bisect = u.bisectRight = x.right, u.bisector = function(n) {
-                    return M(1 === n.length ? function(t, e) {
-                        return d(n(t), e)
-                    } : n)
-                }, u.shuffle = function(n, t, e) {
-                    (u = arguments.length) < 3 && (e = n.length, u < 2 && (t = 0));
-                    for (var r, i, u = e - t; u;) i = Math.random() * u-- | 0, r = n[u + t], n[u + t] = n[i + t], n[i + t] = r;
-                    return n
-                }, u.permute = function(n, t) {
-                    for (var e = t.length, r = new Array(e); e--;) r[e] = n[t[e]];
-                    return r
-                }, u.pairs = function(n) {
-                    for (var t = 0, e = n.length - 1, r = n[0], i = new Array(e < 0 ? 0 : e); t < e;) i[t] = [r, r = n[++t]];
-                    return i
-                }, u.transpose = function(n) {
-                    if (!(i = n.length)) return [];
-                    for (var t = -1, e = u.min(n, b), r = new Array(e); ++t < e;)
-                        for (var i, o = -1, a = r[t] = new Array(i); ++o < i;) a[o] = n[o][t];
-                    return r
-                }, u.zip = function() {
-                    return u.transpose(arguments)
-                }, u.keys = function(n) {
-                    var t = [];
-                    for (var e in n) t.push(e);
-                    return t
-                }, u.values = function(n) {
-                    var t = [];
-                    for (var e in n) t.push(n[e]);
-                    return t
-                }, u.entries = function(n) {
-                    var t = [];
-                    for (var e in n) t.push({
-                        key: e,
-                        value: n[e]
-                    });
-                    return t
-                }, u.merge = function(n) {
-                    for (var t, e, r, i = n.length, u = -1, o = 0; ++u < i;) o += n[u].length;
-                    for (e = new Array(o); --i >= 0;)
-                        for (t = (r = n[i]).length; --t >= 0;) e[--o] = r[t];
-                    return e
-                };
-                var w = Math.abs;
+    function i(n) {
+        for (var t = 1; n * t % 1;) t *= 10;
+        return t
+    }
 
-                function _(n) {
-                    for (var t = 1; n * t % 1;) t *= 10;
-                    return t
-                }
+    function o(n, t) {
+        for (var e in t) Object.defineProperty(n.prototype, e, {
+            value: t[e],
+            enumerable: !1
+        })
+    }
 
-                function k(n, t) {
-                    for (var e in t) Object.defineProperty(n.prototype, e, {
-                        value: t[e],
-                        enumerable: !1
-                    })
-                }
+    function a() {
+        this._ = Object.create(null)
+    }
 
-                function S() {
-                    this._ = Object.create(null)
-                }
-                u.range = function(n, t, e) {
-                    if (arguments.length < 3 && (e = 1, arguments.length < 2 && (t = n, n = 0)), (t - n) / e == 1 / 0) throw new Error("infinite range");
-                    var r, i = [],
-                        u = _(w(e)),
-                        o = -1;
-                    if (n *= u, t *= u, (e *= u) < 0)
-                        for (;
-                            (r = n + e * ++o) > t;) i.push(r / u);
-                    else
-                        for (;
-                            (r = n + e * ++o) < t;) i.push(r / u);
-                    return i
-                }, u.map = function(n, t) {
-                    var e = new S;
-                    if (n instanceof S) n.forEach((function(n, t) {
-                        e.set(n, t)
-                    }));
-                    else if (Array.isArray(n)) {
-                        var r, i = -1,
-                            u = n.length;
-                        if (1 === arguments.length)
-                            for (; ++i < u;) e.set(i, n[i]);
-                        else
-                            for (; ++i < u;) e.set(t.call(n, r = n[i], i), r)
-                    } else
-                        for (var o in n) e.set(o, n[o]);
-                    return e
-                };
+    function c(n) {
+        return (n += "") === la || n[0] === sa ? sa + n : n
+    }
 
-                function N(n) {
-                    return "__proto__" == (n += "") || "\0" === n[0] ? "\0" + n : n
-                }
+    function l(n) {
+        return (n += "")[0] === sa ? n.slice(1) : n
+    }
 
-                function E(n) {
-                    return "\0" === (n += "")[0] ? n.slice(1) : n
-                }
+    function s(n) {
+        return c(n) in this._
+    }
 
-                function A(n) {
-                    return N(n) in this._
-                }
+    function f(n) {
+        return (n = c(n)) in this._ && delete this._[n]
+    }
 
-                function C(n) {
-                    return (n = N(n)) in this._ && delete this._[n]
-                }
+    function h() {
+        var n = [];
+        for (var t in this._) n.push(l(t));
+        return n
+    }
 
-                function z() {
-                    var n = [];
-                    for (var t in this._) n.push(E(t));
-                    return n
-                }
+    function g() {
+        var n = 0;
+        for (var t in this._) ++n;
+        return n
+    }
 
-                function L() {
-                    var n = 0;
-                    for (var t in this._) ++n;
-                    return n
-                }
+    function p() {
+        for (var n in this._) return !1;
+        return !0
+    }
 
-                function q() {
-                    for (var n in this._) return !1;
-                    return !0
-                }
+    function v() {
+        this._ = Object.create(null)
+    }
 
-                function T() {
-                    this._ = Object.create(null)
-                }
+    function d(n, t, e) {
+        return function() {
+            var r = e.apply(t, arguments);
+            return r === t ? n : r
+        }
+    }
 
-                function R(n) {
-                    return n
-                }
+    function m(n, t) {
+        if (t in n) return t;
+        t = t.charAt(0).toUpperCase() + t.slice(1);
+        for (var e = 0, r = fa.length; r > e; ++e) {
+            var u = fa[e] + t;
+            if (u in n) return u
+        }
+    }
 
-                function D(n, t, e) {
-                    return function() {
-                        var r = e.apply(t, arguments);
-                        return r === t ? n : r
-                    }
-                }
+    function y() {}
 
-                function P(n, t) {
-                    if (t in n) return t;
-                    t = t.charAt(0).toUpperCase() + t.slice(1);
-                    for (var e = 0, r = U.length; e < r; ++e) {
-                        var i = U[e] + t;
-                        if (i in n) return i
-                    }
-                }
-                k(S, {
-                    has: A,
-                    get: function(n) {
-                        return this._[N(n)]
-                    },
-                    set: function(n, t) {
-                        return this._[N(n)] = t
-                    },
-                    remove: C,
-                    keys: z,
-                    values: function() {
-                        var n = [];
-                        for (var t in this._) n.push(this._[t]);
-                        return n
-                    },
-                    entries: function() {
-                        var n = [];
-                        for (var t in this._) n.push({
-                            key: E(t),
-                            value: this._[t]
-                        });
-                        return n
-                    },
-                    size: L,
-                    empty: q,
-                    forEach: function(n) {
-                        for (var t in this._) n.call(this, E(t), this._[t])
-                    }
-                }), u.nest = function() {
-                    var n, t, e = {},
-                        r = [],
-                        i = [];
-
-                    function o(i, u, a) {
-                        if (a >= r.length) return t ? t.call(e, u) : n ? u.sort(n) : u;
-                        for (var l, c, f, s, h = -1, p = u.length, g = r[a++], v = new S; ++h < p;)(s = v.get(l = g(c = u[h]))) ? s.push(c) : v.set(l, [c]);
-                        return i ? (c = i(), f = function(n, t) {
-                            c.set(n, o(i, t, a))
-                        }) : (c = {}, f = function(n, t) {
-                            c[n] = o(i, t, a)
-                        }), v.forEach(f), c
-                    }
-                    return e.map = function(n, t) {
-                        return o(t, n, 0)
-                    }, e.entries = function(n) {
-                        return function n(t, e) {
-                            if (e >= r.length) return t;
-                            var u = [],
-                                o = i[e++];
-                            return t.forEach((function(t, r) {
-                                u.push({
-                                    key: t,
-                                    values: n(r, e)
-                                })
-                            })), o ? u.sort((function(n, t) {
-                                return o(n.key, t.key)
-                            })) : u
-                        }(o(u.map, n, 0), 0)
-                    }, e.key = function(n) {
-                        return r.push(n), e
-                    }, e.sortKeys = function(n) {
-                        return i[r.length - 1] = n, e
-                    }, e.sortValues = function(t) {
-                        return n = t, e
-                    }, e.rollup = function(n) {
-                        return t = n, e
-                    }, e
-                }, u.set = function(n) {
-                    var t = new T;
-                    if (n)
-                        for (var e = 0, r = n.length; e < r; ++e) t.add(n[e]);
-                    return t
-                }, k(T, {
-                    has: A,
-                    add: function(n) {
-                        return this._[N(n += "")] = !0, n
-                    },
-                    remove: C,
-                    values: z,
-                    size: L,
-                    empty: q,
-                    forEach: function(n) {
-                        for (var t in this._) n.call(this, E(t))
-                    }
-                }), u.behavior = {}, u.rebind = function(n, t) {
-                    for (var e, r = 1, i = arguments.length; ++r < i;) n[e = arguments[r]] = D(n, t, t[e]);
-                    return n
-                };
-                var U = ["webkit", "ms", "moz", "Moz", "o", "O"];
+    function x() {}
 
-                function j() {}
+    function M(n) {
+        function t() {
+            for (var t, r = e, u = -1, i = r.length; ++u < i;)(t = r[u].on) && t.apply(this, arguments);
+            return n
+        }
+        var e = [],
+            r = new a;
+        return t.on = function(t, u) {
+            var i, o = r.get(t);
+            return arguments.length < 2 ? o && o.on : (o && (o.on = null, e = e.slice(0, i = e.indexOf(o)).concat(e.slice(i + 1)), r.remove(t)), u && e.push(r.set(t, {
+                on: u
+            })), n)
+        }, t
+    }
 
-                function F() {}
+    function _() {
+        Bo.event.preventDefault()
+    }
 
-                function H(n) {
-                    var t = [],
-                        e = new S;
+    function b() {
+        for (var n, t = Bo.event; n = t.sourceEvent;) t = n;
+        return t
+    }
 
-                    function r() {
-                        for (var e, r = t, i = -1, u = r.length; ++i < u;)(e = r[i].on) && e.apply(this, arguments);
-                        return n
-                    }
-                    return r.on = function(r, i) {
-                        var u, o = e.get(r);
-                        return arguments.length < 2 ? o && o.on : (o && (o.on = null, t = t.slice(0, u = t.indexOf(o)).concat(t.slice(u + 1)), e.remove(r)), i && t.push(e.set(r, {
-                            on: i
-                        })), n)
-                    }, r
+    function w(n) {
+        for (var t = new x, e = 0, r = arguments.length; ++e < r;) t[arguments[e]] = M(t);
+        return t.of = function(e, r) {
+            return function(u) {
+                try {
+                    var i = u.sourceEvent = Bo.event;
+                    u.target = n, Bo.event = u, t[u.type].apply(e, r)
+                } finally {
+                    Bo.event = i
                 }
+            }
+        }, t
+    }
 
-                function O() {
-                    u.event.preventDefault()
-                }
+    function S(n) {
+        return ga(n, ya), n
+    }
 
-                function I() {
-                    for (var n, t = u.event; n = t.sourceEvent;) t = n;
-                    return t
-                }
+    function k(n) {
+        return "function" == typeof n ? n : function() {
+            return pa(n, this)
+        }
+    }
 
-                function Y(n) {
-                    for (var t = new F, e = 0, r = arguments.length; ++e < r;) t[arguments[e]] = H(t);
-                    return t.of = function(e, r) {
-                        return function(i) {
-                            try {
-                                var o = i.sourceEvent = u.event;
-                                i.target = n, u.event = i, t[i.type].apply(e, r)
-                            } finally {
-                                u.event = o
-                            }
-                        }
-                    }, t
-                }
-                u.dispatch = function() {
-                    for (var n = new F, t = -1, e = arguments.length; ++t < e;) n[arguments[t]] = H(n);
-                    return n
-                }, F.prototype.on = function(n, t) {
-                    var e = n.indexOf("."),
-                        r = "";
-                    if (e >= 0 && (r = n.slice(e + 1), n = n.slice(0, e)), n) return arguments.length < 2 ? this[n].on(r) : this[n].on(r, t);
-                    if (2 === arguments.length) {
-                        if (null == t)
-                            for (n in this) this.hasOwnProperty(n) && this[n].on(r, null);
-                        return this
-                    }
-                }, u.event = null, u.requote = function(n) {
-                    return n.replace(Z, "\\$&")
-                };
-                var Z = /[\\\^\$\*\+\?\|\[\]\(\)\.\{\}]/g,
-                    V = {}.__proto__ ? function(n, t) {
-                        n.__proto__ = t
-                    } : function(n, t) {
-                        for (var e in t) n[e] = t[e]
-                    };
+    function E(n) {
+        return "function" == typeof n ? n : function() {
+            return va(n, this)
+        }
+    }
 
-                function X(n) {
-                    return V(n, W), n
-                }
-                var $ = function(n, t) {
-                        return t.querySelector(n)
-                    },
-                    B = function(n, t) {
-                        return t.querySelectorAll(n)
-                    },
-                    J = function(n, t) {
-                        var e = n.matches || n[P(n, "matchesSelector")];
-                        return (J = function(n, t) {
-                            return e.call(n, t)
-                        })(n, t)
-                    };
-                "function" == typeof Sizzle && ($ = function(n, t) {
-                    return Sizzle(n, t)[0] || null
-                }, B = Sizzle, J = Sizzle.matchesSelector), u.selection = function() {
-                    return u.select(l.documentElement)
-                };
-                var W = u.selection.prototype = [];
+    function A(n, t) {
+        function e() {
+            this.removeAttribute(n)
+        }
 
-                function G(n) {
-                    return "function" == typeof n ? n : function() {
-                        return $(n, this)
-                    }
-                }
+        function r() {
+            this.removeAttributeNS(n.space, n.local)
+        }
 
-                function K(n) {
-                    return "function" == typeof n ? n : function() {
-                        return B(n, this)
-                    }
-                }
-                W.select = function(n) {
-                    var t, e, r, i, u = [];
-                    n = G(n);
-                    for (var o = -1, a = this.length; ++o < a;) {
-                        u.push(t = []), t.parentNode = (r = this[o]).parentNode;
-                        for (var l = -1, c = r.length; ++l < c;)(i = r[l]) ? (t.push(e = n.call(i, i.__data__, l, o)), e && "__data__" in i && (e.__data__ = i.__data__)) : t.push(null)
-                    }
-                    return X(u)
-                }, W.selectAll = function(n) {
-                    var t, e, r = [];
-                    n = K(n);
-                    for (var i = -1, u = this.length; ++i < u;)
-                        for (var o = this[i], l = -1, c = o.length; ++l < c;)(e = o[l]) && (r.push(t = a(n.call(e, e.__data__, l, i))), t.parentNode = e);
-                    return X(r)
-                };
-                var Q = "http://www.w3.org/1999/xhtml",
-                    nn = {
-                        svg: "http://www.w3.org/2000/svg",
-                        xhtml: Q,
-                        xlink: "http://www.w3.org/1999/xlink",
-                        xml: "http://www.w3.org/XML/1998/namespace",
-                        xmlns: "http://www.w3.org/2000/xmlns/"
-                    };
+        function u() {
+            this.setAttribute(n, t)
+        }
 
-                function tn(n, t) {
-                    return n = u.ns.qualify(n), null == t ? n.local ? function() {
-                        this.removeAttributeNS(n.space, n.local)
-                    } : function() {
-                        this.removeAttribute(n)
-                    } : "function" == typeof t ? n.local ? function() {
-                        var e = t.apply(this, arguments);
-                        null == e ? this.removeAttributeNS(n.space, n.local) : this.setAttributeNS(n.space, n.local, e)
-                    } : function() {
-                        var e = t.apply(this, arguments);
-                        null == e ? this.removeAttribute(n) : this.setAttribute(n, e)
-                    } : n.local ? function() {
-                        this.setAttributeNS(n.space, n.local, t)
-                    } : function() {
-                        this.setAttribute(n, t)
-                    }
-                }
+        function i() {
+            this.setAttributeNS(n.space, n.local, t)
+        }
 
-                function en(n) {
-                    return n.trim().replace(/\s+/g, " ")
-                }
+        function o() {
+            var e = t.apply(this, arguments);
+            null == e ? this.removeAttribute(n) : this.setAttribute(n, e)
+        }
 
-                function rn(n) {
-                    return new RegExp("(?:^|\\s+)" + u.requote(n) + "(?:\\s+|$)", "g")
-                }
+        function a() {
+            var e = t.apply(this, arguments);
+            null == e ? this.removeAttributeNS(n.space, n.local) : this.setAttributeNS(n.space, n.local, e)
+        }
+        return n = Bo.ns.qualify(n), null == t ? n.local ? r : e : "function" == typeof t ? n.local ? a : o : n.local ? i : u
+    }
 
-                function un(n) {
-                    return (n + "").trim().split(/^|\s+/)
-                }
+    function C(n) {
+        return n.trim().replace(/\s+/g, " ")
+    }
 
-                function on(n, t) {
-                    var e = (n = un(n).map(an)).length;
-                    return "function" == typeof t ? function() {
-                        for (var r = -1, i = t.apply(this, arguments); ++r < e;) n[r](this, i)
-                    } : function() {
-                        for (var r = -1; ++r < e;) n[r](this, t)
-                    }
-                }
+    function N(n) {
+        return new RegExp("(?:^|\\s+)" + Bo.requote(n) + "(?:\\s+|$)", "g")
+    }
 
-                function an(n) {
-                    var t = rn(n);
-                    return function(e, r) {
-                        if (i = e.classList) return r ? i.add(n) : i.remove(n);
-                        var i = e.getAttribute("class") || "";
-                        r ? (t.lastIndex = 0, t.test(i) || e.setAttribute("class", en(i + " " + n))) : e.setAttribute("class", en(i.replace(t, " ")))
-                    }
-                }
+    function z(n) {
+        return (n + "").trim().split(/^|\s+/)
+    }
 
-                function ln(n, t, e) {
-                    return null == t ? function() {
-                        this.style.removeProperty(n)
-                    } : "function" == typeof t ? function() {
-                        var r = t.apply(this, arguments);
-                        null == r ? this.style.removeProperty(n) : this.style.setProperty(n, r, e)
-                    } : function() {
-                        this.style.setProperty(n, t, e)
-                    }
-                }
+    function L(n, t) {
+        function e() {
+            for (var e = -1; ++e < u;) n[e](this, t)
+        }
 
-                function cn(n, t) {
-                    return null == t ? function() {
-                        delete this[n]
-                    } : "function" == typeof t ? function() {
-                        var e = t.apply(this, arguments);
-                        null == e ? delete this[n] : this[n] = e
-                    } : function() {
-                        this[n] = t
-                    }
-                }
+        function r() {
+            for (var e = -1, r = t.apply(this, arguments); ++e < u;) n[e](this, r)
+        }
+        n = z(n).map(T);
+        var u = n.length;
+        return "function" == typeof t ? r : e
+    }
 
-                function fn(n) {
-                    return "function" == typeof n ? n : (n = u.ns.qualify(n)).local ? function() {
-                        return this.ownerDocument.createElementNS(n.space, n.local)
-                    } : function() {
-                        var t = this.ownerDocument,
-                            e = this.namespaceURI;
-                        return e === Q && t.documentElement.namespaceURI === Q ? t.createElement(n) : t.createElementNS(e, n)
-                    }
-                }
+    function T(n) {
+        var t = N(n);
+        return function(e, r) {
+            if (u = e.classList) return r ? u.add(n) : u.remove(n);
+            var u = e.getAttribute("class") || "";
+            r ? (t.lastIndex = 0, t.test(u) || e.setAttribute("class", C(u + " " + n))) : e.setAttribute("class", C(u.replace(t, " ")))
+        }
+    }
 
-                function sn() {
-                    var n = this.parentNode;
-                    n && n.removeChild(this)
-                }
+    function q(n, t, e) {
+        function r() {
+            this.style.removeProperty(n)
+        }
 
-                function hn(n) {
-                    return {
-                        __data__: n
-                    }
-                }
+        function u() {
+            this.style.setProperty(n, t, e)
+        }
 
-                function pn(n) {
-                    return function() {
-                        return J(this, n)
-                    }
-                }
+        function i() {
+            var r = t.apply(this, arguments);
+            null == r ? this.style.removeProperty(n) : this.style.setProperty(n, r, e)
+        }
+        return null == t ? r : "function" == typeof t ? i : u
+    }
 
-                function gn(n) {
-                    return arguments.length || (n = d),
-                        function(t, e) {
-                            return t && e ? n(t.__data__, e.__data__) : !t - !e
-                        }
-                }
+    function R(n, t) {
+        function e() {
+            delete this[n]
+        }
 
-                function vn(n, t) {
-                    for (var e = 0, r = n.length; e < r; e++)
-                        for (var i, u = n[e], o = 0, a = u.length; o < a; o++)(i = u[o]) && t(i, o, e);
-                    return n
-                }
-
-                function dn(n) {
-                    return V(n, yn), n
-                }
-                u.ns = {
-                    prefix: nn,
-                    qualify: function(n) {
-                        var t = n.indexOf(":"),
-                            e = n;
-                        return t >= 0 && "xmlns" !== (e = n.slice(0, t)) && (n = n.slice(t + 1)), nn.hasOwnProperty(e) ? {
-                            space: nn[e],
-                            local: n
-                        } : n
-                    }
-                }, W.attr = function(n, t) {
-                    if (arguments.length < 2) {
-                        if ("string" == typeof n) {
-                            var e = this.node();
-                            return (n = u.ns.qualify(n)).local ? e.getAttributeNS(n.space, n.local) : e.getAttribute(n)
-                        }
-                        for (t in n) this.each(tn(t, n[t]));
-                        return this
-                    }
-                    return this.each(tn(n, t))
-                }, W.classed = function(n, t) {
-                    if (arguments.length < 2) {
-                        if ("string" == typeof n) {
-                            var e = this.node(),
-                                r = (n = un(n)).length,
-                                i = -1;
-                            if (t = e.classList) {
-                                for (; ++i < r;)
-                                    if (!t.contains(n[i])) return !1
-                            } else
-                                for (t = e.getAttribute("class"); ++i < r;)
-                                    if (!rn(n[i]).test(t)) return !1;
-                            return !0
-                        }
-                        for (t in n) this.each(on(t, n[t]));
-                        return this
-                    }
-                    return this.each(on(n, t))
-                }, W.style = function(n, t, e) {
-                    var r = arguments.length;
-                    if (r < 3) {
-                        if ("string" != typeof n) {
-                            for (e in r < 2 && (t = ""), n) this.each(ln(e, n[e], t));
-                            return this
-                        }
-                        if (r < 2) {
-                            var i = this.node();
-                            return f(i).getComputedStyle(i, null).getPropertyValue(n)
-                        }
-                        e = ""
-                    }
-                    return this.each(ln(n, t, e))
-                }, W.property = function(n, t) {
-                    if (arguments.length < 2) {
-                        if ("string" == typeof n) return this.node()[n];
-                        for (t in n) this.each(cn(t, n[t]));
-                        return this
-                    }
-                    return this.each(cn(n, t))
-                }, W.text = function(n) {
-                    return arguments.length ? this.each("function" == typeof n ? function() {
-                        var t = n.apply(this, arguments);
-                        this.textContent = null == t ? "" : t
-                    } : null == n ? function() {
-                        this.textContent = ""
-                    } : function() {
-                        this.textContent = n
-                    }) : this.node().textContent
-                }, W.html = function(n) {
-                    return arguments.length ? this.each("function" == typeof n ? function() {
-                        var t = n.apply(this, arguments);
-                        this.innerHTML = null == t ? "" : t
-                    } : null == n ? function() {
-                        this.innerHTML = ""
-                    } : function() {
-                        this.innerHTML = n
-                    }) : this.node().innerHTML
-                }, W.append = function(n) {
-                    return n = fn(n), this.select((function() {
-                        return this.appendChild(n.apply(this, arguments))
-                    }))
-                }, W.insert = function(n, t) {
-                    return n = fn(n), t = G(t), this.select((function() {
-                        return this.insertBefore(n.apply(this, arguments), t.apply(this, arguments) || null)
-                    }))
-                }, W.remove = function() {
-                    return this.each(sn)
-                }, W.data = function(n, t) {
-                    var e, r, i = -1,
-                        u = this.length;
-                    if (!arguments.length) {
-                        for (n = new Array(u = (e = this[0]).length); ++i < u;)(r = e[i]) && (n[i] = r.__data__);
-                        return n
-                    }
+        function r() {
+            this[n] = t
+        }
 
-                    function o(n, e) {
-                        var r, i, u, o = n.length,
-                            f = e.length,
-                            s = Math.min(o, f),
-                            h = new Array(f),
-                            p = new Array(f),
-                            g = new Array(o);
-                        if (t) {
-                            var v, d = new S,
-                                y = new Array(o);
-                            for (r = -1; ++r < o;)(i = n[r]) && (d.has(v = t.call(i, i.__data__, r)) ? g[r] = i : d.set(v, i), y[r] = v);
-                            for (r = -1; ++r < f;)(i = d.get(v = t.call(e, u = e[r], r))) ? !0 !== i && (h[r] = i, i.__data__ = u) : p[r] = hn(u), d.set(v, !0);
-                            for (r = -1; ++r < o;) r in y && !0 !== d.get(y[r]) && (g[r] = n[r])
-                        } else {
-                            for (r = -1; ++r < s;) i = n[r], u = e[r], i ? (i.__data__ = u, h[r] = i) : p[r] = hn(u);
-                            for (; r < f; ++r) p[r] = hn(e[r]);
-                            for (; r < o; ++r) g[r] = n[r]
-                        }
-                        p.update = h, p.parentNode = h.parentNode = g.parentNode = n.parentNode, a.push(p), l.push(h), c.push(g)
-                    }
-                    var a = dn([]),
-                        l = X([]),
-                        c = X([]);
-                    if ("function" == typeof n)
-                        for (; ++i < u;) o(e = this[i], n.call(e, e.parentNode.__data__, i));
-                    else
-                        for (; ++i < u;) o(e = this[i], n);
-                    return l.enter = function() {
-                        return a
-                    }, l.exit = function() {
-                        return c
-                    }, l
-                }, W.datum = function(n) {
-                    return arguments.length ? this.property("__data__", n) : this.property("__data__")
-                }, W.filter = function(n) {
-                    var t, e, r, i = [];
-                    "function" != typeof n && (n = pn(n));
-                    for (var u = 0, o = this.length; u < o; u++) {
-                        i.push(t = []), t.parentNode = (e = this[u]).parentNode;
-                        for (var a = 0, l = e.length; a < l; a++)(r = e[a]) && n.call(r, r.__data__, a, u) && t.push(r)
-                    }
-                    return X(i)
-                }, W.order = function() {
-                    for (var n = -1, t = this.length; ++n < t;)
-                        for (var e, r = this[n], i = r.length - 1, u = r[i]; --i >= 0;)(e = r[i]) && (u && u !== e.nextSibling && u.parentNode.insertBefore(e, u), u = e);
-                    return this
-                }, W.sort = function(n) {
-                    n = gn.apply(this, arguments);
-                    for (var t = -1, e = this.length; ++t < e;) this[t].sort(n);
-                    return this.order()
-                }, W.each = function(n) {
-                    return vn(this, (function(t, e, r) {
-                        n.call(t, t.__data__, e, r)
-                    }))
-                }, W.call = function(n) {
-                    var t = a(arguments);
-                    return n.apply(t[0] = this, t), this
-                }, W.empty = function() {
-                    return !this.node()
-                }, W.node = function() {
-                    for (var n = 0, t = this.length; n < t; n++)
-                        for (var e = this[n], r = 0, i = e.length; r < i; r++) {
-                            var u = e[r];
-                            if (u) return u
-                        }
-                    return null
-                }, W.size = function() {
-                    var n = 0;
-                    return vn(this, (function() {
-                        ++n
-                    })), n
-                };
-                var yn = [];
+        function u() {
+            var e = t.apply(this, arguments);
+            null == e ? delete this[n] : this[n] = e
+        }
+        return null == t ? e : "function" == typeof t ? u : r
+    }
 
-                function mn(n) {
-                    var t, e;
-                    return function(r, i, u) {
-                        var o, a = n[u].update,
-                            l = a.length;
-                        for (u != e && (e = u, t = 0), i >= t && (t = i + 1); !(o = a[t]) && ++t < l;);
-                        return o
-                    }
-                }
+    function D(n) {
+        return "function" == typeof n ? n : (n = Bo.ns.qualify(n)).local ? function() {
+            return this.ownerDocument.createElementNS(n.space, n.local)
+        } : function() {
+            return this.ownerDocument.createElementNS(this.namespaceURI, n)
+        }
+    }
 
-                function Mn(n, t, e) {
-                    var r = "__on" + n,
-                        i = n.indexOf("."),
-                        o = bn;
-                    i > 0 && (n = n.slice(0, i));
-                    var l = xn.get(n);
-
-                    function c() {
-                        var t = this[r];
-                        t && (this.removeEventListener(n, t, t.$), delete this[r])
-                    }
-                    return l && (n = l, o = wn), i ? t ? function() {
-                        var i = o(t, a(arguments));
-                        c.call(this), this.addEventListener(n, this[r] = i, i.$ = e), i._ = t
-                    } : c : t ? j : function() {
-                        var t, e = new RegExp("^__on([^.]+)" + u.requote(n) + "$");
-                        for (var r in this)
-                            if (t = r.match(e)) {
-                                var i = this[r];
-                                this.removeEventListener(t[1], i, i.$), delete this[r]
-                            }
-                    }
-                }
-                u.selection.enter = dn, u.selection.enter.prototype = yn, yn.append = W.append, yn.empty = W.empty, yn.node = W.node, yn.call = W.call, yn.size = W.size, yn.select = function(n) {
-                    for (var t, e, r, i, u, o = [], a = -1, l = this.length; ++a < l;) {
-                        r = (i = this[a]).update, o.push(t = []), t.parentNode = i.parentNode;
-                        for (var c = -1, f = i.length; ++c < f;)(u = i[c]) ? (t.push(r[c] = e = n.call(i.parentNode, u.__data__, c, a)), e.__data__ = u.__data__) : t.push(null)
-                    }
-                    return X(o)
-                }, yn.insert = function(n, t) {
-                    return arguments.length < 2 && (t = mn(this)), W.insert.call(this, n, t)
-                }, u.select = function(n) {
-                    var t;
-                    return "string" == typeof n ? (t = [$(n, l)]).parentNode = l.documentElement : (t = [n]).parentNode = c(n), X([t])
-                }, u.selectAll = function(n) {
-                    var t;
-                    return "string" == typeof n ? (t = a(B(n, l))).parentNode = l.documentElement : (t = a(n)).parentNode = null, X([t])
-                }, W.on = function(n, t, e) {
-                    var r = arguments.length;
-                    if (r < 3) {
-                        if ("string" != typeof n) {
-                            for (e in r < 2 && (t = !1), n) this.each(Mn(e, n[e], t));
-                            return this
-                        }
-                        if (r < 2) return (r = this.node()["__on" + n]) && r._;
-                        e = !1
-                    }
-                    return this.each(Mn(n, t, e))
-                };
-                var xn = u.map({
-                    mouseenter: "mouseover",
-                    mouseleave: "mouseout"
-                });
+    function P(n) {
+        return {
+            __data__: n
+        }
+    }
 
-                function bn(n, t) {
-                    return function(e) {
-                        var r = u.event;
-                        u.event = e, t[0] = this.__data__;
-                        try {
-                            n.apply(this, t)
-                        } finally {
-                            u.event = r
-                        }
-                    }
-                }
+    function U(n) {
+        return function() {
+            return ma(this, n)
+        }
+    }
 
-                function wn(n, t) {
-                    var e = bn(n, t);
-                    return function(n) {
-                        var t = n.relatedTarget;
-                        t && (t === this || 8 & t.compareDocumentPosition(this)) || e.call(this, n)
-                    }
-                }
-                l && xn.forEach((function(n) {
-                    "on" + n in l && xn.remove(n)
-                }));
-                var _n, kn = 0;
-
-                function Sn(n) {
-                    var t = ".dragsuppress-" + ++kn,
-                        e = "click" + t,
-                        r = u.select(f(n)).on("touchmove" + t, O).on("dragstart" + t, O).on("selectstart" + t, O);
-                    if (null == _n && (_n = !("onselectstart" in n) && P(n.style, "userSelect")), _n) {
-                        var i = c(n).style,
-                            o = i[_n];
-                        i[_n] = "none"
-                    }
-                    return function(n) {
-                        if (r.on(t, null), _n && (i[_n] = o), n) {
-                            var u = function() {
-                                r.on(e, null)
-                            };
-                            r.on(e, (function() {
-                                O(), u()
-                            }), !0), setTimeout(u, 0)
-                        }
-                    }
-                }
-                u.mouse = function(n) {
-                    return En(n, I())
-                };
-                var Nn = this.navigator && /WebKit/.test(this.navigator.userAgent) ? -1 : 0;
+    function j(t) {
+        return arguments.length || (t = n),
+            function(n, e) {
+                return n && e ? t(n.__data__, e.__data__) : !n - !e
+            }
+    }
 
-                function En(n, t) {
-                    t.changedTouches && (t = t.changedTouches[0]);
-                    var e = n.ownerSVGElement || n;
-                    if (e.createSVGPoint) {
-                        var r = e.createSVGPoint();
-                        if (Nn < 0) {
-                            var i = f(n);
-                            if (i.scrollX || i.scrollY) {
-                                var o = (e = u.select("body").append("svg").style({
-                                    position: "absolute",
-                                    top: 0,
-                                    left: 0,
-                                    margin: 0,
-                                    padding: 0,
-                                    border: "none"
-                                }, "important"))[0][0].getScreenCTM();
-                                Nn = !(o.f || o.e), e.remove()
-                            }
-                        }
-                        return Nn ? (r.x = t.pageX, r.y = t.pageY) : (r.x = t.clientX, r.y = t.clientY), [(r = r.matrixTransform(n.getScreenCTM().inverse())).x, r.y]
-                    }
-                    var a = n.getBoundingClientRect();
-                    return [t.clientX - a.left - n.clientLeft, t.clientY - a.top - n.clientTop]
-                }
+    function F(n, t) {
+        for (var e = 0, r = n.length; r > e; e++)
+            for (var u, i = n[e], o = 0, a = i.length; a > o; o++)(u = i[o]) && t(u, o, e);
+        return n
+    }
 
-                function An() {
-                    return u.event.changedTouches[0].identifier
-                }
-                u.touch = function(n, t, e) {
-                    if (arguments.length < 3 && (e = t, t = I().changedTouches), t)
-                        for (var r, i = 0, u = t.length; i < u; ++i)
-                            if ((r = t[i]).identifier === e) return En(n, r)
-                }, u.behavior.drag = function() {
-                    var n = Y(i, "drag", "dragstart", "dragend"),
-                        t = null,
-                        e = o(j, u.mouse, f, "mousemove", "mouseup"),
-                        r = o(An, u.touch, R, "touchmove", "touchend");
+    function H(n) {
+        return ga(n, Ma), n
+    }
 
-                    function i() {
-                        this.on("mousedown.drag", e).on("touchstart.drag", r)
-                    }
+    function O(n) {
+        var t, e;
+        return function(r, u, i) {
+            var o, a = n[i].update,
+                c = a.length;
+            for (i != e && (e = i, t = 0), u >= t && (t = u + 1); !(o = a[t]) && ++t < c;);
+            return o
+        }
+    }
 
-                    function o(e, r, i, o, a) {
-                        return function() {
-                            var l, c = this,
-                                f = u.event.target.correspondingElement || u.event.target,
-                                s = c.parentNode,
-                                h = n.of(c, arguments),
-                                p = 0,
-                                g = e(),
-                                v = ".drag" + (null == g ? "" : "-" + g),
-                                d = u.select(i(f)).on(o + v, M).on(a + v, x),
-                                y = Sn(f),
-                                m = r(s, g);
-
-                            function M() {
-                                var n, t, e = r(s, g);
-                                e && (n = e[0] - m[0], t = e[1] - m[1], p |= n | t, m = e, h({
-                                    type: "drag",
-                                    x: e[0] + l[0],
-                                    y: e[1] + l[1],
-                                    dx: n,
-                                    dy: t
-                                }))
-                            }
+    function Y() {
+        var n = this.__transition__;
+        n && ++n.active
+    }
 
-                            function x() {
-                                r(s, g) && (d.on(o + v, null).on(a + v, null), y(p), h({
-                                    type: "dragend"
-                                }))
-                            }
-                            l = t ? [(l = t.apply(c, arguments)).x - m[0], l.y - m[1]] : [0, 0], h({
-                                type: "dragstart"
-                            })
-                        }
-                    }
-                    return i.origin = function(n) {
-                        return arguments.length ? (t = n, i) : t
-                    }, u.rebind(i, n, "on")
-                }, u.touches = function(n, t) {
-                    return arguments.length < 2 && (t = I().touches), t ? a(t).map((function(t) {
-                        var e = En(n, t);
-                        return e.identifier = t.identifier, e
-                    })) : []
-                };
-                var Cn = 1e-6,
-                    zn = 1e-12,
-                    Ln = Math.PI,
-                    qn = 2 * Ln,
-                    Tn = qn - Cn,
-                    Rn = Ln / 2,
-                    Dn = Ln / 180,
-                    Pn = 180 / Ln;
+    function I(n, t, e) {
+        function r() {
+            var t = this[o];
+            t && (this.removeEventListener(n, t, t.$), delete this[o])
+        }
 
-                function Un(n) {
-                    return n > 0 ? 1 : n < 0 ? -1 : 0
-                }
+        function u() {
+            var u = c(t, Jo(arguments));
+            r.call(this), this.addEventListener(n, this[o] = u, u.$ = e), u._ = t
+        }
 
-                function jn(n, t, e) {
-                    return (t[0] - n[0]) * (e[1] - n[1]) - (t[1] - n[1]) * (e[0] - n[0])
+        function i() {
+            var t, e = new RegExp("^__on([^.]+)" + Bo.requote(n) + "$");
+            for (var r in this)
+                if (t = r.match(e)) {
+                    var u = this[r];
+                    this.removeEventListener(t[1], u, u.$), delete this[r]
                 }
+        }
+        var o = "__on" + n,
+            a = n.indexOf("."),
+            c = Z;
+        a > 0 && (n = n.slice(0, a));
+        var l = ba.get(n);
+        return l && (n = l, c = V), a ? t ? u : r : t ? y : i
+    }
 
-                function Fn(n) {
-                    return n > 1 ? 0 : n < -1 ? Ln : Math.acos(n)
-                }
+    function Z(n, t) {
+        return function(e) {
+            var r = Bo.event;
+            Bo.event = e, t[0] = this.__data__;
+            try {
+                n.apply(this, t)
+            } finally {
+                Bo.event = r
+            }
+        }
+    }
 
-                function Hn(n) {
-                    return n > 1 ? Rn : n < -1 ? -Rn : Math.asin(n)
-                }
+    function V(n, t) {
+        var e = Z(n, t);
+        return function(n) {
+            var t = this,
+                r = n.relatedTarget;
+            r && (r === t || 8 & r.compareDocumentPosition(t)) || e.call(t, n)
+        }
+    }
 
-                function On(n) {
-                    return ((n = Math.exp(n)) + 1 / n) / 2
-                }
+    function X() {
+        var n = ".dragsuppress-" + ++Sa,
+            t = "click" + n,
+            e = Bo.select(Qo).on("touchmove" + n, _).on("dragstart" + n, _).on("selectstart" + n, _);
+        if (wa) {
+            var r = Ko.style,
+                u = r[wa];
+            r[wa] = "none"
+        }
+        return function(i) {
+            function o() {
+                e.on(t, null)
+            }
+            e.on(n, null), wa && (r[wa] = u), i && (e.on(t, function() {
+                _(), o()
+            }, !0), setTimeout(o, 0))
+        }
+    }
 
-                function In(n) {
-                    return (n = Math.sin(n / 2)) * n
-                }
-                var Yn = Math.SQRT2;
-                u.interpolateZoom = function(n, t) {
-                    var e, r, i = n[0],
-                        u = n[1],
-                        o = n[2],
-                        a = t[0],
-                        l = t[1],
-                        c = t[2],
-                        f = a - i,
-                        s = l - u,
-                        h = f * f + s * s;
-                    if (h < zn) r = Math.log(c / o) / Yn, e = function(n) {
-                        return [i + n * f, u + n * s, o * Math.exp(Yn * n * r)]
-                    };
-                    else {
-                        var p = Math.sqrt(h),
-                            g = (c * c - o * o + 4 * h) / (2 * o * 2 * p),
-                            v = (c * c - o * o - 4 * h) / (2 * c * 2 * p),
-                            d = Math.log(Math.sqrt(g * g + 1) - g),
-                            y = Math.log(Math.sqrt(v * v + 1) - v);
-                        r = (y - d) / Yn, e = function(n) {
-                            var t, e = n * r,
-                                a = On(d),
-                                l = o / (2 * p) * (a * (t = Yn * e + d, ((t = Math.exp(2 * t)) - 1) / (t + 1)) - function(n) {
-                                    return ((n = Math.exp(n)) - 1 / n) / 2
-                                }(d));
-                            return [i + l * f, u + l * s, o * a / On(Yn * e + d)]
-                        }
-                    }
-                    return e.duration = 1e3 * r, e
-                }, u.behavior.zoom = function() {
-                    var n, t, e, r, i, o, a, c, s, h = {
-                            x: 0,
-                            y: 0,
-                            k: 1
-                        },
-                        p = [960, 500],
-                        g = Xn,
-                        v = 250,
-                        d = 0,
-                        y = "mousedown.zoom",
-                        m = "mousemove.zoom",
-                        M = "mouseup.zoom",
-                        x = "touchstart.zoom",
-                        b = Y(w, "zoomstart", "zoom", "zoomend");
+    function $(n, t) {
+        t.changedTouches && (t = t.changedTouches[0]);
+        var e = n.ownerSVGElement || n;
+        if (e.createSVGPoint) {
+            var r = e.createSVGPoint();
+            if (0 > ka && (Qo.scrollX || Qo.scrollY)) {
+                e = Bo.select("body").append("svg").style({
+                    position: "absolute",
+                    top: 0,
+                    left: 0,
+                    margin: 0,
+                    padding: 0,
+                    border: "none"
+                }, "important");
+                var u = e[0][0].getScreenCTM();
+                ka = !(u.f || u.e), e.remove()
+            }
+            return ka ? (r.x = t.pageX, r.y = t.pageY) : (r.x = t.clientX, r.y = t.clientY), r = r.matrixTransform(n.getScreenCTM().inverse()), [r.x, r.y]
+        }
+        var i = n.getBoundingClientRect();
+        return [t.clientX - i.left - n.clientLeft, t.clientY - i.top - n.clientTop]
+    }
 
-                    function w(n) {
-                        n.on(y, L).on(Vn + ".zoom", T).on("dblclick.zoom", R).on(x, q)
-                    }
+    function B() {
+        return Bo.event.changedTouches[0].identifier
+    }
 
-                    function _(n) {
-                        return [(n[0] - h.x) / h.k, (n[1] - h.y) / h.k]
-                    }
+    function W() {
+        return Bo.event.target
+    }
 
-                    function k(n) {
-                        h.k = Math.max(g[0], Math.min(g[1], n))
-                    }
+    function J() {
+        return Qo
+    }
 
-                    function S(n, t) {
-                        t = function(n) {
-                            return [n[0] * h.k + h.x, n[1] * h.k + h.y]
-                        }(t), h.x += n[0] - t[0], h.y += n[1] - t[1]
-                    }
+    function G(n) {
+        return n > 0 ? 1 : 0 > n ? -1 : 0
+    }
 
-                    function N(n, e, r, i) {
-                        n.__chart__ = {
-                            x: h.x,
-                            y: h.y,
-                            k: h.k
-                        }, k(Math.pow(2, i)), S(t = e, r), n = u.select(n), v > 0 && (n = n.transition().duration(v)), n.call(w.event)
-                    }
+    function K(n, t, e) {
+        return (t[0] - n[0]) * (e[1] - n[1]) - (t[1] - n[1]) * (e[0] - n[0])
+    }
 
-                    function E() {
-                        a && a.domain(o.range().map((function(n) {
-                            return (n - h.x) / h.k
-                        })).map(o.invert)), s && s.domain(c.range().map((function(n) {
-                            return (n - h.y) / h.k
-                        })).map(c.invert))
-                    }
+    function Q(n) {
+        return n > 1 ? 0 : -1 > n ? Ea : Math.acos(n)
+    }
 
-                    function A(n) {
-                        d++ || n({
-                            type: "zoomstart"
-                        })
-                    }
+    function nt(n) {
+        return n > 1 ? Ca : -1 > n ? -Ca : Math.asin(n)
+    }
 
-                    function C(n) {
-                        E(), n({
-                            type: "zoom",
-                            scale: h.k,
-                            translate: [h.x, h.y]
-                        })
-                    }
+    function tt(n) {
+        return ((n = Math.exp(n)) - 1 / n) / 2
+    }
 
-                    function z(n) {
-                        --d || (n({
-                            type: "zoomend"
-                        }), t = null)
-                    }
+    function et(n) {
+        return ((n = Math.exp(n)) + 1 / n) / 2
+    }
 
-                    function L() {
-                        var n = this,
-                            t = b.of(n, arguments),
-                            e = 0,
-                            r = u.select(f(n)).on(m, a).on(M, l),
-                            i = _(u.mouse(n)),
-                            o = Sn(n);
+    function rt(n) {
+        return ((n = Math.exp(2 * n)) - 1) / (n + 1)
+    }
 
-                        function a() {
-                            e = 1, S(u.mouse(n), i), C(t)
-                        }
+    function ut(n) {
+        return (n = Math.sin(n / 2)) * n
+    }
 
-                        function l() {
-                            r.on(m, null).on(M, null), o(e), z(t)
-                        }
-                        ba.call(n), A(t)
-                    }
+    function it() {}
 
-                    function q() {
-                        var n, t = this,
-                            e = b.of(t, arguments),
-                            r = {},
-                            o = 0,
-                            a = ".zoom-" + u.event.changedTouches[0].identifier,
-                            l = "touchmove" + a,
-                            c = "touchend" + a,
-                            f = [],
-                            s = u.select(t),
-                            p = Sn(t);
-
-                        function g() {
-                            var e = u.touches(t);
-                            return n = h.k, e.forEach((function(n) {
-                                n.identifier in r && (r[n.identifier] = _(n))
-                            })), e
-                        }
+    function ot(n, t, e) {
+        return this instanceof ot ? (this.h = +n, this.s = +t, void(this.l = +e)) : arguments.length < 2 ? n instanceof ot ? new ot(n.h, n.s, n.l) : Mt("" + n, _t, ot) : new ot(n, t, e)
+    }
 
-                        function v() {
-                            var n = u.event.target;
-                            u.select(n).on(l, d).on(c, m), f.push(n);
-                            for (var e = u.event.changedTouches, a = 0, s = e.length; a < s; ++a) r[e[a].identifier] = null;
-                            var p = g(),
-                                v = Date.now();
-                            if (1 === p.length) {
-                                if (v - i < 500) {
-                                    var y = p[0];
-                                    N(t, y, r[y.identifier], Math.floor(Math.log(h.k) / Math.LN2) + 1), O()
-                                }
-                                i = v
-                            } else if (p.length > 1) {
-                                y = p[0];
-                                var M = p[1],
-                                    x = y[0] - M[0],
-                                    b = y[1] - M[1];
-                                o = x * x + b * b
-                            }
-                        }
+    function at(n, t, e) {
+        function r(n) {
+            return n > 360 ? n -= 360 : 0 > n && (n += 360), 60 > n ? i + (o - i) * n / 60 : 180 > n ? o : 240 > n ? i + (o - i) * (240 - n) / 60 : i
+        }
 
-                        function d() {
-                            var a, l, c, f, s = u.touches(t);
-                            ba.call(t);
-                            for (var h = 0, p = s.length; h < p; ++h, f = null)
-                                if (c = s[h], f = r[c.identifier]) {
-                                    if (l) break;
-                                    a = c, l = f
-                                } if (f) {
-                                var g = (g = c[0] - a[0]) * g + (g = c[1] - a[1]) * g,
-                                    v = o && Math.sqrt(g / o);
-                                a = [(a[0] + c[0]) / 2, (a[1] + c[1]) / 2], l = [(l[0] + f[0]) / 2, (l[1] + f[1]) / 2], k(v * n)
-                            }
-                            i = null, S(a, l), C(e)
-                        }
+        function u(n) {
+            return Math.round(255 * r(n))
+        }
+        var i, o;
+        return n = isNaN(n) ? 0 : (n %= 360) < 0 ? n + 360 : n, t = isNaN(t) ? 0 : 0 > t ? 0 : t > 1 ? 1 : t, e = 0 > e ? 0 : e > 1 ? 1 : e, o = .5 >= e ? e * (1 + t) : e + t - e * t, i = 2 * e - o, new dt(u(n + 120), u(n), u(n - 120))
+    }
 
-                        function m() {
-                            if (u.event.touches.length) {
-                                for (var n = u.event.changedTouches, t = 0, i = n.length; t < i; ++t) delete r[n[t].identifier];
-                                for (var o in r) return void g()
-                            }
-                            u.selectAll(f).on(a, null), s.on(y, L).on(x, q), p(), z(e)
-                        }
-                        v(), A(e), s.on(y, null).on(x, v)
-                    }
+    function ct(n, t, e) {
+        return this instanceof ct ? (this.h = +n, this.c = +t, void(this.l = +e)) : arguments.length < 2 ? n instanceof ct ? new ct(n.h, n.c, n.l) : n instanceof st ? ht(n.l, n.a, n.b) : ht((n = bt((n = Bo.rgb(n)).r, n.g, n.b)).l, n.a, n.b) : new ct(n, t, e)
+    }
 
-                    function T() {
-                        var i = b.of(this, arguments);
-                        r ? clearTimeout(r) : (ba.call(this), n = _(t = e || u.mouse(this)), A(i)), r = setTimeout((function() {
-                            r = null, z(i)
-                        }), 50), O(), k(Math.pow(2, .002 * Zn()) * h.k), S(t, n), C(i)
-                    }
+    function lt(n, t, e) {
+        return isNaN(n) && (n = 0), isNaN(t) && (t = 0), new st(e, Math.cos(n *= La) * t, Math.sin(n) * t)
+    }
 
-                    function R() {
-                        var n = u.mouse(this),
-                            t = Math.log(h.k) / Math.LN2;
-                        N(this, n, _(n), u.event.shiftKey ? Math.ceil(t) - 1 : Math.floor(t) + 1)
-                    }
-                    return Vn || (Vn = "onwheel" in l ? (Zn = function() {
-                        return -u.event.deltaY * (u.event.deltaMode ? 120 : 1)
-                    }, "wheel") : "onmousewheel" in l ? (Zn = function() {
-                        return u.event.wheelDelta
-                    }, "mousewheel") : (Zn = function() {
-                        return -u.event.detail
-                    }, "MozMousePixelScroll")), w.event = function(n) {
-                        n.each((function() {
-                            var n = b.of(this, arguments),
-                                e = h;
-                            ka ? u.select(this).transition().each("start.zoom", (function() {
-                                h = this.__chart__ || {
-                                    x: 0,
-                                    y: 0,
-                                    k: 1
-                                }, A(n)
-                            })).tween("zoom:zoom", (function() {
-                                var r = p[0],
-                                    i = p[1],
-                                    o = t ? t[0] : r / 2,
-                                    a = t ? t[1] : i / 2,
-                                    l = u.interpolateZoom([(o - h.x) / h.k, (a - h.y) / h.k, r / h.k], [(o - e.x) / e.k, (a - e.y) / e.k, r / e.k]);
-                                return function(t) {
-                                    var e = l(t),
-                                        i = r / e[2];
-                                    this.__chart__ = h = {
-                                        x: o - e[0] * i,
-                                        y: a - e[1] * i,
-                                        k: i
-                                    }, C(n)
-                                }
-                            })).each("interrupt.zoom", (function() {
-                                z(n)
-                            })).each("end.zoom", (function() {
-                                z(n)
-                            })) : (this.__chart__ = h, A(n), C(n), z(n))
-                        }))
-                    }, w.translate = function(n) {
-                        return arguments.length ? (h = {
-                            x: +n[0],
-                            y: +n[1],
-                            k: h.k
-                        }, E(), w) : [h.x, h.y]
-                    }, w.scale = function(n) {
-                        return arguments.length ? (h = {
-                            x: h.x,
-                            y: h.y,
-                            k: null
-                        }, k(+n), E(), w) : h.k
-                    }, w.scaleExtent = function(n) {
-                        return arguments.length ? (g = null == n ? Xn : [+n[0], +n[1]], w) : g
-                    }, w.center = function(n) {
-                        return arguments.length ? (e = n && [+n[0], +n[1]], w) : e
-                    }, w.size = function(n) {
-                        return arguments.length ? (p = n && [+n[0], +n[1]], w) : p
-                    }, w.duration = function(n) {
-                        return arguments.length ? (v = +n, w) : v
-                    }, w.x = function(n) {
-                        return arguments.length ? (a = n, o = n.copy(), h = {
-                            x: 0,
-                            y: 0,
-                            k: 1
-                        }, w) : a
-                    }, w.y = function(n) {
-                        return arguments.length ? (s = n, c = n.copy(), h = {
-                            x: 0,
-                            y: 0,
-                            k: 1
-                        }, w) : s
-                    }, u.rebind(w, b, "on")
-                };
-                var Zn, Vn, Xn = [0, 1 / 0];
+    function st(n, t, e) {
+        return this instanceof st ? (this.l = +n, this.a = +t, void(this.b = +e)) : arguments.length < 2 ? n instanceof st ? new st(n.l, n.a, n.b) : n instanceof ct ? lt(n.h, n.c, n.l) : bt((n = dt(n)).r, n.g, n.b) : new st(n, t, e)
+    }
 
-                function $n() {}
+    function ft(n, t, e) {
+        var r = (n + 16) / 116,
+            u = r + t / 500,
+            i = r - e / 200;
+        return u = gt(u) * Ya, r = gt(r) * Ia, i = gt(i) * Za, new dt(vt(3.2404542 * u - 1.5371385 * r - .4985314 * i), vt(-.969266 * u + 1.8760108 * r + .041556 * i), vt(.0556434 * u - .2040259 * r + 1.0572252 * i))
+    }
 
-                function Bn(n, t, e) {
-                    return this instanceof Bn ? (this.h = +n, this.s = +t, void(this.l = +e)) : arguments.length < 2 ? n instanceof Bn ? new Bn(n.h, n.s, n.l) : pt("" + n, gt, Bn) : new Bn(n, t, e)
-                }
-                u.color = $n, $n.prototype.toString = function() {
-                    return this.rgb() + ""
-                }, u.hsl = Bn;
-                var Jn = Bn.prototype = new $n;
+    function ht(n, t, e) {
+        return n > 0 ? new ct(Math.atan2(e, t) * Ta, Math.sqrt(t * t + e * e), n) : new ct(0 / 0, 0 / 0, n)
+    }
 
-                function Wn(n, t, e) {
-                    var r, i;
+    function gt(n) {
+        return n > .206893034 ? n * n * n : (n - 4 / 29) / 7.787037
+    }
 
-                    function u(n) {
-                        return Math.round(255 * function(n) {
-                            return n > 360 ? n -= 360 : n < 0 && (n += 360), n < 60 ? r + (i - r) * n / 60 : n < 180 ? i : n < 240 ? r + (i - r) * (240 - n) / 60 : r
-                        }(n))
-                    }
-                    return n = isNaN(n) ? 0 : (n %= 360) < 0 ? n + 360 : n, t = isNaN(t) || t < 0 ? 0 : t > 1 ? 1 : t, r = 2 * (e = e < 0 ? 0 : e > 1 ? 1 : e) - (i = e <= .5 ? e * (1 + t) : e + t - e * t), new lt(u(n + 120), u(n), u(n - 120))
-                }
+    function pt(n) {
+        return n > .008856 ? Math.pow(n, 1 / 3) : 7.787037 * n + 4 / 29
+    }
 
-                function Gn(n, t, e) {
-                    return this instanceof Gn ? (this.h = +n, this.c = +t, void(this.l = +e)) : arguments.length < 2 ? n instanceof Gn ? new Gn(n.h, n.c, n.l) : it(n instanceof nt ? n.l : (n = vt((n = u.rgb(n)).r, n.g, n.b)).l, n.a, n.b) : new Gn(n, t, e)
-                }
-                Jn.brighter = function(n) {
-                    return n = Math.pow(.7, arguments.length ? n : 1), new Bn(this.h, this.s, this.l / n)
-                }, Jn.darker = function(n) {
-                    return n = Math.pow(.7, arguments.length ? n : 1), new Bn(this.h, this.s, n * this.l)
-                }, Jn.rgb = function() {
-                    return Wn(this.h, this.s, this.l)
-                }, u.hcl = Gn;
-                var Kn = Gn.prototype = new $n;
+    function vt(n) {
+        return Math.round(255 * (.00304 >= n ? 12.92 * n : 1.055 * Math.pow(n, 1 / 2.4) - .055))
+    }
 
-                function Qn(n, t, e) {
-                    return isNaN(n) && (n = 0), isNaN(t) && (t = 0), new nt(e, Math.cos(n *= Dn) * t, Math.sin(n) * t)
-                }
+    function dt(n, t, e) {
+        return this instanceof dt ? (this.r = ~~n, this.g = ~~t, void(this.b = ~~e)) : arguments.length < 2 ? n instanceof dt ? new dt(n.r, n.g, n.b) : Mt("" + n, dt, at) : new dt(n, t, e)
+    }
 
-                function nt(n, t, e) {
-                    return this instanceof nt ? (this.l = +n, this.a = +t, void(this.b = +e)) : arguments.length < 2 ? n instanceof nt ? new nt(n.l, n.a, n.b) : n instanceof Gn ? Qn(n.h, n.c, n.l) : vt((n = lt(n)).r, n.g, n.b) : new nt(n, t, e)
-                }
-                Kn.brighter = function(n) {
-                    return new Gn(this.h, this.c, Math.min(100, this.l + tt * (arguments.length ? n : 1)))
-                }, Kn.darker = function(n) {
-                    return new Gn(this.h, this.c, Math.max(0, this.l - tt * (arguments.length ? n : 1)))
-                }, Kn.rgb = function() {
-                    return Qn(this.h, this.c, this.l).rgb()
-                }, u.lab = nt;
-                var tt = 18,
-                    et = nt.prototype = new $n;
+    function mt(n) {
+        return new dt(n >> 16, 255 & n >> 8, 255 & n)
+    }
 
-                function rt(n, t, e) {
-                    var r = (n + 16) / 116,
-                        i = r + t / 500,
-                        u = r - e / 200;
-                    return new lt(at(3.2404542 * (i = .95047 * ut(i)) - 1.5371385 * (r = 1 * ut(r)) - .4985314 * (u = 1.08883 * ut(u))), at(-.969266 * i + 1.8760108 * r + .041556 * u), at(.0556434 * i - .2040259 * r + 1.0572252 * u))
-                }
+    function yt(n) {
+        return mt(n) + ""
+    }
 
-                function it(n, t, e) {
-                    return n > 0 ? new Gn(Math.atan2(e, t) * Pn, Math.sqrt(t * t + e * e), n) : new Gn(NaN, NaN, n)
-                }
+    function xt(n) {
+        return 16 > n ? "0" + Math.max(0, n).toString(16) : Math.min(255, n).toString(16)
+    }
 
-                function ut(n) {
-                    return n > .206893034 ? n * n * n : (n - 4 / 29) / 7.787037
-                }
+    function Mt(n, t, e) {
+        var r, u, i, o = 0,
+            a = 0,
+            c = 0;
+        if (r = /([a-z]+)\((.*)\)/i.exec(n)) switch (u = r[2].split(","), r[1]) {
+            case "hsl":
+                return e(parseFloat(u[0]), parseFloat(u[1]) / 100, parseFloat(u[2]) / 100);
+            case "rgb":
+                return t(St(u[0]), St(u[1]), St(u[2]))
+        }
+        return (i = $a.get(n)) ? t(i.r, i.g, i.b) : (null == n || "#" !== n.charAt(0) || isNaN(i = parseInt(n.slice(1), 16)) || (4 === n.length ? (o = (3840 & i) >> 4, o = o >> 4 | o, a = 240 & i, a = a >> 4 | a, c = 15 & i, c = c << 4 | c) : 7 === n.length && (o = (16711680 & i) >> 16, a = (65280 & i) >> 8, c = 255 & i)), t(o, a, c))
+    }
 
-                function ot(n) {
-                    return n > .008856 ? Math.pow(n, 1 / 3) : 7.787037 * n + 4 / 29
-                }
+    function _t(n, t, e) {
+        var r, u, i = Math.min(n /= 255, t /= 255, e /= 255),
+            o = Math.max(n, t, e),
+            a = o - i,
+            c = (o + i) / 2;
+        return a ? (u = .5 > c ? a / (o + i) : a / (2 - o - i), r = n == o ? (t - e) / a + (e > t ? 6 : 0) : t == o ? (e - n) / a + 2 : (n - t) / a + 4, r *= 60) : (r = 0 / 0, u = c > 0 && 1 > c ? 0 : r), new ot(r, u, c)
+    }
 
-                function at(n) {
-                    return Math.round(255 * (n <= .00304 ? 12.92 * n : 1.055 * Math.pow(n, 1 / 2.4) - .055))
-                }
+    function bt(n, t, e) {
+        n = wt(n), t = wt(t), e = wt(e);
+        var r = pt((.4124564 * n + .3575761 * t + .1804375 * e) / Ya),
+            u = pt((.2126729 * n + .7151522 * t + .072175 * e) / Ia),
+            i = pt((.0193339 * n + .119192 * t + .9503041 * e) / Za);
+        return st(116 * u - 16, 500 * (r - u), 200 * (u - i))
+    }
 
-                function lt(n, t, e) {
-                    return this instanceof lt ? (this.r = ~~n, this.g = ~~t, void(this.b = ~~e)) : arguments.length < 2 ? n instanceof lt ? new lt(n.r, n.g, n.b) : pt("" + n, lt, Wn) : new lt(n, t, e)
-                }
+    function wt(n) {
+        return (n /= 255) <= .04045 ? n / 12.92 : Math.pow((n + .055) / 1.055, 2.4)
+    }
 
-                function ct(n) {
-                    return new lt(n >> 16, n >> 8 & 255, 255 & n)
-                }
+    function St(n) {
+        var t = parseFloat(n);
+        return "%" === n.charAt(n.length - 1) ? Math.round(2.55 * t) : t
+    }
 
-                function ft(n) {
-                    return ct(n) + ""
-                }
-                et.brighter = function(n) {
-                    return new nt(Math.min(100, this.l + tt * (arguments.length ? n : 1)), this.a, this.b)
-                }, et.darker = function(n) {
-                    return new nt(Math.max(0, this.l - tt * (arguments.length ? n : 1)), this.a, this.b)
-                }, et.rgb = function() {
-                    return rt(this.l, this.a, this.b)
-                }, u.rgb = lt;
-                var st = lt.prototype = new $n;
+    function kt(n) {
+        return "function" == typeof n ? n : function() {
+            return n
+        }
+    }
 
-                function ht(n) {
-                    return n < 16 ? "0" + Math.max(0, n).toString(16) : Math.min(255, n).toString(16)
-                }
+    function Et(n) {
+        return n
+    }
 
-                function pt(n, t, e) {
-                    var r, i, u, o = 0,
-                        a = 0,
-                        l = 0;
-                    if (r = /([a-z]+)\((.*)\)/.exec(n = n.toLowerCase())) switch (i = r[2].split(","), r[1]) {
-                        case "hsl":
-                            return e(parseFloat(i[0]), parseFloat(i[1]) / 100, parseFloat(i[2]) / 100);
-                        case "rgb":
-                            return t(yt(i[0]), yt(i[1]), yt(i[2]))
-                    }
-                    return (u = mt.get(n)) ? t(u.r, u.g, u.b) : (null == n || "#" !== n.charAt(0) || isNaN(u = parseInt(n.slice(1), 16)) || (4 === n.length ? (o = (3840 & u) >> 4, o |= o >> 4, a = 240 & u, a |= a >> 4, l = 15 & u, l |= l << 4) : 7 === n.length && (o = (16711680 & u) >> 16, a = (65280 & u) >> 8, l = 255 & u)), t(o, a, l))
+    function At(n) {
+        return function(t, e, r) {
+            return 2 === arguments.length && "function" == typeof e && (r = e, e = null), Ct(t, e, n, r)
+        }
+    }
+
+    function Ct(n, t, e, r) {
+        function u() {
+            var n, t = c.status;
+            if (!t && zt(c) || t >= 200 && 300 > t || 304 === t) {
+                try {
+                    n = e.call(i, c)
+                } catch (r) {
+                    return o.error.call(i, r), void 0
                 }
+                o.load.call(i, n)
+            } else o.error.call(i, c)
+        }
+        var i = {},
+            o = Bo.dispatch("beforesend", "progress", "load", "error"),
+            a = {},
+            c = new XMLHttpRequest,
+            l = null;
+        return !Qo.XDomainRequest || "withCredentials" in c || !/^(http(s)?:)?\/\//.test(n) || (c = new XDomainRequest), "onload" in c ? c.onload = c.onerror = u : c.onreadystatechange = function() {
+            c.readyState > 3 && u()
+        }, c.onprogress = function(n) {
+            var t = Bo.event;
+            Bo.event = n;
+            try {
+                o.progress.call(i, c)
+            } finally {
+                Bo.event = t
+            }
+        }, i.header = function(n, t) {
+            return n = (n + "").toLowerCase(), arguments.length < 2 ? a[n] : (null == t ? delete a[n] : a[n] = t + "", i)
+        }, i.mimeType = function(n) {
+            return arguments.length ? (t = null == n ? null : n + "", i) : t
+        }, i.responseType = function(n) {
+            return arguments.length ? (l = n, i) : l
+        }, i.response = function(n) {
+            return e = n, i
+        }, ["get", "post"].forEach(function(n) {
+            i[n] = function() {
+                return i.send.apply(i, [n].concat(Jo(arguments)))
+            }
+        }), i.send = function(e, r, u) {
+            if (2 === arguments.length && "function" == typeof r && (u = r, r = null), c.open(e, n, !0), null == t || "accept" in a || (a.accept = t + ",*/*"), c.setRequestHeader)
+                for (var s in a) c.setRequestHeader(s, a[s]);
+            return null != t && c.overrideMimeType && c.overrideMimeType(t), null != l && (c.responseType = l), null != u && i.on("error", u).on("load", function(n) {
+                u(null, n)
+            }), o.beforesend.call(i, c), c.send(null == r ? null : r), i
+        }, i.abort = function() {
+            return c.abort(), i
+        }, Bo.rebind(i, o, "on"), null == r ? i : i.get(Nt(r))
+    }
 
-                function gt(n, t, e) {
-                    var r, i, u = Math.min(n /= 255, t /= 255, e /= 255),
-                        o = Math.max(n, t, e),
-                        a = o - u,
-                        l = (o + u) / 2;
-                    return a ? (i = l < .5 ? a / (o + u) : a / (2 - o - u), r = n == o ? (t - e) / a + (t < e ? 6 : 0) : t == o ? (e - n) / a + 2 : (n - t) / a + 4, r *= 60) : (r = NaN, i = l > 0 && l < 1 ? 0 : r), new Bn(r, i, l)
-                }
-
-                function vt(n, t, e) {
-                    var r = ot((.4124564 * (n = dt(n)) + .3575761 * (t = dt(t)) + .1804375 * (e = dt(e))) / .95047),
-                        i = ot((.2126729 * n + .7151522 * t + .072175 * e) / 1);
-                    return nt(116 * i - 16, 500 * (r - i), 200 * (i - ot((.0193339 * n + .119192 * t + .9503041 * e) / 1.08883)))
-                }
-
-                function dt(n) {
-                    return (n /= 255) <= .04045 ? n / 12.92 : Math.pow((n + .055) / 1.055, 2.4)
-                }
-
-                function yt(n) {
-                    var t = parseFloat(n);
-                    return "%" === n.charAt(n.length - 1) ? Math.round(2.55 * t) : t
-                }
-                st.brighter = function(n) {
-                    n = Math.pow(.7, arguments.length ? n : 1);
-                    var t = this.r,
-                        e = this.g,
-                        r = this.b,
-                        i = 30;
-                    return t || e || r ? (t && t < i && (t = i), e && e < i && (e = i), r && r < i && (r = i), new lt(Math.min(255, t / n), Math.min(255, e / n), Math.min(255, r / n))) : new lt(i, i, i)
-                }, st.darker = function(n) {
-                    return new lt((n = Math.pow(.7, arguments.length ? n : 1)) * this.r, n * this.g, n * this.b)
-                }, st.hsl = function() {
-                    return gt(this.r, this.g, this.b)
-                }, st.toString = function() {
-                    return "#" + ht(this.r) + ht(this.g) + ht(this.b)
-                };
-                var mt = u.map({
-                    aliceblue: 15792383,
-                    antiquewhite: 16444375,
-                    aqua: 65535,
-                    aquamarine: 8388564,
-                    azure: 15794175,
-                    beige: 16119260,
-                    bisque: 16770244,
-                    black: 0,
-                    blanchedalmond: 16772045,
-                    blue: 255,
-                    blueviolet: 9055202,
-                    brown: 10824234,
-                    burlywood: 14596231,
-                    cadetblue: 6266528,
-                    chartreuse: 8388352,
-                    chocolate: 13789470,
-                    coral: 16744272,
-                    cornflowerblue: 6591981,
-                    cornsilk: 16775388,
-                    crimson: 14423100,
-                    cyan: 65535,
-                    darkblue: 139,
-                    darkcyan: 35723,
-                    darkgoldenrod: 12092939,
-                    darkgray: 11119017,
-                    darkgreen: 25600,
-                    darkgrey: 11119017,
-                    darkkhaki: 12433259,
-                    darkmagenta: 9109643,
-                    darkolivegreen: 5597999,
-                    darkorange: 16747520,
-                    darkorchid: 10040012,
-                    darkred: 9109504,
-                    darksalmon: 15308410,
-                    darkseagreen: 9419919,
-                    darkslateblue: 4734347,
-                    darkslategray: 3100495,
-                    darkslategrey: 3100495,
-                    darkturquoise: 52945,
-                    darkviolet: 9699539,
-                    deeppink: 16716947,
-                    deepskyblue: 49151,
-                    dimgray: 6908265,
-                    dimgrey: 6908265,
-                    dodgerblue: 2003199,
-                    firebrick: 11674146,
-                    floralwhite: 16775920,
-                    forestgreen: 2263842,
-                    fuchsia: 16711935,
-                    gainsboro: 14474460,
-                    ghostwhite: 16316671,
-                    gold: 16766720,
-                    goldenrod: 14329120,
-                    gray: 8421504,
-                    green: 32768,
-                    greenyellow: 11403055,
-                    grey: 8421504,
-                    honeydew: 15794160,
-                    hotpink: 16738740,
-                    indianred: 13458524,
-                    indigo: 4915330,
-                    ivory: 16777200,
-                    khaki: 15787660,
-                    lavender: 15132410,
-                    lavenderblush: 16773365,
-                    lawngreen: 8190976,
-                    lemonchiffon: 16775885,
-                    lightblue: 11393254,
-                    lightcoral: 15761536,
-                    lightcyan: 14745599,
-                    lightgoldenrodyellow: 16448210,
-                    lightgray: 13882323,
-                    lightgreen: 9498256,
-                    lightgrey: 13882323,
-                    lightpink: 16758465,
-                    lightsalmon: 16752762,
-                    lightseagreen: 2142890,
-                    lightskyblue: 8900346,
-                    lightslategray: 7833753,
-                    lightslategrey: 7833753,
-                    lightsteelblue: 11584734,
-                    lightyellow: 16777184,
-                    lime: 65280,
-                    limegreen: 3329330,
-                    linen: 16445670,
-                    magenta: 16711935,
-                    maroon: 8388608,
-                    mediumaquamarine: 6737322,
-                    mediumblue: 205,
-                    mediumorchid: 12211667,
-                    mediumpurple: 9662683,
-                    mediumseagreen: 3978097,
-                    mediumslateblue: 8087790,
-                    mediumspringgreen: 64154,
-                    mediumturquoise: 4772300,
-                    mediumvioletred: 13047173,
-                    midnightblue: 1644912,
-                    mintcream: 16121850,
-                    mistyrose: 16770273,
-                    moccasin: 16770229,
-                    navajowhite: 16768685,
-                    navy: 128,
-                    oldlace: 16643558,
-                    olive: 8421376,
-                    olivedrab: 7048739,
-                    orange: 16753920,
-                    orangered: 16729344,
-                    orchid: 14315734,
-                    palegoldenrod: 15657130,
-                    palegreen: 10025880,
-                    paleturquoise: 11529966,
-                    palevioletred: 14381203,
-                    papayawhip: 16773077,
-                    peachpuff: 16767673,
-                    peru: 13468991,
-                    pink: 16761035,
-                    plum: 14524637,
-                    powderblue: 11591910,
-                    purple: 8388736,
-                    rebeccapurple: 6697881,
-                    red: 16711680,
-                    rosybrown: 12357519,
-                    royalblue: 4286945,
-                    saddlebrown: 9127187,
-                    salmon: 16416882,
-                    sandybrown: 16032864,
-                    seagreen: 3050327,
-                    seashell: 16774638,
-                    sienna: 10506797,
-                    silver: 12632256,
-                    skyblue: 8900331,
-                    slateblue: 6970061,
-                    slategray: 7372944,
-                    slategrey: 7372944,
-                    snow: 16775930,
-                    springgreen: 65407,
-                    steelblue: 4620980,
-                    tan: 13808780,
-                    teal: 32896,
-                    thistle: 14204888,
-                    tomato: 16737095,
-                    turquoise: 4251856,
-                    violet: 15631086,
-                    wheat: 16113331,
-                    white: 16777215,
-                    whitesmoke: 16119285,
-                    yellow: 16776960,
-                    yellowgreen: 10145074
-                });
+    function Nt(n) {
+        return 1 === n.length ? function(t, e) {
+            n(null == t ? e : null)
+        } : n
+    }
 
-                function Mt(n) {
-                    return "function" == typeof n ? n : function() {
-                        return n
-                    }
-                }
+    function zt(n) {
+        var t = n.responseType;
+        return t && "text" !== t ? n.response : n.responseText
+    }
 
-                function xt(n) {
-                    return function(t, e, r) {
-                        return 2 === arguments.length && "function" == typeof e && (r = e, e = null), bt(t, e, n, r)
-                    }
-                }
+    function Lt() {
+        var n = Tt(),
+            t = qt() - n;
+        t > 24 ? (isFinite(t) && (clearTimeout(Ga), Ga = setTimeout(Lt, t)), Ja = 0) : (Ja = 1, Qa(Lt))
+    }
 
-                function bt(n, t, e, r) {
-                    var i = {},
-                        o = u.dispatch("beforesend", "progress", "load", "error"),
-                        l = {},
-                        c = new XMLHttpRequest,
-                        f = null;
-
-                    function s() {
-                        var n, t = c.status;
-                        if (!t && function(n) {
-                                var t = n.responseType;
-                                return t && "text" !== t ? n.response : n.responseText
-                            }(c) || t >= 200 && t < 300 || 304 === t) {
-                            try {
-                                n = e.call(i, c)
-                            } catch (n) {
-                                return void o.error.call(i, n)
-                            }
-                            o.load.call(i, n)
-                        } else o.error.call(i, c)
-                    }
-                    return this.XDomainRequest && !("withCredentials" in c) && /^(http(s)?:)?\/\//.test(n) && (c = new XDomainRequest), "onload" in c ? c.onload = c.onerror = s : c.onreadystatechange = function() {
-                        c.readyState > 3 && s()
-                    }, c.onprogress = function(n) {
-                        var t = u.event;
-                        u.event = n;
-                        try {
-                            o.progress.call(i, c)
-                        } finally {
-                            u.event = t
-                        }
-                    }, i.header = function(n, t) {
-                        return n = (n + "").toLowerCase(), arguments.length < 2 ? l[n] : (null == t ? delete l[n] : l[n] = t + "", i)
-                    }, i.mimeType = function(n) {
-                        return arguments.length ? (t = null == n ? null : n + "", i) : t
-                    }, i.responseType = function(n) {
-                        return arguments.length ? (f = n, i) : f
-                    }, i.response = function(n) {
-                        return e = n, i
-                    }, ["get", "post"].forEach((function(n) {
-                        i[n] = function() {
-                            return i.send.apply(i, [n].concat(a(arguments)))
-                        }
-                    })), i.send = function(e, r, u) {
-                        if (2 === arguments.length && "function" == typeof r && (u = r, r = null), c.open(e, n, !0), null == t || "accept" in l || (l.accept = t + ",*/*"), c.setRequestHeader)
-                            for (var a in l) c.setRequestHeader(a, l[a]);
-                        return null != t && c.overrideMimeType && c.overrideMimeType(t), null != f && (c.responseType = f), null != u && i.on("error", u).on("load", (function(n) {
-                            u(null, n)
-                        })), o.beforesend.call(i, c), c.send(null == r ? null : r), i
-                    }, i.abort = function() {
-                        return c.abort(), i
-                    }, u.rebind(i, o, "on"), null == r ? i : i.get(function(n) {
-                        return 1 === n.length ? function(t, e) {
-                            n(null == t ? e : null)
-                        } : n
-                    }(r))
-                }
-                mt.forEach((function(n, t) {
-                    mt.set(n, ct(t))
-                })), u.functor = Mt, u.xhr = xt(R), u.dsv = function(n, t) {
-                    var e = new RegExp('["' + n + "\n]"),
-                        r = n.charCodeAt(0);
-
-                    function i(n, e, r) {
-                        arguments.length < 3 && (r = e, e = null);
-                        var i = bt(n, t, null == e ? u : o(e), r);
-                        return i.row = function(n) {
-                            return arguments.length ? i.response(null == (e = n) ? u : o(n)) : e
-                        }, i
-                    }
+    function Tt() {
+        var n = Date.now();
+        for (Ka = Ba; Ka;) n >= Ka.t && (Ka.f = Ka.c(n - Ka.t)), Ka = Ka.n;
+        return n
+    }
 
-                    function u(n) {
-                        return i.parse(n.responseText)
-                    }
+    function qt() {
+        for (var n, t = Ba, e = 1 / 0; t;) t.f ? t = n ? n.n = t.n : Ba = t.n : (t.t < e && (e = t.t), t = (n = t).n);
+        return Wa = n, e
+    }
 
-                    function o(n) {
-                        return function(t) {
-                            return i.parse(t.responseText, n)
-                        }
-                    }
+    function Rt(n, t) {
+        return t - (n ? Math.ceil(Math.log(n) / Math.LN10) : 1)
+    }
 
-                    function a(t) {
-                        return t.map(l).join(n)
-                    }
+    function Dt(n, t) {
+        var e = Math.pow(10, 3 * ca(8 - t));
+        return {
+            scale: t > 8 ? function(n) {
+                return n / e
+            } : function(n) {
+                return n * e
+            },
+            symbol: n
+        }
+    }
 
-                    function l(n) {
-                        return e.test(n) ? '"' + n.replace(/\"/g, '""') + '"' : n
-                    }
-                    return i.parse = function(n, t) {
-                        var e;
-                        return i.parseRows(n, (function(n, r) {
-                            if (e) return e(n, r - 1);
-                            var i = new Function("d", "return {" + n.map((function(n, t) {
-                                return JSON.stringify(n) + ": d[" + t + "]"
-                            })).join(",") + "}");
-                            e = t ? function(n, e) {
-                                return t(i(n), e)
-                            } : i
-                        }))
-                    }, i.parseRows = function(n, t) {
-                        var e, i, u = {},
-                            o = {},
-                            a = [],
-                            l = n.length,
-                            c = 0,
-                            f = 0;
-
-                        function s() {
-                            if (c >= l) return o;
-                            if (i) return i = !1, u;
-                            var t = c;
-                            if (34 === n.charCodeAt(t)) {
-                                for (var e = t; e++ < l;)
-                                    if (34 === n.charCodeAt(e)) {
-                                        if (34 !== n.charCodeAt(e + 1)) break;
-                                        ++e
-                                    } return c = e + 2, 13 === (a = n.charCodeAt(e + 1)) ? (i = !0, 10 === n.charCodeAt(e + 2) && ++c) : 10 === a && (i = !0), n.slice(t + 1, e).replace(/""/g, '"')
-                            }
-                            for (; c < l;) {
-                                var a, f = 1;
-                                if (10 === (a = n.charCodeAt(c++))) i = !0;
-                                else if (13 === a) i = !0, 10 === n.charCodeAt(c) && (++c, ++f);
-                                else if (a !== r) continue;
-                                return n.slice(t, c - f)
-                            }
-                            return n.slice(t)
-                        }
-                        for (;
-                            (e = s()) !== o;) {
-                            for (var h = []; e !== u && e !== o;) h.push(e), e = s();
-                            t && null == (h = t(h, f++)) || a.push(h)
-                        }
-                        return a
-                    }, i.format = function(t) {
-                        if (Array.isArray(t[0])) return i.formatRows(t);
-                        var e = new T,
-                            r = [];
-                        return t.forEach((function(n) {
-                            for (var t in n) e.has(t) || r.push(e.add(t))
-                        })), [r.map(l).join(n)].concat(t.map((function(t) {
-                            return r.map((function(n) {
-                                return l(t[n])
-                            })).join(n)
-                        }))).join("\n")
-                    }, i.formatRows = function(n) {
-                        return n.map(a).join("\n")
-                    }, i
-                }, u.csv = u.dsv(",", "text/csv"), u.tsv = u.dsv("\t", "text/tab-separated-values");
-                var wt, _t, kt, St, Nt = this[P(this, "requestAnimationFrame")] || function(n) {
-                    setTimeout(n, 17)
-                };
+    function Pt(n) {
+        var t = n.decimal,
+            e = n.thousands,
+            r = n.grouping,
+            u = n.currency,
+            i = r && e ? function(n, t) {
+                for (var u = n.length, i = [], o = 0, a = r[0], c = 0; u > 0 && a > 0 && (c + a + 1 > t && (a = Math.max(1, t - c)), i.push(n.substring(u -= a, u + a)), !((c += a + 1) > t));) a = r[o = (o + 1) % r.length];
+                return i.reverse().join(e)
+            } : Et;
+        return function(n) {
+            var e = tc.exec(n),
+                r = e[1] || " ",
+                o = e[2] || ">",
+                a = e[3] || "-",
+                c = e[4] || "",
+                l = e[5],
+                s = +e[6],
+                f = e[7],
+                h = e[8],
+                g = e[9],
+                p = 1,
+                v = "",
+                d = "",
+                m = !1,
+                y = !0;
+            switch (h && (h = +h.substring(1)), (l || "0" === r && "=" === o) && (l = r = "0", o = "="), g) {
+                case "n":
+                    f = !0, g = "g";
+                    break;
+                case "%":
+                    p = 100, d = "%", g = "f";
+                    break;
+                case "p":
+                    p = 100, d = "%", g = "r";
+                    break;
+                case "b":
+                case "o":
+                case "x":
+                case "X":
+                    "#" === c && (v = "0" + g.toLowerCase());
+                case "c":
+                    y = !1;
+                case "d":
+                    m = !0, h = 0;
+                    break;
+                case "s":
+                    p = -1, g = "r"
+            }
+            "$" === c && (v = u[0], d = u[1]), "r" != g || h || (g = "g"), null != h && ("g" == g ? h = Math.max(1, Math.min(21, h)) : ("e" == g || "f" == g) && (h = Math.max(0, Math.min(20, h)))), g = ec.get(g) || Ut;
+            var x = l && f;
+            return function(n) {
+                var e = d;
+                if (m && n % 1) return "";
+                var u = 0 > n || 0 === n && 0 > 1 / n ? (n = -n, "-") : "-" === a ? "" : a;
+                if (0 > p) {
+                    var c = Bo.formatPrefix(n, h);
+                    n = c.scale(n), e = c.symbol + d
+                } else n *= p;
+                n = g(n, h);
+                var M, _, b = n.lastIndexOf(".");
+                if (0 > b) {
+                    var w = y ? n.lastIndexOf("e") : -1;
+                    0 > w ? (M = n, _ = "") : (M = n.substring(0, w), _ = n.substring(w))
+                } else M = n.substring(0, b), _ = t + n.substring(b + 1);
+                !l && f && (M = i(M, 1 / 0));
+                var S = v.length + M.length + _.length + (x ? 0 : u.length),
+                    k = s > S ? new Array(S = s - S + 1).join(r) : "";
+                return x && (M = i(k + M, k.length ? s - _.length : 1 / 0)), u += v, n = M + _, ("<" === o ? u + n + k : ">" === o ? k + u + n : "^" === o ? k.substring(0, S >>= 1) + u + n + k.substring(S) : u + (x ? n : k + n)) + e
+            }
+        }
+    }
 
-                function Et(n, t, e) {
-                    var r = arguments.length;
-                    r < 2 && (t = 0), r < 3 && (e = Date.now());
-                    var i = e + t,
-                        u = {
-                            c: n,
-                            t: i,
-                            n: null
-                        };
-                    return _t ? _t.n = u : wt = u, _t = u, kt || (St = clearTimeout(St), kt = 1, Nt(At)), u
-                }
-
-                function At() {
-                    var n = Ct(),
-                        t = zt() - n;
-                    t > 24 ? (isFinite(t) && (clearTimeout(St), St = setTimeout(At, t)), kt = 0) : (kt = 1, Nt(At))
-                }
-
-                function Ct() {
-                    for (var n = Date.now(), t = wt; t;) n >= t.t && t.c(n - t.t) && (t.c = null), t = t.n;
-                    return n
-                }
-
-                function zt() {
-                    for (var n, t = wt, e = 1 / 0; t;) t.c ? (t.t < e && (e = t.t), t = (n = t).n) : t = n ? n.n = t.n : wt = t.n;
-                    return _t = n, e
-                }
-
-                function Lt(n, t) {
-                    return t - (n ? Math.ceil(Math.log(n) / Math.LN10) : 1)
-                }
-                u.timer = function() {
-                    Et.apply(this, arguments)
-                }, u.timer.flush = function() {
-                    Ct(), zt()
-                }, u.round = function(n, t) {
-                    return t ? Math.round(n * (t = Math.pow(10, t))) / t : Math.round(n)
-                };
-                var qt = ["y", "z", "a", "f", "p", "n", "µ", "m", "", "k", "M", "G", "T", "P", "E", "Z", "Y"].map((function(n, t) {
-                    var e = Math.pow(10, 3 * w(8 - t));
-                    return {
-                        scale: t > 8 ? function(n) {
-                            return n / e
-                        } : function(n) {
-                            return n * e
-                        },
-                        symbol: n
-                    }
-                }));
+    function Ut(n) {
+        return n + ""
+    }
 
-                function Tt(n) {
-                    var t = n.decimal,
-                        e = n.thousands,
-                        r = n.grouping,
-                        i = n.currency,
-                        o = r && e ? function(n, t) {
-                            for (var i = n.length, u = [], o = 0, a = r[0], l = 0; i > 0 && a > 0 && (l + a + 1 > t && (a = Math.max(1, t - l)), u.push(n.substring(i -= a, i + a)), !((l += a + 1) > t));) a = r[o = (o + 1) % r.length];
-                            return u.reverse().join(e)
-                        } : R;
-                    return function(n) {
-                        var e = Rt.exec(n),
-                            r = e[1] || " ",
-                            a = e[2] || ">",
-                            l = e[3] || "-",
-                            c = e[4] || "",
-                            f = e[5],
-                            s = +e[6],
-                            h = e[7],
-                            p = e[8],
-                            g = e[9],
-                            v = 1,
-                            d = "",
-                            y = "",
-                            m = !1,
-                            M = !0;
-                        switch (p && (p = +p.substring(1)), (f || "0" === r && "=" === a) && (f = r = "0", a = "="), g) {
-                            case "n":
-                                h = !0, g = "g";
-                                break;
-                            case "%":
-                                v = 100, y = "%", g = "f";
-                                break;
-                            case "p":
-                                v = 100, y = "%", g = "r";
-                                break;
-                            case "b":
-                            case "o":
-                            case "x":
-                            case "X":
-                                "#" === c && (d = "0" + g.toLowerCase());
-                            case "c":
-                                M = !1;
-                            case "d":
-                                m = !0, p = 0;
-                                break;
-                            case "s":
-                                v = -1, g = "r"
-                        }
-                        "$" === c && (d = i[0], y = i[1]), "r" != g || p || (g = "g"), null != p && ("g" == g ? p = Math.max(1, Math.min(21, p)) : "e" != g && "f" != g || (p = Math.max(0, Math.min(20, p)))), g = Dt.get(g) || Pt;
-                        var x = f && h;
-                        return function(n) {
-                            var e = y;
-                            if (m && n % 1) return "";
-                            var i = n < 0 || 0 === n && 1 / n < 0 ? (n = -n, "-") : "-" === l ? "" : l;
-                            if (v < 0) {
-                                var c = u.formatPrefix(n, p);
-                                n = c.scale(n), e = c.symbol + y
-                            } else n *= v;
-                            var b, w, _ = (n = g(n, p)).lastIndexOf(".");
-                            if (_ < 0) {
-                                var k = M ? n.lastIndexOf("e") : -1;
-                                k < 0 ? (b = n, w = "") : (b = n.substring(0, k), w = n.substring(k))
-                            } else b = n.substring(0, _), w = t + n.substring(_ + 1);
-                            !f && h && (b = o(b, 1 / 0));
-                            var S = d.length + b.length + w.length + (x ? 0 : i.length),
-                                N = S < s ? new Array(S = s - S + 1).join(r) : "";
-                            return x && (b = o(N + b, N.length ? s - w.length : 1 / 0)), i += d, n = b + w, ("<" === a ? i + n + N : ">" === a ? N + i + n : "^" === a ? N.substring(0, S >>= 1) + i + n + N.substring(S) : i + (x ? n : N + n)) + e
-                        }
-                    }
-                }
-                u.formatPrefix = function(n, t) {
-                    var e = 0;
-                    return (n = +n) && (n < 0 && (n *= -1), t && (n = u.round(n, Lt(n, t))), e = 1 + Math.floor(1e-12 + Math.log(n) / Math.LN10), e = Math.max(-24, Math.min(24, 3 * Math.floor((e - 1) / 3)))), qt[8 + e / 3]
-                };
-                var Rt = /(?:([^{])?([<>=^]))?([+\- ])?([$#])?(0)?(\d+)?(,)?(\.-?\d+)?([a-z%])?/i,
-                    Dt = u.map({
-                        b: function(n) {
-                            return n.toString(2)
-                        },
-                        c: function(n) {
-                            return String.fromCharCode(n)
-                        },
-                        o: function(n) {
-                            return n.toString(8)
-                        },
-                        x: function(n) {
-                            return n.toString(16)
-                        },
-                        X: function(n) {
-                            return n.toString(16).toUpperCase()
-                        },
-                        g: function(n, t) {
-                            return n.toPrecision(t)
-                        },
-                        e: function(n, t) {
-                            return n.toExponential(t)
-                        },
-                        f: function(n, t) {
-                            return n.toFixed(t)
-                        },
-                        r: function(n, t) {
-                            return (n = u.round(n, Lt(n, t))).toFixed(Math.max(0, Math.min(20, Lt(n * (1 + 1e-15), t))))
-                        }
-                    });
+    function jt() {
+        this._ = new Date(arguments.length > 1 ? Date.UTC.apply(this, arguments) : arguments[0])
+    }
 
-                function Pt(n) {
-                    return n + ""
-                }
-                var Ut = u.time = {},
-                    jt = Date;
+    function Ft(n, t, e) {
+        function r(t) {
+            var e = n(t),
+                r = i(e, 1);
+            return r - t > t - e ? e : r
+        }
 
-                function Ft() {
-                    this._ = new Date(arguments.length > 1 ? Date.UTC.apply(this, arguments) : arguments[0])
-                }
-                Ft.prototype = {
-                    getDate: function() {
-                        return this._.getUTCDate()
-                    },
-                    getDay: function() {
-                        return this._.getUTCDay()
-                    },
-                    getFullYear: function() {
-                        return this._.getUTCFullYear()
-                    },
-                    getHours: function() {
-                        return this._.getUTCHours()
-                    },
-                    getMilliseconds: function() {
-                        return this._.getUTCMilliseconds()
-                    },
-                    getMinutes: function() {
-                        return this._.getUTCMinutes()
-                    },
-                    getMonth: function() {
-                        return this._.getUTCMonth()
-                    },
-                    getSeconds: function() {
-                        return this._.getUTCSeconds()
-                    },
-                    getTime: function() {
-                        return this._.getTime()
-                    },
-                    getTimezoneOffset: function() {
-                        return 0
-                    },
-                    valueOf: function() {
-                        return this._.valueOf()
-                    },
-                    setDate: function() {
-                        Ht.setUTCDate.apply(this._, arguments)
-                    },
-                    setDay: function() {
-                        Ht.setUTCDay.apply(this._, arguments)
-                    },
-                    setFullYear: function() {
-                        Ht.setUTCFullYear.apply(this._, arguments)
-                    },
-                    setHours: function() {
-                        Ht.setUTCHours.apply(this._, arguments)
-                    },
-                    setMilliseconds: function() {
-                        Ht.setUTCMilliseconds.apply(this._, arguments)
-                    },
-                    setMinutes: function() {
-                        Ht.setUTCMinutes.apply(this._, arguments)
-                    },
-                    setMonth: function() {
-                        Ht.setUTCMonth.apply(this._, arguments)
-                    },
-                    setSeconds: function() {
-                        Ht.setUTCSeconds.apply(this._, arguments)
-                    },
-                    setTime: function() {
-                        Ht.setTime.apply(this._, arguments)
-                    }
-                };
-                var Ht = Date.prototype;
+        function u(e) {
+            return t(e = n(new uc(e - 1)), 1), e
+        }
 
-                function Ot(n, t, e) {
-                    function r(t) {
-                        var e = n(t),
-                            r = u(e, 1);
-                        return t - e < r - t ? e : r
-                    }
+        function i(n, e) {
+            return t(n = new uc(+n), e), n
+        }
 
-                    function i(e) {
-                        return t(e = n(new jt(e - 1)), 1), e
-                    }
+        function o(n, r, i) {
+            var o = u(n),
+                a = [];
+            if (i > 1)
+                for (; r > o;) e(o) % i || a.push(new Date(+o)), t(o, 1);
+            else
+                for (; r > o;) a.push(new Date(+o)), t(o, 1);
+            return a
+        }
 
-                    function u(n, e) {
-                        return t(n = new jt(+n), e), n
-                    }
+        function a(n, t, e) {
+            try {
+                uc = jt;
+                var r = new jt;
+                return r._ = n, o(r, t, e)
+            } finally {
+                uc = Date
+            }
+        }
+        n.floor = n, n.round = r, n.ceil = u, n.offset = i, n.range = o;
+        var c = n.utc = Ht(n);
+        return c.floor = c, c.round = Ht(r), c.ceil = Ht(u), c.offset = Ht(i), c.range = a, n
+    }
 
-                    function o(n, r, u) {
-                        var o = i(n),
-                            a = [];
-                        if (u > 1)
-                            for (; o < r;) e(o) % u || a.push(new Date(+o)), t(o, 1);
-                        else
-                            for (; o < r;) a.push(new Date(+o)), t(o, 1);
-                        return a
-                    }
-                    n.floor = n, n.round = r, n.ceil = i, n.offset = u, n.range = o;
-                    var a = n.utc = It(n);
-                    return a.floor = a, a.round = It(r), a.ceil = It(i), a.offset = It(u), a.range = function(n, t, e) {
-                        try {
-                            jt = Ft;
-                            var r = new Ft;
-                            return r._ = n, o(r, t, e)
-                        } finally {
-                            jt = Date
-                        }
-                    }, n
-                }
+    function Ht(n) {
+        return function(t, e) {
+            try {
+                uc = jt;
+                var r = new jt;
+                return r._ = t, n(r, e)._
+            } finally {
+                uc = Date
+            }
+        }
+    }
 
-                function It(n) {
-                    return function(t, e) {
-                        try {
-                            jt = Ft;
-                            var r = new Ft;
-                            return r._ = t, n(r, e)._
-                        } finally {
-                            jt = Date
-                        }
-                    }
-                }
+    function Ot(n) {
+        function t(n) {
+            function t(t) {
+                for (var e, u, i, o = [], a = -1, c = 0; ++a < r;) 37 === n.charCodeAt(a) && (o.push(n.slice(c, a)), null != (u = oc[e = n.charAt(++a)]) && (e = n.charAt(++a)), (i = C[e]) && (e = i(t, null == u ? "e" === e ? " " : "0" : u)), o.push(e), c = a + 1);
+                return o.push(n.slice(c, a)), o.join("")
+            }
+            var r = n.length;
+            return t.parse = function(t) {
+                var r = {
+                        y: 1900,
+                        m: 0,
+                        d: 1,
+                        H: 0,
+                        M: 0,
+                        S: 0,
+                        L: 0,
+                        Z: null
+                    },
+                    u = e(r, n, t, 0);
+                if (u != t.length) return null;
+                "p" in r && (r.H = r.H % 12 + 12 * r.p);
+                var i = null != r.Z && uc !== jt,
+                    o = new(i ? jt : uc);
+                return "j" in r ? o.setFullYear(r.y, 0, r.j) : "w" in r && ("W" in r || "U" in r) ? (o.setFullYear(r.y, 0, 1), o.setFullYear(r.y, 0, "W" in r ? (r.w + 6) % 7 + 7 * r.W - (o.getDay() + 5) % 7 : r.w + 7 * r.U - (o.getDay() + 6) % 7)) : o.setFullYear(r.y, r.m, r.d), o.setHours(r.H + (0 | r.Z / 100), r.M + r.Z % 100, r.S, r.L), i ? o._ : o
+            }, t.toString = function() {
+                return n
+            }, t
+        }
 
-                function Yt(n) {
-                    var t = n.dateTime,
-                        e = n.date,
-                        r = n.time,
-                        i = n.periods,
-                        o = n.days,
-                        a = n.shortDays,
-                        l = n.months,
-                        c = n.shortMonths;
-
-                    function f(n) {
-                        var t = n.length;
-
-                        function e(e) {
-                            for (var r, i, u, o = [], a = -1, l = 0; ++a < t;) 37 === n.charCodeAt(a) && (o.push(n.slice(l, a)), null != (i = Zt[r = n.charAt(++a)]) && (r = n.charAt(++a)), (u = b[r]) && (r = u(e, null == i ? "e" === r ? " " : "0" : i)), o.push(r), l = a + 1);
-                            return o.push(n.slice(l, a)), o.join("")
-                        }
-                        return e.parse = function(t) {
-                            var e = {
-                                y: 1900,
-                                m: 0,
-                                d: 1,
-                                H: 0,
-                                M: 0,
-                                S: 0,
-                                L: 0,
-                                Z: null
-                            };
-                            if (s(e, n, t, 0) != t.length) return null;
-                            "p" in e && (e.H = e.H % 12 + 12 * e.p);
-                            var r = null != e.Z && jt !== Ft,
-                                i = new(r ? Ft : jt);
-                            return "j" in e ? i.setFullYear(e.y, 0, e.j) : "W" in e || "U" in e ? ("w" in e || (e.w = "W" in e ? 1 : 0), i.setFullYear(e.y, 0, 1), i.setFullYear(e.y, 0, "W" in e ? (e.w + 6) % 7 + 7 * e.W - (i.getDay() + 5) % 7 : e.w + 7 * e.U - (i.getDay() + 6) % 7)) : i.setFullYear(e.y, e.m, e.d), i.setHours(e.H + (e.Z / 100 | 0), e.M + e.Z % 100, e.S, e.L), r ? i._ : i
-                        }, e.toString = function() {
-                            return n
-                        }, e
-                    }
+        function e(n, t, e, r) {
+            for (var u, i, o, a = 0, c = t.length, l = e.length; c > a;) {
+                if (r >= l) return -1;
+                if (u = t.charCodeAt(a++), 37 === u) {
+                    if (o = t.charAt(a++), i = N[o in oc ? t.charAt(a++) : o], !i || (r = i(n, e, r)) < 0) return -1
+                } else if (u != e.charCodeAt(r++)) return -1
+            }
+            return r
+        }
 
-                    function s(n, t, e, r) {
-                        for (var i, u, o, a = 0, l = t.length, c = e.length; a < l;) {
-                            if (r >= c) return -1;
-                            if (37 === (i = t.charCodeAt(a++))) {
-                                if (o = t.charAt(a++), !(u = w[o in Zt ? t.charAt(a++) : o]) || (r = u(n, e, r)) < 0) return -1
-                            } else if (i != e.charCodeAt(r++)) return -1
-                        }
-                        return r
-                    }
-                    f.utc = function(n) {
-                        var t = f(n);
+        function r(n, t, e) {
+            b.lastIndex = 0;
+            var r = b.exec(t.slice(e));
+            return r ? (n.w = w.get(r[0].toLowerCase()), e + r[0].length) : -1
+        }
 
-                        function e(n) {
-                            try {
-                                var e = new(jt = Ft);
-                                return e._ = n, t(e)
-                            } finally {
-                                jt = Date
-                            }
-                        }
-                        return e.parse = function(n) {
-                            try {
-                                jt = Ft;
-                                var e = t.parse(n);
-                                return e && e._
-                            } finally {
-                                jt = Date
-                            }
-                        }, e.toString = t.toString, e
-                    }, f.multi = f.utc.multi = se;
-                    var h = u.map(),
-                        p = Bt(o),
-                        g = Jt(o),
-                        v = Bt(a),
-                        d = Jt(a),
-                        y = Bt(l),
-                        m = Jt(l),
-                        M = Bt(c),
-                        x = Jt(c);
-                    i.forEach((function(n, t) {
-                        h.set(n.toLowerCase(), t)
-                    }));
-                    var b = {
-                            a: function(n) {
-                                return a[n.getDay()]
-                            },
-                            A: function(n) {
-                                return o[n.getDay()]
-                            },
-                            b: function(n) {
-                                return c[n.getMonth()]
-                            },
-                            B: function(n) {
-                                return l[n.getMonth()]
-                            },
-                            c: f(t),
-                            d: function(n, t) {
-                                return $t(n.getDate(), t, 2)
-                            },
-                            e: function(n, t) {
-                                return $t(n.getDate(), t, 2)
-                            },
-                            H: function(n, t) {
-                                return $t(n.getHours(), t, 2)
-                            },
-                            I: function(n, t) {
-                                return $t(n.getHours() % 12 || 12, t, 2)
-                            },
-                            j: function(n, t) {
-                                return $t(1 + Ut.dayOfYear(n), t, 3)
-                            },
-                            L: function(n, t) {
-                                return $t(n.getMilliseconds(), t, 3)
-                            },
-                            m: function(n, t) {
-                                return $t(n.getMonth() + 1, t, 2)
-                            },
-                            M: function(n, t) {
-                                return $t(n.getMinutes(), t, 2)
-                            },
-                            p: function(n) {
-                                return i[+(n.getHours() >= 12)]
-                            },
-                            S: function(n, t) {
-                                return $t(n.getSeconds(), t, 2)
-                            },
-                            U: function(n, t) {
-                                return $t(Ut.sundayOfYear(n), t, 2)
-                            },
-                            w: function(n) {
-                                return n.getDay()
-                            },
-                            W: function(n, t) {
-                                return $t(Ut.mondayOfYear(n), t, 2)
-                            },
-                            x: f(e),
-                            X: f(r),
-                            y: function(n, t) {
-                                return $t(n.getFullYear() % 100, t, 2)
-                            },
-                            Y: function(n, t) {
-                                return $t(n.getFullYear() % 1e4, t, 4)
-                            },
-                            Z: ce,
-                            "%": function() {
-                                return "%"
-                            }
-                        },
-                        w = {
-                            a: function(n, t, e) {
-                                v.lastIndex = 0;
-                                var r = v.exec(t.slice(e));
-                                return r ? (n.w = d.get(r[0].toLowerCase()), e + r[0].length) : -1
-                            },
-                            A: function(n, t, e) {
-                                p.lastIndex = 0;
-                                var r = p.exec(t.slice(e));
-                                return r ? (n.w = g.get(r[0].toLowerCase()), e + r[0].length) : -1
-                            },
-                            b: function(n, t, e) {
-                                M.lastIndex = 0;
-                                var r = M.exec(t.slice(e));
-                                return r ? (n.m = x.get(r[0].toLowerCase()), e + r[0].length) : -1
-                            },
-                            B: function(n, t, e) {
-                                y.lastIndex = 0;
-                                var r = y.exec(t.slice(e));
-                                return r ? (n.m = m.get(r[0].toLowerCase()), e + r[0].length) : -1
-                            },
-                            c: function(n, t, e) {
-                                return s(n, b.c.toString(), t, e)
-                            },
-                            d: re,
-                            e: re,
-                            H: ue,
-                            I: ue,
-                            j: ie,
-                            L: le,
-                            m: ee,
-                            M: oe,
-                            p: function(n, t, e) {
-                                var r = h.get(t.slice(e, e += 2).toLowerCase());
-                                return null == r ? -1 : (n.p = r, e)
-                            },
-                            S: ae,
-                            U: Gt,
-                            w: Wt,
-                            W: Kt,
-                            x: function(n, t, e) {
-                                return s(n, b.x.toString(), t, e)
-                            },
-                            X: function(n, t, e) {
-                                return s(n, b.X.toString(), t, e)
-                            },
-                            y: ne,
-                            Y: Qt,
-                            Z: te,
-                            "%": fe
-                        };
-                    return f
-                }
-                Ut.year = Ot((function(n) {
-                    return (n = Ut.day(n)).setMonth(0, 1), n
-                }), (function(n, t) {
-                    n.setFullYear(n.getFullYear() + t)
-                }), (function(n) {
-                    return n.getFullYear()
-                })), Ut.years = Ut.year.range, Ut.years.utc = Ut.year.utc.range, Ut.day = Ot((function(n) {
-                    var t = new jt(2e3, 0);
-                    return t.setFullYear(n.getFullYear(), n.getMonth(), n.getDate()), t
-                }), (function(n, t) {
-                    n.setDate(n.getDate() + t)
-                }), (function(n) {
-                    return n.getDate() - 1
-                })), Ut.days = Ut.day.range, Ut.days.utc = Ut.day.utc.range, Ut.dayOfYear = function(n) {
-                    var t = Ut.year(n);
-                    return Math.floor((n - t - 6e4 * (n.getTimezoneOffset() - t.getTimezoneOffset())) / 864e5)
-                }, ["sunday", "monday", "tuesday", "wednesday", "thursday", "friday", "saturday"].forEach((function(n, t) {
-                    t = 7 - t;
-                    var e = Ut[n] = Ot((function(n) {
-                        return (n = Ut.day(n)).setDate(n.getDate() - (n.getDay() + t) % 7), n
-                    }), (function(n, t) {
-                        n.setDate(n.getDate() + 7 * Math.floor(t))
-                    }), (function(n) {
-                        var e = Ut.year(n).getDay();
-                        return Math.floor((Ut.dayOfYear(n) + (e + t) % 7) / 7) - (e !== t)
-                    }));
-                    Ut[n + "s"] = e.range, Ut[n + "s"].utc = e.utc.range, Ut[n + "OfYear"] = function(n) {
-                        var e = Ut.year(n).getDay();
-                        return Math.floor((Ut.dayOfYear(n) + (e + t) % 7) / 7)
-                    }
-                })), Ut.week = Ut.sunday, Ut.weeks = Ut.sunday.range, Ut.weeks.utc = Ut.sunday.utc.range, Ut.weekOfYear = Ut.sundayOfYear;
-                var Zt = {
-                        "-": "",
-                        _: " ",
-                        0: "0"
-                    },
-                    Vt = /^\s*\d+/,
-                    Xt = /^%/;
+        function u(n, t, e) {
+            M.lastIndex = 0;
+            var r = M.exec(t.slice(e));
+            return r ? (n.w = _.get(r[0].toLowerCase()), e + r[0].length) : -1
+        }
 
-                function $t(n, t, e) {
-                    var r = n < 0 ? "-" : "",
-                        i = (r ? -n : n) + "",
-                        u = i.length;
-                    return r + (u < e ? new Array(e - u + 1).join(t) + i : i)
-                }
+        function i(n, t, e) {
+            E.lastIndex = 0;
+            var r = E.exec(t.slice(e));
+            return r ? (n.m = A.get(r[0].toLowerCase()), e + r[0].length) : -1
+        }
 
-                function Bt(n) {
-                    return new RegExp("^(?:" + n.map(u.requote).join("|") + ")", "i")
-                }
+        function o(n, t, e) {
+            S.lastIndex = 0;
+            var r = S.exec(t.slice(e));
+            return r ? (n.m = k.get(r[0].toLowerCase()), e + r[0].length) : -1
+        }
 
-                function Jt(n) {
-                    for (var t = new S, e = -1, r = n.length; ++e < r;) t.set(n[e].toLowerCase(), e);
-                    return t
-                }
+        function a(n, t, r) {
+            return e(n, C.c.toString(), t, r)
+        }
 
-                function Wt(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r = Vt.exec(t.slice(e, e + 1));
-                    return r ? (n.w = +r[0], e + r[0].length) : -1
-                }
+        function c(n, t, r) {
+            return e(n, C.x.toString(), t, r)
+        }
 
-                function Gt(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r = Vt.exec(t.slice(e));
-                    return r ? (n.U = +r[0], e + r[0].length) : -1
-                }
+        function l(n, t, r) {
+            return e(n, C.X.toString(), t, r)
+        }
 
-                function Kt(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r = Vt.exec(t.slice(e));
-                    return r ? (n.W = +r[0], e + r[0].length) : -1
-                }
+        function s(n, t, e) {
+            var r = x.get(t.slice(e, e += 2).toLowerCase());
+            return null == r ? -1 : (n.p = r, e)
+        }
+        var f = n.dateTime,
+            h = n.date,
+            g = n.time,
+            p = n.periods,
+            v = n.days,
+            d = n.shortDays,
+            m = n.months,
+            y = n.shortMonths;
+        t.utc = function(n) {
+            function e(n) {
+                try {
+                    uc = jt;
+                    var t = new uc;
+                    return t._ = n, r(t)
+                } finally {
+                    uc = Date
+                }
+            }
+            var r = t(n);
+            return e.parse = function(n) {
+                try {
+                    uc = jt;
+                    var t = r.parse(n);
+                    return t && t._
+                } finally {
+                    uc = Date
+                }
+            }, e.toString = r.toString, e
+        }, t.multi = t.utc.multi = ae;
+        var x = Bo.map(),
+            M = It(v),
+            _ = Zt(v),
+            b = It(d),
+            w = Zt(d),
+            S = It(m),
+            k = Zt(m),
+            E = It(y),
+            A = Zt(y);
+        p.forEach(function(n, t) {
+            x.set(n.toLowerCase(), t)
+        });
+        var C = {
+                a: function(n) {
+                    return d[n.getDay()]
+                },
+                A: function(n) {
+                    return v[n.getDay()]
+                },
+                b: function(n) {
+                    return y[n.getMonth()]
+                },
+                B: function(n) {
+                    return m[n.getMonth()]
+                },
+                c: t(f),
+                d: function(n, t) {
+                    return Yt(n.getDate(), t, 2)
+                },
+                e: function(n, t) {
+                    return Yt(n.getDate(), t, 2)
+                },
+                H: function(n, t) {
+                    return Yt(n.getHours(), t, 2)
+                },
+                I: function(n, t) {
+                    return Yt(n.getHours() % 12 || 12, t, 2)
+                },
+                j: function(n, t) {
+                    return Yt(1 + rc.dayOfYear(n), t, 3)
+                },
+                L: function(n, t) {
+                    return Yt(n.getMilliseconds(), t, 3)
+                },
+                m: function(n, t) {
+                    return Yt(n.getMonth() + 1, t, 2)
+                },
+                M: function(n, t) {
+                    return Yt(n.getMinutes(), t, 2)
+                },
+                p: function(n) {
+                    return p[+(n.getHours() >= 12)]
+                },
+                S: function(n, t) {
+                    return Yt(n.getSeconds(), t, 2)
+                },
+                U: function(n, t) {
+                    return Yt(rc.sundayOfYear(n), t, 2)
+                },
+                w: function(n) {
+                    return n.getDay()
+                },
+                W: function(n, t) {
+                    return Yt(rc.mondayOfYear(n), t, 2)
+                },
+                x: t(h),
+                X: t(g),
+                y: function(n, t) {
+                    return Yt(n.getFullYear() % 100, t, 2)
+                },
+                Y: function(n, t) {
+                    return Yt(n.getFullYear() % 1e4, t, 4)
+                },
+                Z: ie,
+                "%": function() {
+                    return "%"
+                }
+            },
+            N = {
+                a: r,
+                A: u,
+                b: i,
+                B: o,
+                c: a,
+                d: Qt,
+                e: Qt,
+                H: te,
+                I: te,
+                j: ne,
+                L: ue,
+                m: Kt,
+                M: ee,
+                p: s,
+                S: re,
+                U: Xt,
+                w: Vt,
+                W: $t,
+                x: c,
+                X: l,
+                y: Wt,
+                Y: Bt,
+                Z: Jt,
+                "%": oe
+            };
+        return t
+    }
 
-                function Qt(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r = Vt.exec(t.slice(e, e + 4));
-                    return r ? (n.y = +r[0], e + r[0].length) : -1
-                }
+    function Yt(n, t, e) {
+        var r = 0 > n ? "-" : "",
+            u = (r ? -n : n) + "",
+            i = u.length;
+        return r + (e > i ? new Array(e - i + 1).join(t) + u : u)
+    }
 
-                function ne(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r, i = Vt.exec(t.slice(e, e + 2));
-                    return i ? (n.y = (r = +i[0]) + (r > 68 ? 1900 : 2e3), e + i[0].length) : -1
-                }
+    function It(n) {
+        return new RegExp("^(?:" + n.map(Bo.requote).join("|") + ")", "i")
+    }
 
-                function te(n, t, e) {
-                    return /^[+-]\d{4}$/.test(t = t.slice(e, e + 5)) ? (n.Z = -t, e + 5) : -1
-                }
+    function Zt(n) {
+        for (var t = new a, e = -1, r = n.length; ++e < r;) t.set(n[e].toLowerCase(), e);
+        return t
+    }
 
-                function ee(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r = Vt.exec(t.slice(e, e + 2));
-                    return r ? (n.m = r[0] - 1, e + r[0].length) : -1
-                }
+    function Vt(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e, e + 1));
+        return r ? (n.w = +r[0], e + r[0].length) : -1
+    }
 
-                function re(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r = Vt.exec(t.slice(e, e + 2));
-                    return r ? (n.d = +r[0], e + r[0].length) : -1
-                }
+    function Xt(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e));
+        return r ? (n.U = +r[0], e + r[0].length) : -1
+    }
 
-                function ie(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r = Vt.exec(t.slice(e, e + 3));
-                    return r ? (n.j = +r[0], e + r[0].length) : -1
-                }
+    function $t(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e));
+        return r ? (n.W = +r[0], e + r[0].length) : -1
+    }
 
-                function ue(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r = Vt.exec(t.slice(e, e + 2));
-                    return r ? (n.H = +r[0], e + r[0].length) : -1
-                }
+    function Bt(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e, e + 4));
+        return r ? (n.y = +r[0], e + r[0].length) : -1
+    }
 
-                function oe(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r = Vt.exec(t.slice(e, e + 2));
-                    return r ? (n.M = +r[0], e + r[0].length) : -1
-                }
+    function Wt(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e, e + 2));
+        return r ? (n.y = Gt(+r[0]), e + r[0].length) : -1
+    }
 
-                function ae(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r = Vt.exec(t.slice(e, e + 2));
-                    return r ? (n.S = +r[0], e + r[0].length) : -1
-                }
+    function Jt(n, t, e) {
+        return /^[+-]\d{4}$/.test(t = t.slice(e, e + 5)) ? (n.Z = -t, e + 5) : -1
+    }
 
-                function le(n, t, e) {
-                    Vt.lastIndex = 0;
-                    var r = Vt.exec(t.slice(e, e + 3));
-                    return r ? (n.L = +r[0], e + r[0].length) : -1
-                }
+    function Gt(n) {
+        return n + (n > 68 ? 1900 : 2e3)
+    }
 
-                function ce(n) {
-                    var t = n.getTimezoneOffset(),
-                        e = t > 0 ? "-" : "+",
-                        r = w(t) / 60 | 0,
-                        i = w(t) % 60;
-                    return e + $t(r, "0", 2) + $t(i, "0", 2)
-                }
+    function Kt(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e, e + 2));
+        return r ? (n.m = r[0] - 1, e + r[0].length) : -1
+    }
 
-                function fe(n, t, e) {
-                    Xt.lastIndex = 0;
-                    var r = Xt.exec(t.slice(e, e + 1));
-                    return r ? e + r[0].length : -1
-                }
+    function Qt(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e, e + 2));
+        return r ? (n.d = +r[0], e + r[0].length) : -1
+    }
 
-                function se(n) {
-                    for (var t = n.length, e = -1; ++e < t;) n[e][0] = this(n[e][0]);
-                    return function(t) {
-                        for (var e = 0, r = n[e]; !r[1](t);) r = n[++e];
-                        return r[0](t)
-                    }
-                }
-                u.locale = function(n) {
-                    return {
-                        numberFormat: Tt(n),
-                        timeFormat: Yt(n)
-                    }
-                };
-                var he = u.locale({
-                    decimal: ".",
-                    thousands: ",",
-                    grouping: [3],
-                    currency: ["$", ""],
-                    dateTime: "%a %b %e %X %Y",
-                    date: "%m/%d/%Y",
-                    time: "%H:%M:%S",
-                    periods: ["AM", "PM"],
-                    days: ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"],
-                    shortDays: ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
-                    months: ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"],
-                    shortMonths: ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"]
-                });
+    function ne(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e, e + 3));
+        return r ? (n.j = +r[0], e + r[0].length) : -1
+    }
 
-                function pe() {}
-                u.format = he.numberFormat, u.geo = {}, pe.prototype = {
-                    s: 0,
-                    t: 0,
-                    add: function(n) {
-                        ve(n, this.t, ge), ve(ge.s, this.s, this), this.s ? this.t += ge.t : this.s = ge.t
-                    },
-                    reset: function() {
-                        this.s = this.t = 0
-                    },
-                    valueOf: function() {
-                        return this.s
-                    }
-                };
-                var ge = new pe;
+    function te(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e, e + 2));
+        return r ? (n.H = +r[0], e + r[0].length) : -1
+    }
 
-                function ve(n, t, e) {
-                    var r = e.s = n + t,
-                        i = r - n,
-                        u = r - i;
-                    e.t = n - u + (t - i)
-                }
+    function ee(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e, e + 2));
+        return r ? (n.M = +r[0], e + r[0].length) : -1
+    }
 
-                function de(n, t) {
-                    n && me.hasOwnProperty(n.type) && me[n.type](n, t)
-                }
-                u.geo.stream = function(n, t) {
-                    n && ye.hasOwnProperty(n.type) ? ye[n.type](n, t) : de(n, t)
-                };
-                var ye = {
-                        Feature: function(n, t) {
-                            de(n.geometry, t)
-                        },
-                        FeatureCollection: function(n, t) {
-                            for (var e = n.features, r = -1, i = e.length; ++r < i;) de(e[r].geometry, t)
-                        }
-                    },
-                    me = {
-                        Sphere: function(n, t) {
-                            t.sphere()
-                        },
-                        Point: function(n, t) {
-                            n = n.coordinates, t.point(n[0], n[1], n[2])
-                        },
-                        MultiPoint: function(n, t) {
-                            for (var e = n.coordinates, r = -1, i = e.length; ++r < i;) n = e[r], t.point(n[0], n[1], n[2])
-                        },
-                        LineString: function(n, t) {
-                            Me(n.coordinates, t, 0)
-                        },
-                        MultiLineString: function(n, t) {
-                            for (var e = n.coordinates, r = -1, i = e.length; ++r < i;) Me(e[r], t, 0)
-                        },
-                        Polygon: function(n, t) {
-                            xe(n.coordinates, t)
-                        },
-                        MultiPolygon: function(n, t) {
-                            for (var e = n.coordinates, r = -1, i = e.length; ++r < i;) xe(e[r], t)
-                        },
-                        GeometryCollection: function(n, t) {
-                            for (var e = n.geometries, r = -1, i = e.length; ++r < i;) de(e[r], t)
-                        }
-                    };
+    function re(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e, e + 2));
+        return r ? (n.S = +r[0], e + r[0].length) : -1
+    }
 
-                function Me(n, t, e) {
-                    var r, i = -1,
-                        u = n.length - e;
-                    for (t.lineStart(); ++i < u;) r = n[i], t.point(r[0], r[1], r[2]);
-                    t.lineEnd()
-                }
+    function ue(n, t, e) {
+        ac.lastIndex = 0;
+        var r = ac.exec(t.slice(e, e + 3));
+        return r ? (n.L = +r[0], e + r[0].length) : -1
+    }
 
-                function xe(n, t) {
-                    var e = -1,
-                        r = n.length;
-                    for (t.polygonStart(); ++e < r;) Me(n[e], t, 1);
-                    t.polygonEnd()
-                }
-                u.geo.area = function(n) {
-                    return be = 0, u.geo.stream(n, Re), be
-                };
-                var be, we, _e, ke, Se, Ne, Ee, Ae, Ce, ze, Le, qe, Te = new pe,
-                    Re = {
-                        sphere: function() {
-                            be += 4 * Ln
-                        },
-                        point: j,
-                        lineStart: j,
-                        lineEnd: j,
-                        polygonStart: function() {
-                            Te.reset(), Re.lineStart = De
-                        },
-                        polygonEnd: function() {
-                            var n = 2 * Te;
-                            be += n < 0 ? 4 * Ln + n : n, Re.lineStart = Re.lineEnd = Re.point = j
-                        }
-                    };
+    function ie(n) {
+        var t = n.getTimezoneOffset(),
+            e = t > 0 ? "-" : "+",
+            r = 0 | ca(t) / 60,
+            u = ca(t) % 60;
+        return e + Yt(r, "0", 2) + Yt(u, "0", 2)
+    }
 
-                function De() {
-                    var n, t, e, r, i;
+    function oe(n, t, e) {
+        cc.lastIndex = 0;
+        var r = cc.exec(t.slice(e, e + 1));
+        return r ? e + r[0].length : -1
+    }
 
-                    function u(n, t) {
-                        t = t * Dn / 2 + Ln / 4;
-                        var u = (n *= Dn) - e,
-                            o = u >= 0 ? 1 : -1,
-                            a = o * u,
-                            l = Math.cos(t),
-                            c = Math.sin(t),
-                            f = i * c,
-                            s = r * l + f * Math.cos(a),
-                            h = f * o * Math.sin(a);
-                        Te.add(Math.atan2(h, s)), e = n, r = l, i = c
-                    }
-                    Re.point = function(o, a) {
-                        Re.point = u, e = (n = o) * Dn, r = Math.cos(a = (t = a) * Dn / 2 + Ln / 4), i = Math.sin(a)
-                    }, Re.lineEnd = function() {
-                        u(n, t)
-                    }
-                }
+    function ae(n) {
+        for (var t = n.length, e = -1; ++e < t;) n[e][0] = this(n[e][0]);
+        return function(t) {
+            for (var e = 0, r = n[e]; !r[1](t);) r = n[++e];
+            return r[0](t)
+        }
+    }
 
-                function Pe(n) {
-                    var t = n[0],
-                        e = n[1],
-                        r = Math.cos(e);
-                    return [r * Math.cos(t), r * Math.sin(t), Math.sin(e)]
-                }
+    function ce() {}
 
-                function Ue(n, t) {
-                    return n[0] * t[0] + n[1] * t[1] + n[2] * t[2]
-                }
+    function le(n, t, e) {
+        var r = e.s = n + t,
+            u = r - n,
+            i = r - u;
+        e.t = n - i + (t - u)
+    }
 
-                function je(n, t) {
-                    return [n[1] * t[2] - n[2] * t[1], n[2] * t[0] - n[0] * t[2], n[0] * t[1] - n[1] * t[0]]
-                }
+    function se(n, t) {
+        n && hc.hasOwnProperty(n.type) && hc[n.type](n, t)
+    }
 
-                function Fe(n, t) {
-                    n[0] += t[0], n[1] += t[1], n[2] += t[2]
-                }
+    function fe(n, t, e) {
+        var r, u = -1,
+            i = n.length - e;
+        for (t.lineStart(); ++u < i;) r = n[u], t.point(r[0], r[1], r[2]);
+        t.lineEnd()
+    }
 
-                function He(n, t) {
-                    return [n[0] * t, n[1] * t, n[2] * t]
-                }
+    function he(n, t) {
+        var e = -1,
+            r = n.length;
+        for (t.polygonStart(); ++e < r;) fe(n[e], t, 1);
+        t.polygonEnd()
+    }
 
-                function Oe(n) {
-                    var t = Math.sqrt(n[0] * n[0] + n[1] * n[1] + n[2] * n[2]);
-                    n[0] /= t, n[1] /= t, n[2] /= t
-                }
+    function ge() {
+        function n(n, t) {
+            n *= La, t = t * La / 2 + Ea / 4;
+            var e = n - r,
+                o = e >= 0 ? 1 : -1,
+                a = o * e,
+                c = Math.cos(t),
+                l = Math.sin(t),
+                s = i * l,
+                f = u * c + s * Math.cos(a),
+                h = s * o * Math.sin(a);
+            pc.add(Math.atan2(h, f)), r = n, u = c, i = l
+        }
+        var t, e, r, u, i;
+        vc.point = function(o, a) {
+            vc.point = n, r = (t = o) * La, u = Math.cos(a = (e = a) * La / 2 + Ea / 4), i = Math.sin(a)
+        }, vc.lineEnd = function() {
+            n(t, e)
+        }
+    }
 
-                function Ie(n) {
-                    return [Math.atan2(n[1], n[0]), Hn(n[2])]
-                }
+    function pe(n) {
+        var t = n[0],
+            e = n[1],
+            r = Math.cos(e);
+        return [r * Math.cos(t), r * Math.sin(t), Math.sin(e)]
+    }
 
-                function Ye(n, t) {
-                    return w(n[0] - t[0]) < Cn && w(n[1] - t[1]) < Cn
-                }
-                u.geo.bounds = function() {
-                    var n, t, e, r, i, o, a, l, c, f, s, h = {
-                        point: p,
-                        lineStart: v,
-                        lineEnd: d,
-                        polygonStart: function() {
-                            h.point = y, h.lineStart = m, h.lineEnd = M, c = 0, Re.polygonStart()
-                        },
-                        polygonEnd: function() {
-                            Re.polygonEnd(), h.point = p, h.lineStart = v, h.lineEnd = d, Te < 0 ? (n = -(e = 180), t = -(r = 90)) : c > Cn ? r = 90 : c < -Cn && (t = -90), s[0] = n, s[1] = e
-                        }
-                    };
+    function ve(n, t) {
+        return n[0] * t[0] + n[1] * t[1] + n[2] * t[2]
+    }
 
-                    function p(i, u) {
-                        f.push(s = [n = i, e = i]), u < t && (t = u), u > r && (r = u)
-                    }
+    function de(n, t) {
+        return [n[1] * t[2] - n[2] * t[1], n[2] * t[0] - n[0] * t[2], n[0] * t[1] - n[1] * t[0]]
+    }
 
-                    function g(u, o) {
-                        var a = Pe([u * Dn, o * Dn]);
-                        if (l) {
-                            var c = je(l, a),
-                                f = je([c[1], -c[0], 0], c);
-                            Oe(f), f = Ie(f);
-                            var s = u - i,
-                                h = s > 0 ? 1 : -1,
-                                g = f[0] * Pn * h,
-                                v = w(s) > 180;
-                            if (v ^ (h * i < g && g < h * u))(d = f[1] * Pn) > r && (r = d);
-                            else if (v ^ (h * i < (g = (g + 360) % 360 - 180) && g < h * u)) {
-                                var d;
-                                (d = -f[1] * Pn) < t && (t = d)
-                            } else o < t && (t = o), o > r && (r = o);
-                            v ? u < i ? x(n, u) > x(n, e) && (e = u) : x(u, e) > x(n, e) && (n = u) : e >= n ? (u < n && (n = u), u > e && (e = u)) : u > i ? x(n, u) > x(n, e) && (e = u) : x(u, e) > x(n, e) && (n = u)
-                        } else p(u, o);
-                        l = a, i = u
-                    }
+    function me(n, t) {
+        n[0] += t[0], n[1] += t[1], n[2] += t[2]
+    }
 
-                    function v() {
-                        h.point = g
-                    }
+    function ye(n, t) {
+        return [n[0] * t, n[1] * t, n[2] * t]
+    }
 
-                    function d() {
-                        s[0] = n, s[1] = e, h.point = p, l = null
-                    }
+    function xe(n) {
+        var t = Math.sqrt(n[0] * n[0] + n[1] * n[1] + n[2] * n[2]);
+        n[0] /= t, n[1] /= t, n[2] /= t
+    }
 
-                    function y(n, t) {
-                        if (l) {
-                            var e = n - i;
-                            c += w(e) > 180 ? e + (e > 0 ? 360 : -360) : e
-                        } else o = n, a = t;
-                        Re.point(n, t), g(n, t)
-                    }
+    function Me(n) {
+        return [Math.atan2(n[1], n[0]), nt(n[2])]
+    }
 
-                    function m() {
-                        Re.lineStart()
-                    }
+    function _e(n, t) {
+        return ca(n[0] - t[0]) < Na && ca(n[1] - t[1]) < Na
+    }
 
-                    function M() {
-                        y(o, a), Re.lineEnd(), w(c) > Cn && (n = -(e = 180)), s[0] = n, s[1] = e, l = null
-                    }
+    function be(n, t) {
+        n *= La;
+        var e = Math.cos(t *= La);
+        we(e * Math.cos(n), e * Math.sin(n), Math.sin(t))
+    }
 
-                    function x(n, t) {
-                        return (t -= n) < 0 ? t + 360 : t
-                    }
+    function we(n, t, e) {
+        ++dc, yc += (n - yc) / dc, xc += (t - xc) / dc, Mc += (e - Mc) / dc
+    }
 
-                    function b(n, t) {
-                        return n[0] - t[0]
-                    }
+    function Se() {
+        function n(n, u) {
+            n *= La;
+            var i = Math.cos(u *= La),
+                o = i * Math.cos(n),
+                a = i * Math.sin(n),
+                c = Math.sin(u),
+                l = Math.atan2(Math.sqrt((l = e * c - r * a) * l + (l = r * o - t * c) * l + (l = t * a - e * o) * l), t * o + e * a + r * c);
+            mc += l, _c += l * (t + (t = o)), bc += l * (e + (e = a)), wc += l * (r + (r = c)), we(t, e, r)
+        }
+        var t, e, r;
+        Ac.point = function(u, i) {
+            u *= La;
+            var o = Math.cos(i *= La);
+            t = o * Math.cos(u), e = o * Math.sin(u), r = Math.sin(i), Ac.point = n, we(t, e, r)
+        }
+    }
 
-                    function _(n, t) {
-                        return t[0] <= t[1] ? t[0] <= n && n <= t[1] : n < t[0] || t[1] < n
-                    }
-                    return function(i) {
-                        if (r = e = -(n = t = 1 / 0), f = [], u.geo.stream(i, h), c = f.length) {
-                            f.sort(b);
-                            for (var o = 1, a = [v = f[0]]; o < c; ++o) _((p = f[o])[0], v) || _(p[1], v) ? (x(v[0], p[1]) > x(v[0], v[1]) && (v[1] = p[1]), x(p[0], v[1]) > x(v[0], v[1]) && (v[0] = p[0])) : a.push(v = p);
-                            for (var l, c, p, g = -1 / 0, v = (o = 0, a[c = a.length - 1]); o <= c; v = p, ++o) p = a[o], (l = x(v[1], p[0])) > g && (g = l, n = p[0], e = v[1])
-                        }
-                        return f = s = null, n === 1 / 0 || t === 1 / 0 ? [
-                            [NaN, NaN],
-                            [NaN, NaN]
-                        ] : [
-                            [n, t],
-                            [e, r]
-                        ]
-                    }
-                }(), u.geo.centroid = function(n) {
-                    we = _e = ke = Se = Ne = Ee = Ae = Ce = ze = Le = qe = 0, u.geo.stream(n, Ze);
-                    var t = ze,
-                        e = Le,
-                        r = qe,
-                        i = t * t + e * e + r * r;
-                    return i < zn && (t = Ee, e = Ae, r = Ce, _e < Cn && (t = ke, e = Se, r = Ne), (i = t * t + e * e + r * r) < zn) ? [NaN, NaN] : [Math.atan2(e, t) * Pn, Hn(r / Math.sqrt(i)) * Pn]
-                };
-                var Ze = {
-                    sphere: j,
-                    point: Ve,
-                    lineStart: $e,
-                    lineEnd: Be,
-                    polygonStart: function() {
-                        Ze.lineStart = Je
-                    },
-                    polygonEnd: function() {
-                        Ze.lineStart = $e
-                    }
-                };
+    function ke() {
+        Ac.point = be
+    }
 
-                function Ve(n, t) {
-                    n *= Dn;
-                    var e = Math.cos(t *= Dn);
-                    Xe(e * Math.cos(n), e * Math.sin(n), Math.sin(t))
-                }
-
-                function Xe(n, t, e) {
-                    ++we, ke += (n - ke) / we, Se += (t - Se) / we, Ne += (e - Ne) / we
-                }
-
-                function $e() {
-                    var n, t, e;
-
-                    function r(r, i) {
-                        r *= Dn;
-                        var u = Math.cos(i *= Dn),
-                            o = u * Math.cos(r),
-                            a = u * Math.sin(r),
-                            l = Math.sin(i),
-                            c = Math.atan2(Math.sqrt((c = t * l - e * a) * c + (c = e * o - n * l) * c + (c = n * a - t * o) * c), n * o + t * a + e * l);
-                        _e += c, Ee += c * (n + (n = o)), Ae += c * (t + (t = a)), Ce += c * (e + (e = l)), Xe(n, t, e)
-                    }
-                    Ze.point = function(i, u) {
-                        i *= Dn;
-                        var o = Math.cos(u *= Dn);
-                        n = o * Math.cos(i), t = o * Math.sin(i), e = Math.sin(u), Ze.point = r, Xe(n, t, e)
-                    }
-                }
+    function Ee() {
+        function n(n, t) {
+            n *= La;
+            var e = Math.cos(t *= La),
+                o = e * Math.cos(n),
+                a = e * Math.sin(n),
+                c = Math.sin(t),
+                l = u * c - i * a,
+                s = i * o - r * c,
+                f = r * a - u * o,
+                h = Math.sqrt(l * l + s * s + f * f),
+                g = r * o + u * a + i * c,
+                p = h && -Q(g) / h,
+                v = Math.atan2(h, g);
+            Sc += p * l, kc += p * s, Ec += p * f, mc += v, _c += v * (r + (r = o)), bc += v * (u + (u = a)), wc += v * (i + (i = c)), we(r, u, i)
+        }
+        var t, e, r, u, i;
+        Ac.point = function(o, a) {
+            t = o, e = a, Ac.point = n, o *= La;
+            var c = Math.cos(a *= La);
+            r = c * Math.cos(o), u = c * Math.sin(o), i = Math.sin(a), we(r, u, i)
+        }, Ac.lineEnd = function() {
+            n(t, e), Ac.lineEnd = ke, Ac.point = be
+        }
+    }
 
-                function Be() {
-                    Ze.point = Ve
-                }
+    function Ae() {
+        return !0
+    }
 
-                function Je() {
-                    var n, t, e, r, i;
+    function Ce(n, t, e, r, u) {
+        var i = [],
+            o = [];
+        if (n.forEach(function(n) {
+                if (!((t = n.length - 1) <= 0)) {
+                    var t, e = n[0],
+                        r = n[t];
+                    if (_e(e, r)) {
+                        u.lineStart();
+                        for (var a = 0; t > a; ++a) u.point((e = n[a])[0], e[1]);
+                        return u.lineEnd(), void 0
+                    }
+                    var c = new ze(e, n, null, !0),
+                        l = new ze(e, null, c, !1);
+                    c.o = l, i.push(c), o.push(l), c = new ze(r, n, null, !1), l = new ze(r, null, c, !0), c.o = l, i.push(c), o.push(l)
+                }
+            }), o.sort(t), Ne(i), Ne(o), i.length) {
+            for (var a = 0, c = e, l = o.length; l > a; ++a) o[a].e = c = !c;
+            for (var s, f, h = i[0];;) {
+                for (var g = h, p = !0; g.v;)
+                    if ((g = g.n) === h) return;
+                s = g.z, u.lineStart();
+                do {
+                    if (g.v = g.o.v = !0, g.e) {
+                        if (p)
+                            for (var a = 0, l = s.length; l > a; ++a) u.point((f = s[a])[0], f[1]);
+                        else r(g.x, g.n.x, 1, u);
+                        g = g.n
+                    } else {
+                        if (p) {
+                            s = g.p.z;
+                            for (var a = s.length - 1; a >= 0; --a) u.point((f = s[a])[0], f[1])
+                        } else r(g.x, g.p.x, -1, u);
+                        g = g.p
+                    }
+                    g = g.o, s = g.z, p = !p
+                } while (!g.v);
+                u.lineEnd()
+            }
+        }
+    }
 
-                    function u(n, t) {
-                        n *= Dn;
-                        var u = Math.cos(t *= Dn),
-                            o = u * Math.cos(n),
-                            a = u * Math.sin(n),
-                            l = Math.sin(t),
-                            c = r * l - i * a,
-                            f = i * o - e * l,
-                            s = e * a - r * o,
-                            h = Math.sqrt(c * c + f * f + s * s),
-                            p = e * o + r * a + i * l,
-                            g = h && -Fn(p) / h,
-                            v = Math.atan2(h, p);
-                        ze += g * c, Le += g * f, qe += g * s, _e += v, Ee += v * (e + (e = o)), Ae += v * (r + (r = a)), Ce += v * (i + (i = l)), Xe(e, r, i)
-                    }
-                    Ze.point = function(o, a) {
-                        n = o, t = a, Ze.point = u, o *= Dn;
-                        var l = Math.cos(a *= Dn);
-                        e = l * Math.cos(o), r = l * Math.sin(o), i = Math.sin(a), Xe(e, r, i)
-                    }, Ze.lineEnd = function() {
-                        u(n, t), Ze.lineEnd = Be, Ze.point = Ve
-                    }
-                }
+    function Ne(n) {
+        if (t = n.length) {
+            for (var t, e, r = 0, u = n[0]; ++r < t;) u.n = e = n[r], e.p = u, u = e;
+            u.n = e = n[0], e.p = u
+        }
+    }
 
-                function We(n, t) {
-                    function e(e, r) {
-                        return e = n(e, r), t(e[0], e[1])
-                    }
-                    return n.invert && t.invert && (e.invert = function(e, r) {
-                        return (e = t.invert(e, r)) && n.invert(e[0], e[1])
-                    }), e
-                }
-
-                function Ge() {
-                    return !0
-                }
-
-                function Ke(n, t, e, r, i) {
-                    var u = [],
-                        o = [];
-                    if (n.forEach((function(n) {
-                            if (!((t = n.length - 1) <= 0)) {
-                                var t, e = n[0],
-                                    r = n[t];
-                                if (Ye(e, r)) {
-                                    i.lineStart();
-                                    for (var a = 0; a < t; ++a) i.point((e = n[a])[0], e[1]);
-                                    i.lineEnd()
-                                } else {
-                                    var l = new nr(e, n, null, !0),
-                                        c = new nr(e, null, l, !1);
-                                    l.o = c, u.push(l), o.push(c), l = new nr(r, n, null, !1), c = new nr(r, null, l, !0), l.o = c, u.push(l), o.push(c)
-                                }
-                            }
-                        })), o.sort(t), Qe(u), Qe(o), u.length) {
-                        for (var a = 0, l = e, c = o.length; a < c; ++a) o[a].e = l = !l;
-                        for (var f, s, h = u[0];;) {
-                            for (var p = h, g = !0; p.v;)
-                                if ((p = p.n) === h) return;
-                            f = p.z, i.lineStart();
-                            do {
-                                if (p.v = p.o.v = !0, p.e) {
-                                    if (g)
-                                        for (a = 0, c = f.length; a < c; ++a) i.point((s = f[a])[0], s[1]);
-                                    else r(p.x, p.n.x, 1, i);
-                                    p = p.n
-                                } else {
-                                    if (g)
-                                        for (a = (f = p.p.z).length - 1; a >= 0; --a) i.point((s = f[a])[0], s[1]);
-                                    else r(p.x, p.p.x, -1, i);
-                                    p = p.p
-                                }
-                                f = (p = p.o).z, g = !g
-                            } while (!p.v);
+    function ze(n, t, e, r) {
+        this.x = n, this.z = t, this.o = e, this.e = r, this.v = !1, this.n = this.p = null
+    }
+
+    function Le(n, t, e, r) {
+        return function(u, i) {
+            function o(t, e) {
+                var r = u(t, e);
+                n(t = r[0], e = r[1]) && i.point(t, e)
+            }
+
+            function a(n, t) {
+                var e = u(n, t);
+                d.point(e[0], e[1])
+            }
+
+            function c() {
+                y.point = a, d.lineStart()
+            }
+
+            function l() {
+                y.point = o, d.lineEnd()
+            }
+
+            function s(n, t) {
+                v.push([n, t]);
+                var e = u(n, t);
+                M.point(e[0], e[1])
+            }
+
+            function f() {
+                M.lineStart(), v = []
+            }
+
+            function h() {
+                s(v[0][0], v[0][1]), M.lineEnd();
+                var n, t = M.clean(),
+                    e = x.buffer(),
+                    r = e.length;
+                if (v.pop(), p.push(v), v = null, r)
+                    if (1 & t) {
+                        n = e[0];
+                        var u, r = n.length - 1,
+                            o = -1;
+                        if (r > 0) {
+                            for (_ || (i.polygonStart(), _ = !0), i.lineStart(); ++o < r;) i.point((u = n[o])[0], u[1]);
                             i.lineEnd()
                         }
+                    } else r > 1 && 2 & t && e.push(e.pop().concat(e.shift())), g.push(e.filter(Te))
+            }
+            var g, p, v, d = t(i),
+                m = u.invert(r[0], r[1]),
+                y = {
+                    point: o,
+                    lineStart: c,
+                    lineEnd: l,
+                    polygonStart: function() {
+                        y.point = s, y.lineStart = f, y.lineEnd = h, g = [], p = []
+                    },
+                    polygonEnd: function() {
+                        y.point = o, y.lineStart = c, y.lineEnd = l, g = Bo.merge(g);
+                        var n = je(m, p);
+                        g.length ? (_ || (i.polygonStart(), _ = !0), Ce(g, Re, n, e, i)) : n && (_ || (i.polygonStart(), _ = !0), i.lineStart(), e(null, null, 1, i), i.lineEnd()), _ && (i.polygonEnd(), _ = !1), g = p = null
+                    },
+                    sphere: function() {
+                        i.polygonStart(), i.lineStart(), e(null, null, 1, i), i.lineEnd(), i.polygonEnd()
                     }
-                }
-
-                function Qe(n) {
-                    if (t = n.length) {
-                        for (var t, e, r = 0, i = n[0]; ++r < t;) i.n = e = n[r], e.p = i, i = e;
-                        i.n = e = n[0], e.p = i
-                    }
-                }
+                },
+                x = qe(),
+                M = t(x),
+                _ = !1;
+            return y
+        }
+    }
 
-                function nr(n, t, e, r) {
-                    this.x = n, this.z = t, this.o = e, this.e = r, this.v = !1, this.n = this.p = null
-                }
+    function Te(n) {
+        return n.length > 1
+    }
 
-                function tr(n, t, e, r) {
-                    return function(i, o) {
-                        var a, l = t(o),
-                            c = i.invert(r[0], r[1]),
-                            f = {
-                                point: s,
-                                lineStart: p,
-                                lineEnd: g,
-                                polygonStart: function() {
-                                    f.point = x, f.lineStart = b, f.lineEnd = w, a = [], v = []
-                                },
-                                polygonEnd: function() {
-                                    f.point = s, f.lineStart = p, f.lineEnd = g, a = u.merge(a);
-                                    var n = function(n, t) {
-                                        var e = n[0],
-                                            r = n[1],
-                                            i = [Math.sin(e), -Math.cos(e), 0],
-                                            u = 0,
-                                            o = 0;
-                                        Te.reset();
-                                        for (var a = 0, l = t.length; a < l; ++a) {
-                                            var c = t[a],
-                                                f = c.length;
-                                            if (f)
-                                                for (var s = c[0], h = s[0], p = s[1] / 2 + Ln / 4, g = Math.sin(p), v = Math.cos(p), d = 1;;) {
-                                                    d === f && (d = 0);
-                                                    var y = (n = c[d])[0],
-                                                        m = n[1] / 2 + Ln / 4,
-                                                        M = Math.sin(m),
-                                                        x = Math.cos(m),
-                                                        b = y - h,
-                                                        w = b >= 0 ? 1 : -1,
-                                                        _ = w * b,
-                                                        k = _ > Ln,
-                                                        S = g * M;
-                                                    if (Te.add(Math.atan2(S * w * Math.sin(_), v * x + S * Math.cos(_))), u += k ? b + w * qn : b, k ^ h >= e ^ y >= e) {
-                                                        var N = je(Pe(s), Pe(n));
-                                                        Oe(N);
-                                                        var E = je(i, N);
-                                                        Oe(E);
-                                                        var A = (k ^ b >= 0 ? -1 : 1) * Hn(E[2]);
-                                                        (r > A || r === A && (N[0] || N[1])) && (o += k ^ b >= 0 ? 1 : -1)
-                                                    }
-                                                    if (!d++) break;
-                                                    h = y, g = M, v = x, s = n
-                                                }
-                                        }
-                                        return (u < -Cn || u < Cn && Te < -Cn) ^ 1 & o
-                                    }(c, v);
-                                    a.length ? (M || (o.polygonStart(), M = !0), Ke(a, ir, n, e, o)) : n && (M || (o.polygonStart(), M = !0), o.lineStart(), e(null, null, 1, o), o.lineEnd()), M && (o.polygonEnd(), M = !1), a = v = null
-                                },
-                                sphere: function() {
-                                    o.polygonStart(), o.lineStart(), e(null, null, 1, o), o.lineEnd(), o.polygonEnd()
-                                }
-                            };
-
-                        function s(t, e) {
-                            var r = i(t, e);
-                            n(t = r[0], e = r[1]) && o.point(t, e)
-                        }
+    function qe() {
+        var n, t = [];
+        return {
+            lineStart: function() {
+                t.push(n = [])
+            },
+            point: function(t, e) {
+                n.push([t, e])
+            },
+            lineEnd: y,
+            buffer: function() {
+                var e = t;
+                return t = [], n = null, e
+            },
+            rejoin: function() {
+                t.length > 1 && t.push(t.pop().concat(t.shift()))
+            }
+        }
+    }
 
-                        function h(n, t) {
-                            var e = i(n, t);
-                            l.point(e[0], e[1])
-                        }
+    function Re(n, t) {
+        return ((n = n.x)[0] < 0 ? n[1] - Ca - Na : Ca - n[1]) - ((t = t.x)[0] < 0 ? t[1] - Ca - Na : Ca - t[1])
+    }
 
-                        function p() {
-                            f.point = h, l.lineStart()
-                        }
+    function De(n) {
+        var t, e = 0 / 0,
+            r = 0 / 0,
+            u = 0 / 0;
+        return {
+            lineStart: function() {
+                n.lineStart(), t = 1
+            },
+            point: function(i, o) {
+                var a = i > 0 ? Ea : -Ea,
+                    c = ca(i - e);
+                ca(c - Ea) < Na ? (n.point(e, r = (r + o) / 2 > 0 ? Ca : -Ca), n.point(u, r), n.lineEnd(), n.lineStart(), n.point(a, r), n.point(i, r), t = 0) : u !== a && c >= Ea && (ca(e - u) < Na && (e -= u * Na), ca(i - a) < Na && (i -= a * Na), r = Pe(e, r, i, o), n.point(u, r), n.lineEnd(), n.lineStart(), n.point(a, r), t = 0), n.point(e = i, r = o), u = a
+            },
+            lineEnd: function() {
+                n.lineEnd(), e = r = 0 / 0
+            },
+            clean: function() {
+                return 2 - t
+            }
+        }
+    }
 
-                        function g() {
-                            f.point = s, l.lineEnd()
-                        }
-                        var v, d, y = rr(),
-                            m = t(y),
-                            M = !1;
-
-                        function x(n, t) {
-                            d.push([n, t]);
-                            var e = i(n, t);
-                            m.point(e[0], e[1])
-                        }
+    function Pe(n, t, e, r) {
+        var u, i, o = Math.sin(n - e);
+        return ca(o) > Na ? Math.atan((Math.sin(t) * (i = Math.cos(r)) * Math.sin(e) - Math.sin(r) * (u = Math.cos(t)) * Math.sin(n)) / (u * i * o)) : (t + r) / 2
+    }
 
-                        function b() {
-                            m.lineStart(), d = []
-                        }
+    function Ue(n, t, e, r) {
+        var u;
+        if (null == n) u = e * Ca, r.point(-Ea, u), r.point(0, u), r.point(Ea, u), r.point(Ea, 0), r.point(Ea, -u), r.point(0, -u), r.point(-Ea, -u), r.point(-Ea, 0), r.point(-Ea, u);
+        else if (ca(n[0] - t[0]) > Na) {
+            var i = n[0] < t[0] ? Ea : -Ea;
+            u = e * i / 2, r.point(-i, u), r.point(0, u), r.point(i, u)
+        } else r.point(t[0], t[1])
+    }
 
-                        function w() {
-                            x(d[0][0], d[0][1]), m.lineEnd();
-                            var n, t = m.clean(),
-                                e = y.buffer(),
-                                r = e.length;
-                            if (d.pop(), v.push(d), d = null, r)
-                                if (1 & t) {
-                                    var i, u = -1;
-                                    if ((r = (n = e[0]).length - 1) > 0) {
-                                        for (M || (o.polygonStart(), M = !0), o.lineStart(); ++u < r;) o.point((i = n[u])[0], i[1]);
-                                        o.lineEnd()
-                                    }
-                                } else r > 1 && 2 & t && e.push(e.pop().concat(e.shift())), a.push(e.filter(er))
-                        }
-                        return f
+    function je(n, t) {
+        var e = n[0],
+            r = n[1],
+            u = [Math.sin(e), -Math.cos(e), 0],
+            i = 0,
+            o = 0;
+        pc.reset();
+        for (var a = 0, c = t.length; c > a; ++a) {
+            var l = t[a],
+                s = l.length;
+            if (s)
+                for (var f = l[0], h = f[0], g = f[1] / 2 + Ea / 4, p = Math.sin(g), v = Math.cos(g), d = 1;;) {
+                    d === s && (d = 0), n = l[d];
+                    var m = n[0],
+                        y = n[1] / 2 + Ea / 4,
+                        x = Math.sin(y),
+                        M = Math.cos(y),
+                        _ = m - h,
+                        b = _ >= 0 ? 1 : -1,
+                        w = b * _,
+                        S = w > Ea,
+                        k = p * x;
+                    if (pc.add(Math.atan2(k * b * Math.sin(w), v * M + k * Math.cos(w))), i += S ? _ + b * Aa : _, S ^ h >= e ^ m >= e) {
+                        var E = de(pe(f), pe(n));
+                        xe(E);
+                        var A = de(u, E);
+                        xe(A);
+                        var C = (S ^ _ >= 0 ? -1 : 1) * nt(A[2]);
+                        (r > C || r === C && (E[0] || E[1])) && (o += S ^ _ >= 0 ? 1 : -1)
                     }
+                    if (!d++) break;
+                    h = m, p = x, v = M, f = n
                 }
+        }
+        return (-Na > i || Na > i && 0 > pc) ^ 1 & o
+    }
 
-                function er(n) {
-                    return n.length > 1
-                }
+    function Fe(n) {
+        function t(n, t) {
+            return Math.cos(n) * Math.cos(t) > i
+        }
 
-                function rr() {
-                    var n, t = [];
-                    return {
-                        lineStart: function() {
-                            t.push(n = [])
-                        },
-                        point: function(t, e) {
-                            n.push([t, e])
-                        },
-                        lineEnd: j,
-                        buffer: function() {
-                            var e = t;
-                            return t = [], n = null, e
-                        },
-                        rejoin: function() {
-                            t.length > 1 && t.push(t.pop().concat(t.shift()))
-                        }
-                    }
+        function e(n) {
+            var e, i, c, l, s;
+            return {
+                lineStart: function() {
+                    l = c = !1, s = 1
+                },
+                point: function(f, h) {
+                    var g, p = [f, h],
+                        v = t(f, h),
+                        d = o ? v ? 0 : u(f, h) : v ? u(f + (0 > f ? Ea : -Ea), h) : 0;
+                    if (!e && (l = c = v) && n.lineStart(), v !== c && (g = r(e, p), (_e(e, g) || _e(p, g)) && (p[0] += Na, p[1] += Na, v = t(p[0], p[1]))), v !== c) s = 0, v ? (n.lineStart(), g = r(p, e), n.point(g[0], g[1])) : (g = r(e, p), n.point(g[0], g[1]), n.lineEnd()), e = g;
+                    else if (a && e && o ^ v) {
+                        var m;
+                        d & i || !(m = r(p, e, !0)) || (s = 0, o ? (n.lineStart(), n.point(m[0][0], m[0][1]), n.point(m[1][0], m[1][1]), n.lineEnd()) : (n.point(m[1][0], m[1][1]), n.lineEnd(), n.lineStart(), n.point(m[0][0], m[0][1])))
+                    }!v || e && _e(e, p) || n.point(p[0], p[1]), e = p, c = v, i = d
+                },
+                lineEnd: function() {
+                    c && n.lineEnd(), e = null
+                },
+                clean: function() {
+                    return s | (l && c) << 1
                 }
+            }
+        }
 
-                function ir(n, t) {
-                    return ((n = n.x)[0] < 0 ? n[1] - Rn - Cn : Rn - n[1]) - ((t = t.x)[0] < 0 ? t[1] - Rn - Cn : Rn - t[1])
+        function r(n, t, e) {
+            var r = pe(n),
+                u = pe(t),
+                o = [1, 0, 0],
+                a = de(r, u),
+                c = ve(a, a),
+                l = a[0],
+                s = c - l * l;
+            if (!s) return !e && n;
+            var f = i * c / s,
+                h = -i * l / s,
+                g = de(o, a),
+                p = ye(o, f),
+                v = ye(a, h);
+            me(p, v);
+            var d = g,
+                m = ve(p, d),
+                y = ve(d, d),
+                x = m * m - y * (ve(p, p) - 1);
+            if (!(0 > x)) {
+                var M = Math.sqrt(x),
+                    _ = ye(d, (-m - M) / y);
+                if (me(_, p), _ = Me(_), !e) return _;
+                var b, w = n[0],
+                    S = t[0],
+                    k = n[1],
+                    E = t[1];
+                w > S && (b = w, w = S, S = b);
+                var A = S - w,
+                    C = ca(A - Ea) < Na,
+                    N = C || Na > A;
+                if (!C && k > E && (b = k, k = E, E = b), N ? C ? k + E > 0 ^ _[1] < (ca(_[0] - w) < Na ? k : E) : k <= _[1] && _[1] <= E : A > Ea ^ (w <= _[0] && _[0] <= S)) {
+                    var z = ye(d, (-m + M) / y);
+                    return me(z, p), [_, Me(z)]
                 }
-                var ur = tr(Ge, (function(n) {
-                    var t, e = NaN,
-                        r = NaN,
-                        i = NaN;
-                    return {
-                        lineStart: function() {
-                            n.lineStart(), t = 1
-                        },
-                        point: function(u, o) {
-                            var a = u > 0 ? Ln : -Ln,
-                                l = w(u - e);
-                            w(l - Ln) < Cn ? (n.point(e, r = (r + o) / 2 > 0 ? Rn : -Rn), n.point(i, r), n.lineEnd(), n.lineStart(), n.point(a, r), n.point(u, r), t = 0) : i !== a && l >= Ln && (w(e - i) < Cn && (e -= i * Cn), w(u - a) < Cn && (u -= a * Cn), r = function(n, t, e, r) {
-                                var i, u, o = Math.sin(n - e);
-                                return w(o) > Cn ? Math.atan((Math.sin(t) * (u = Math.cos(r)) * Math.sin(e) - Math.sin(r) * (i = Math.cos(t)) * Math.sin(n)) / (i * u * o)) : (t + r) / 2
-                            }(e, r, u, o), n.point(i, r), n.lineEnd(), n.lineStart(), n.point(a, r), t = 0), n.point(e = u, r = o), i = a
-                        },
-                        lineEnd: function() {
-                            n.lineEnd(), e = r = NaN
-                        },
-                        clean: function() {
-                            return 2 - t
-                        }
-                    }
-                }), (function(n, t, e, r) {
-                    var i;
-                    if (null == n) i = e * Rn, r.point(-Ln, i), r.point(0, i), r.point(Ln, i), r.point(Ln, 0), r.point(Ln, -i), r.point(0, -i), r.point(-Ln, -i), r.point(-Ln, 0), r.point(-Ln, i);
-                    else if (w(n[0] - t[0]) > Cn) {
-                        var u = n[0] < t[0] ? Ln : -Ln;
-                        i = e * u / 2, r.point(-u, i), r.point(0, i), r.point(u, i)
-                    } else r.point(t[0], t[1])
-                }), [-Ln, -Ln / 2]);
-
-                function or(n) {
-                    var t = Math.cos(n),
-                        e = t > 0,
-                        r = w(t) > Cn;
-                    return tr(i, (function(n) {
-                        var t, a, l, c, f;
-                        return {
-                            lineStart: function() {
-                                c = l = !1, f = 1
-                            },
-                            point: function(s, h) {
-                                var p, g = [s, h],
-                                    v = i(s, h),
-                                    d = e ? v ? 0 : o(s, h) : v ? o(s + (s < 0 ? Ln : -Ln), h) : 0;
-                                if (!t && (c = l = v) && n.lineStart(), v !== l && (p = u(t, g), (Ye(t, p) || Ye(g, p)) && (g[0] += Cn, g[1] += Cn, v = i(g[0], g[1]))), v !== l) f = 0, v ? (n.lineStart(), p = u(g, t), n.point(p[0], p[1])) : (p = u(t, g), n.point(p[0], p[1]), n.lineEnd()), t = p;
-                                else if (r && t && e ^ v) {
-                                    var y;
-                                    d & a || !(y = u(g, t, !0)) || (f = 0, e ? (n.lineStart(), n.point(y[0][0], y[0][1]), n.point(y[1][0], y[1][1]), n.lineEnd()) : (n.point(y[1][0], y[1][1]), n.lineEnd(), n.lineStart(), n.point(y[0][0], y[0][1])))
-                                }!v || t && Ye(t, g) || n.point(g[0], g[1]), t = g, l = v, a = d
-                            },
-                            lineEnd: function() {
-                                l && n.lineEnd(), t = null
-                            },
-                            clean: function() {
-                                return f | (c && l) << 1
-                            }
-                        }
-                    }), Ir(n, 6 * Dn), e ? [0, -n] : [-Ln, n - Ln]);
-
-                    function i(n, e) {
-                        return Math.cos(n) * Math.cos(e) > t
-                    }
-
-                    function u(n, e, r) {
-                        var i = [1, 0, 0],
-                            u = je(Pe(n), Pe(e)),
-                            o = Ue(u, u),
-                            a = u[0],
-                            l = o - a * a;
-                        if (!l) return !r && n;
-                        var c = t * o / l,
-                            f = -t * a / l,
-                            s = je(i, u),
-                            h = He(i, c);
-                        Fe(h, He(u, f));
-                        var p = s,
-                            g = Ue(h, p),
-                            v = Ue(p, p),
-                            d = g * g - v * (Ue(h, h) - 1);
-                        if (!(d < 0)) {
-                            var y = Math.sqrt(d),
-                                m = He(p, (-g - y) / v);
-                            if (Fe(m, h), m = Ie(m), !r) return m;
-                            var M, x = n[0],
-                                b = e[0],
-                                _ = n[1],
-                                k = e[1];
-                            b < x && (M = x, x = b, b = M);
-                            var S = b - x,
-                                N = w(S - Ln) < Cn;
-                            if (!N && k < _ && (M = _, _ = k, k = M), N || S < Cn ? N ? _ + k > 0 ^ m[1] < (w(m[0] - x) < Cn ? _ : k) : _ <= m[1] && m[1] <= k : S > Ln ^ (x <= m[0] && m[0] <= b)) {
-                                var E = He(p, (-g + y) / v);
-                                return Fe(E, h), [m, Ie(E)]
-                            }
-                        }
-                    }
+            }
+        }
 
-                    function o(t, r) {
-                        var i = e ? n : Ln - n,
-                            u = 0;
-                        return t < -i ? u |= 1 : t > i && (u |= 2), r < -i ? u |= 4 : r > i && (u |= 8), u
-                    }
-                }
+        function u(t, e) {
+            var r = o ? n : Ea - n,
+                u = 0;
+            return -r > t ? u |= 1 : t > r && (u |= 2), -r > e ? u |= 4 : e > r && (u |= 8), u
+        }
+        var i = Math.cos(n),
+            o = i > 0,
+            a = ca(i) > Na,
+            c = gr(n, 6 * La);
+        return Le(t, e, c, o ? [0, -n] : [-Ea, n - Ea])
+    }
 
-                function ar(n, t, e, r) {
-                    return function(i) {
-                        var u, o = i.a,
-                            a = i.b,
-                            l = o.x,
-                            c = o.y,
-                            f = 0,
-                            s = 1,
-                            h = a.x - l,
-                            p = a.y - c;
-                        if (u = n - l, h || !(u > 0)) {
-                            if (u /= h, h < 0) {
-                                if (u < f) return;
-                                u < s && (s = u)
-                            } else if (h > 0) {
-                                if (u > s) return;
-                                u > f && (f = u)
-                            }
-                            if (u = e - l, h || !(u < 0)) {
-                                if (u /= h, h < 0) {
-                                    if (u > s) return;
-                                    u > f && (f = u)
-                                } else if (h > 0) {
-                                    if (u < f) return;
-                                    u < s && (s = u)
-                                }
-                                if (u = t - c, p || !(u > 0)) {
-                                    if (u /= p, p < 0) {
-                                        if (u < f) return;
-                                        u < s && (s = u)
-                                    } else if (p > 0) {
-                                        if (u > s) return;
-                                        u > f && (f = u)
-                                    }
-                                    if (u = r - c, p || !(u < 0)) {
-                                        if (u /= p, p < 0) {
-                                            if (u > s) return;
-                                            u > f && (f = u)
-                                        } else if (p > 0) {
-                                            if (u < f) return;
-                                            u < s && (s = u)
-                                        }
-                                        return f > 0 && (i.a = {
-                                            x: l + f * h,
-                                            y: c + f * p
-                                        }), s < 1 && (i.b = {
-                                            x: l + s * h,
-                                            y: c + s * p
-                                        }), i
-                                    }
-                                }
-                            }
+    function He(n, t, e, r) {
+        return function(u) {
+            var i, o = u.a,
+                a = u.b,
+                c = o.x,
+                l = o.y,
+                s = a.x,
+                f = a.y,
+                h = 0,
+                g = 1,
+                p = s - c,
+                v = f - l;
+            if (i = n - c, p || !(i > 0)) {
+                if (i /= p, 0 > p) {
+                    if (h > i) return;
+                    g > i && (g = i)
+                } else if (p > 0) {
+                    if (i > g) return;
+                    i > h && (h = i)
+                }
+                if (i = e - c, p || !(0 > i)) {
+                    if (i /= p, 0 > p) {
+                        if (i > g) return;
+                        i > h && (h = i)
+                    } else if (p > 0) {
+                        if (h > i) return;
+                        g > i && (g = i)
+                    }
+                    if (i = t - l, v || !(i > 0)) {
+                        if (i /= v, 0 > v) {
+                            if (h > i) return;
+                            g > i && (g = i)
+                        } else if (v > 0) {
+                            if (i > g) return;
+                            i > h && (h = i)
+                        }
+                        if (i = r - l, v || !(0 > i)) {
+                            if (i /= v, 0 > v) {
+                                if (i > g) return;
+                                i > h && (h = i)
+                            } else if (v > 0) {
+                                if (h > i) return;
+                                g > i && (g = i)
+                            }
+                            return h > 0 && (u.a = {
+                                x: c + h * p,
+                                y: l + h * v
+                            }), 1 > g && (u.b = {
+                                x: c + g * p,
+                                y: l + g * v
+                            }), u
                         }
                     }
                 }
+            }
+        }
+    }
 
-                function lr(n, t, e, r) {
-                    return function(l) {
-                        var c, f, s, h, p, g, v, d, y, m, M, x = l,
-                            b = rr(),
-                            w = ar(n, t, e, r),
-                            _ = {
-                                point: N,
-                                lineStart: function() {
-                                    _.point = E, f && f.push(s = []);
-                                    m = !0, y = !1, v = d = NaN
-                                },
-                                lineEnd: function() {
-                                    c && (E(h, p), g && y && b.rejoin(), c.push(b.buffer()));
-                                    _.point = N, y && l.lineEnd()
-                                },
-                                polygonStart: function() {
-                                    l = b, c = [], f = [], M = !0
-                                },
-                                polygonEnd: function() {
-                                    l = x, c = u.merge(c);
-                                    var t = function(n) {
-                                            for (var t = 0, e = f.length, r = n[1], i = 0; i < e; ++i)
-                                                for (var u, o = 1, a = f[i], l = a.length, c = a[0]; o < l; ++o) u = a[o], c[1] <= r ? u[1] > r && jn(c, u, n) > 0 && ++t : u[1] <= r && jn(c, u, n) < 0 && --t, c = u;
-                                            return 0 !== t
-                                        }([n, r]),
-                                        e = M && t,
-                                        i = c.length;
-                                    (e || i) && (l.polygonStart(), e && (l.lineStart(), k(null, null, 1, l), l.lineEnd()), i && Ke(c, o, t, k, l), l.polygonEnd()), c = f = s = null
-                                }
-                            };
-
-                        function k(u, o, l, c) {
-                            var f = 0,
-                                s = 0;
-                            if (null == u || (f = i(u, l)) !== (s = i(o, l)) || a(u, o) < 0 ^ l > 0)
-                                do {
-                                    c.point(0 === f || 3 === f ? n : e, f > 1 ? r : t)
-                                } while ((f = (f + l + 4) % 4) !== s);
-                            else c.point(o[0], o[1])
-                        }
-
-                        function S(i, u) {
-                            return n <= i && i <= e && t <= u && u <= r
-                        }
+    function Oe(n, t, e, r) {
+        function u(r, u) {
+            return ca(r[0] - n) < Na ? u > 0 ? 0 : 3 : ca(r[0] - e) < Na ? u > 0 ? 2 : 1 : ca(r[1] - t) < Na ? u > 0 ? 1 : 0 : u > 0 ? 3 : 2
+        }
 
-                        function N(n, t) {
-                            S(n, t) && l.point(n, t)
-                        }
+        function i(n, t) {
+            return o(n.x, t.x)
+        }
 
-                        function E(n, t) {
-                            var e = S(n = Math.max(-1e9, Math.min(1e9, n)), t = Math.max(-1e9, Math.min(1e9, t)));
-                            if (f && s.push([n, t]), m) h = n, p = t, g = e, m = !1, e && (l.lineStart(), l.point(n, t));
-                            else if (e && y) l.point(n, t);
-                            else {
-                                var r = {
-                                    a: {
-                                        x: v,
-                                        y: d
-                                    },
-                                    b: {
-                                        x: n,
-                                        y: t
-                                    }
-                                };
-                                w(r) ? (y || (l.lineStart(), l.point(r.a.x, r.a.y)), l.point(r.b.x, r.b.y), e || l.lineEnd(), M = !1) : e && (l.lineStart(), l.point(n, t), M = !1)
-                            }
-                            v = n, d = t, y = e
+        function o(n, t) {
+            var e = u(n, 1),
+                r = u(t, 1);
+            return e !== r ? e - r : 0 === e ? t[1] - n[1] : 1 === e ? n[0] - t[0] : 2 === e ? n[1] - t[1] : t[0] - n[0]
+        }
+        return function(a) {
+            function c(n) {
+                for (var t = 0, e = d.length, r = n[1], u = 0; e > u; ++u)
+                    for (var i, o = 1, a = d[u], c = a.length, l = a[0]; c > o; ++o) i = a[o], l[1] <= r ? i[1] > r && K(l, i, n) > 0 && ++t : i[1] <= r && K(l, i, n) < 0 && --t, l = i;
+                return 0 !== t
+            }
+
+            function l(i, a, c, l) {
+                var s = 0,
+                    f = 0;
+                if (null == i || (s = u(i, c)) !== (f = u(a, c)) || o(i, a) < 0 ^ c > 0) {
+                    do l.point(0 === s || 3 === s ? n : e, s > 1 ? r : t); while ((s = (s + c + 4) % 4) !== f)
+                } else l.point(a[0], a[1])
+            }
+
+            function s(u, i) {
+                return u >= n && e >= u && i >= t && r >= i
+            }
+
+            function f(n, t) {
+                s(n, t) && a.point(n, t)
+            }
+
+            function h() {
+                N.point = p, d && d.push(m = []), S = !0, w = !1, _ = b = 0 / 0
+            }
+
+            function g() {
+                v && (p(y, x), M && w && A.rejoin(), v.push(A.buffer())), N.point = f, w && a.lineEnd()
+            }
+
+            function p(n, t) {
+                n = Math.max(-Nc, Math.min(Nc, n)), t = Math.max(-Nc, Math.min(Nc, t));
+                var e = s(n, t);
+                if (d && m.push([n, t]), S) y = n, x = t, M = e, S = !1, e && (a.lineStart(), a.point(n, t));
+                else if (e && w) a.point(n, t);
+                else {
+                    var r = {
+                        a: {
+                            x: _,
+                            y: b
+                        },
+                        b: {
+                            x: n,
+                            y: t
                         }
-                        return _
                     };
-
-                    function i(r, i) {
-                        return w(r[0] - n) < Cn ? i > 0 ? 0 : 3 : w(r[0] - e) < Cn ? i > 0 ? 2 : 1 : w(r[1] - t) < Cn ? i > 0 ? 1 : 0 : i > 0 ? 3 : 2
-                    }
-
-                    function o(n, t) {
-                        return a(n.x, t.x)
-                    }
-
-                    function a(n, t) {
-                        var e = i(n, 1),
-                            r = i(t, 1);
-                        return e !== r ? e - r : 0 === e ? t[1] - n[1] : 1 === e ? n[0] - t[0] : 2 === e ? n[1] - t[1] : t[0] - n[0]
-                    }
+                    C(r) ? (w || (a.lineStart(), a.point(r.a.x, r.a.y)), a.point(r.b.x, r.b.y), e || a.lineEnd(), k = !1) : e && (a.lineStart(), a.point(n, t), k = !1)
                 }
-
-                function cr(n) {
-                    var t = 0,
-                        e = Ln / 3,
-                        r = Rr(n),
-                        i = r(t, e);
-                    return i.parallels = function(n) {
-                        return arguments.length ? r(t = n[0] * Ln / 180, e = n[1] * Ln / 180) : [t / Ln * 180, e / Ln * 180]
-                    }, i
-                }
-
-                function fr(n, t) {
-                    var e = Math.sin(n),
-                        r = (e + Math.sin(t)) / 2,
-                        i = 1 + e * (2 * r - e),
-                        u = Math.sqrt(i) / r;
-
-                    function o(n, t) {
-                        var e = Math.sqrt(i - 2 * r * Math.sin(t)) / r;
-                        return [e * Math.sin(n *= r), u - e * Math.cos(n)]
-                    }
-                    return o.invert = function(n, t) {
-                        var e = u - t;
-                        return [Math.atan2(n, e) / r, Hn((i - (n * n + e * e) * r * r) / (2 * r))]
-                    }, o
-                }
-                u.geo.clipExtent = function() {
-                    var n, t, e, r, i, u, o = {
-                        stream: function(n) {
-                            return i && (i.valid = !1), (i = u(n)).valid = !0, i
-                        },
-                        extent: function(a) {
-                            return arguments.length ? (u = lr(n = +a[0][0], t = +a[0][1], e = +a[1][0], r = +a[1][1]), i && (i.valid = !1, i = null), o) : [
-                                [n, t],
-                                [e, r]
-                            ]
-                        }
-                    };
-                    return o.extent([
-                        [0, 0],
-                        [960, 500]
-                    ])
-                }, (u.geo.conicEqualArea = function() {
-                    return cr(fr)
-                }).raw = fr, u.geo.albers = function() {
-                    return u.geo.conicEqualArea().rotate([96, 0]).center([-.6, 38.7]).parallels([29.5, 45.5]).scale(1070)
-                }, u.geo.albersUsa = function() {
-                    var n, t, e, r, i = u.geo.albers(),
-                        o = u.geo.conicEqualArea().rotate([154, 0]).center([-2, 58.5]).parallels([55, 65]),
-                        a = u.geo.conicEqualArea().rotate([157, 0]).center([-3, 19.9]).parallels([8, 18]),
-                        l = {
-                            point: function(t, e) {
-                                n = [t, e]
-                            }
-                        };
-
-                    function c(i) {
-                        var u = i[0],
-                            o = i[1];
-                        return n = null, t(u, o), n || (e(u, o), n) || r(u, o), n
-                    }
-                    return c.invert = function(n) {
-                        var t = i.scale(),
-                            e = i.translate(),
-                            r = (n[0] - e[0]) / t,
-                            u = (n[1] - e[1]) / t;
-                        return (u >= .12 && u < .234 && r >= -.425 && r < -.214 ? o : u >= .166 && u < .234 && r >= -.214 && r < -.115 ? a : i).invert(n)
-                    }, c.stream = function(n) {
-                        var t = i.stream(n),
-                            e = o.stream(n),
-                            r = a.stream(n);
-                        return {
-                            point: function(n, i) {
-                                t.point(n, i), e.point(n, i), r.point(n, i)
-                            },
-                            sphere: function() {
-                                t.sphere(), e.sphere(), r.sphere()
-                            },
-                            lineStart: function() {
-                                t.lineStart(), e.lineStart(), r.lineStart()
-                            },
-                            lineEnd: function() {
-                                t.lineEnd(), e.lineEnd(), r.lineEnd()
-                            },
-                            polygonStart: function() {
-                                t.polygonStart(), e.polygonStart(), r.polygonStart()
-                            },
-                            polygonEnd: function() {
-                                t.polygonEnd(), e.polygonEnd(), r.polygonEnd()
-                            }
-                        }
-                    }, c.precision = function(n) {
-                        return arguments.length ? (i.precision(n), o.precision(n), a.precision(n), c) : i.precision()
-                    }, c.scale = function(n) {
-                        return arguments.length ? (i.scale(n), o.scale(.35 * n), a.scale(n), c.translate(i.translate())) : i.scale()
-                    }, c.translate = function(n) {
-                        if (!arguments.length) return i.translate();
-                        var u = i.scale(),
-                            f = +n[0],
-                            s = +n[1];
-                        return t = i.translate(n).clipExtent([
-                            [f - .455 * u, s - .238 * u],
-                            [f + .455 * u, s + .238 * u]
-                        ]).stream(l).point, e = o.translate([f - .307 * u, s + .201 * u]).clipExtent([
-                            [f - .425 * u + Cn, s + .12 * u + Cn],
-                            [f - .214 * u - Cn, s + .234 * u - Cn]
-                        ]).stream(l).point, r = a.translate([f - .205 * u, s + .212 * u]).clipExtent([
-                            [f - .214 * u + Cn, s + .166 * u + Cn],
-                            [f - .115 * u - Cn, s + .234 * u - Cn]
-                        ]).stream(l).point, c
-                    }, c.scale(1070)
-                };
-                var sr, hr, pr, gr, vr, dr, yr = {
-                    point: j,
-                    lineStart: j,
-                    lineEnd: j,
+                _ = n, b = t, w = e
+            }
+            var v, d, m, y, x, M, _, b, w, S, k, E = a,
+                A = qe(),
+                C = He(n, t, e, r),
+                N = {
+                    point: f,
+                    lineStart: h,
+                    lineEnd: g,
                     polygonStart: function() {
-                        hr = 0, yr.lineStart = mr
+                        a = A, v = [], d = [], k = !0
                     },
                     polygonEnd: function() {
-                        yr.lineStart = yr.lineEnd = yr.point = j, sr += w(hr / 2)
+                        a = E, v = Bo.merge(v);
+                        var t = c([n, r]),
+                            e = k && t,
+                            u = v.length;
+                        (e || u) && (a.polygonStart(), e && (a.lineStart(), l(null, null, 1, a), a.lineEnd()), u && Ce(v, i, t, l, a), a.polygonEnd()), v = d = m = null
                     }
                 };
+            return N
+        }
+    }
 
-                function mr() {
-                    var n, t, e, r;
+    function Ye(n, t) {
+        function e(e, r) {
+            return e = n(e, r), t(e[0], e[1])
+        }
+        return n.invert && t.invert && (e.invert = function(e, r) {
+            return e = t.invert(e, r), e && n.invert(e[0], e[1])
+        }), e
+    }
 
-                    function i(n, t) {
-                        hr += r * n - e * t, e = n, r = t
-                    }
-                    yr.point = function(u, o) {
-                        yr.point = i, n = e = u, t = r = o
-                    }, yr.lineEnd = function() {
-                        i(n, t)
-                    }
-                }
-                var Mr = {
-                    point: function(n, t) {
-                        n < pr && (pr = n);
-                        n > vr && (vr = n);
-                        t < gr && (gr = t);
-                        t > dr && (dr = t)
-                    },
-                    lineStart: j,
-                    lineEnd: j,
-                    polygonStart: j,
-                    polygonEnd: j
-                };
+    function Ie(n) {
+        var t = 0,
+            e = Ea / 3,
+            r = ir(n),
+            u = r(t, e);
+        return u.parallels = function(n) {
+            return arguments.length ? r(t = n[0] * Ea / 180, e = n[1] * Ea / 180) : [180 * (t / Ea), 180 * (e / Ea)]
+        }, u
+    }
 
-                function xr() {
-                    var n = br(4.5),
-                        t = [],
-                        e = {
-                            point: r,
-                            lineStart: function() {
-                                e.point = i
-                            },
-                            lineEnd: o,
-                            polygonStart: function() {
-                                e.lineEnd = a
-                            },
-                            polygonEnd: function() {
-                                e.lineEnd = o, e.point = r
-                            },
-                            pointRadius: function(t) {
-                                return n = br(t), e
-                            },
-                            result: function() {
-                                if (t.length) {
-                                    var n = t.join("");
-                                    return t = [], n
-                                }
-                            }
-                        };
+    function Ze(n, t) {
+        function e(n, t) {
+            var e = Math.sqrt(i - 2 * u * Math.sin(t)) / u;
+            return [e * Math.sin(n *= u), o - e * Math.cos(n)]
+        }
+        var r = Math.sin(n),
+            u = (r + Math.sin(t)) / 2,
+            i = 1 + r * (2 * u - r),
+            o = Math.sqrt(i) / u;
+        return e.invert = function(n, t) {
+            var e = o - t;
+            return [Math.atan2(n, e) / u, nt((i - (n * n + e * e) * u * u) / (2 * u))]
+        }, e
+    }
 
-                    function r(e, r) {
-                        t.push("M", e, ",", r, n)
-                    }
+    function Ve() {
+        function n(n, t) {
+            Lc += u * n - r * t, r = n, u = t
+        }
+        var t, e, r, u;
+        Pc.point = function(i, o) {
+            Pc.point = n, t = r = i, e = u = o
+        }, Pc.lineEnd = function() {
+            n(t, e)
+        }
+    }
 
-                    function i(n, r) {
-                        t.push("M", n, ",", r), e.point = u
-                    }
+    function Xe(n, t) {
+        Tc > n && (Tc = n), n > Rc && (Rc = n), qc > t && (qc = t), t > Dc && (Dc = t)
+    }
 
-                    function u(n, e) {
-                        t.push("L", n, ",", e)
-                    }
+    function $e() {
+        function n(n, t) {
+            o.push("M", n, ",", t, i)
+        }
 
-                    function o() {
-                        e.point = r
-                    }
+        function t(n, t) {
+            o.push("M", n, ",", t), a.point = e
+        }
 
-                    function a() {
-                        t.push("Z")
+        function e(n, t) {
+            o.push("L", n, ",", t)
+        }
+
+        function r() {
+            a.point = n
+        }
+
+        function u() {
+            o.push("Z")
+        }
+        var i = Be(4.5),
+            o = [],
+            a = {
+                point: n,
+                lineStart: function() {
+                    a.point = t
+                },
+                lineEnd: r,
+                polygonStart: function() {
+                    a.lineEnd = u
+                },
+                polygonEnd: function() {
+                    a.lineEnd = r, a.point = n
+                },
+                pointRadius: function(n) {
+                    return i = Be(n), a
+                },
+                result: function() {
+                    if (o.length) {
+                        var n = o.join("");
+                        return o = [], n
                     }
-                    return e
                 }
+            };
+        return a
+    }
 
-                function br(n) {
-                    return "m0," + n + "a" + n + "," + n + " 0 1,1 0," + -2 * n + "a" + n + "," + n + " 0 1,1 0," + 2 * n + "z"
-                }
-                var wr, _r = {
-                    point: kr,
-                    lineStart: Sr,
-                    lineEnd: Nr,
-                    polygonStart: function() {
-                        _r.lineStart = Er
-                    },
-                    polygonEnd: function() {
-                        _r.point = kr, _r.lineStart = Sr, _r.lineEnd = Nr
-                    }
-                };
+    function Be(n) {
+        return "m0," + n + "a" + n + "," + n + " 0 1,1 0," + -2 * n + "a" + n + "," + n + " 0 1,1 0," + 2 * n + "z"
+    }
 
-                function kr(n, t) {
-                    ke += n, Se += t, ++Ne
-                }
+    function We(n, t) {
+        yc += n, xc += t, ++Mc
+    }
 
-                function Sr() {
-                    var n, t;
+    function Je() {
+        function n(n, r) {
+            var u = n - t,
+                i = r - e,
+                o = Math.sqrt(u * u + i * i);
+            _c += o * (t + n) / 2, bc += o * (e + r) / 2, wc += o, We(t = n, e = r)
+        }
+        var t, e;
+        jc.point = function(r, u) {
+            jc.point = n, We(t = r, e = u)
+        }
+    }
 
-                    function e(e, r) {
-                        var i = e - n,
-                            u = r - t,
-                            o = Math.sqrt(i * i + u * u);
-                        Ee += o * (n + e) / 2, Ae += o * (t + r) / 2, Ce += o, kr(n = e, t = r)
-                    }
-                    _r.point = function(r, i) {
-                        _r.point = e, kr(n = r, t = i)
-                    }
-                }
+    function Ge() {
+        jc.point = We
+    }
 
-                function Nr() {
-                    _r.point = kr
-                }
+    function Ke() {
+        function n(n, t) {
+            var e = n - r,
+                i = t - u,
+                o = Math.sqrt(e * e + i * i);
+            _c += o * (r + n) / 2, bc += o * (u + t) / 2, wc += o, o = u * n - r * t, Sc += o * (r + n), kc += o * (u + t), Ec += 3 * o, We(r = n, u = t)
+        }
+        var t, e, r, u;
+        jc.point = function(i, o) {
+            jc.point = n, We(t = r = i, e = u = o)
+        }, jc.lineEnd = function() {
+            n(t, e)
+        }
+    }
 
-                function Er() {
-                    var n, t, e, r;
+    function Qe(n) {
+        function t(t, e) {
+            n.moveTo(t, e), n.arc(t, e, o, 0, Aa)
+        }
 
-                    function i(n, t) {
-                        var i = n - e,
-                            u = t - r,
-                            o = Math.sqrt(i * i + u * u);
-                        Ee += o * (e + n) / 2, Ae += o * (r + t) / 2, Ce += o, ze += (o = r * n - e * t) * (e + n), Le += o * (r + t), qe += 3 * o, kr(e = n, r = t)
-                    }
-                    _r.point = function(u, o) {
-                        _r.point = i, kr(n = e = u, t = r = o)
-                    }, _r.lineEnd = function() {
-                        i(n, t)
-                    }
-                }
+        function e(t, e) {
+            n.moveTo(t, e), a.point = r
+        }
 
-                function Ar(n) {
-                    var t = 4.5,
-                        e = {
-                            point: r,
-                            lineStart: function() {
-                                e.point = i
-                            },
-                            lineEnd: o,
-                            polygonStart: function() {
-                                e.lineEnd = a
-                            },
-                            polygonEnd: function() {
-                                e.lineEnd = o, e.point = r
-                            },
-                            pointRadius: function(n) {
-                                return t = n, e
-                            },
-                            result: j
-                        };
+        function r(t, e) {
+            n.lineTo(t, e)
+        }
 
-                    function r(e, r) {
-                        n.moveTo(e + t, r), n.arc(e, r, t, 0, qn)
-                    }
+        function u() {
+            a.point = t
+        }
 
-                    function i(t, r) {
-                        n.moveTo(t, r), e.point = u
-                    }
+        function i() {
+            n.closePath()
+        }
+        var o = 4.5,
+            a = {
+                point: t,
+                lineStart: function() {
+                    a.point = e
+                },
+                lineEnd: u,
+                polygonStart: function() {
+                    a.lineEnd = i
+                },
+                polygonEnd: function() {
+                    a.lineEnd = u, a.point = t
+                },
+                pointRadius: function(n) {
+                    return o = n, a
+                },
+                result: y
+            };
+        return a
+    }
 
-                    function u(t, e) {
-                        n.lineTo(t, e)
-                    }
+    function nr(n) {
+        function t(n) {
+            return (a ? r : e)(n)
+        }
 
-                    function o() {
-                        e.point = r
-                    }
+        function e(t) {
+            return rr(t, function(e, r) {
+                e = n(e, r), t.point(e[0], e[1])
+            })
+        }
 
-                    function a() {
-                        n.closePath()
-                    }
-                    return e
+        function r(t) {
+            function e(e, r) {
+                e = n(e, r), t.point(e[0], e[1])
+            }
+
+            function r() {
+                x = 0 / 0, S.point = i, t.lineStart()
+            }
+
+            function i(e, r) {
+                var i = pe([e, r]),
+                    o = n(e, r);
+                u(x, M, y, _, b, w, x = o[0], M = o[1], y = e, _ = i[0], b = i[1], w = i[2], a, t), t.point(x, M)
+            }
+
+            function o() {
+                S.point = e, t.lineEnd()
+            }
+
+            function c() {
+                r(), S.point = l, S.lineEnd = s
+            }
+
+            function l(n, t) {
+                i(f = n, h = t), g = x, p = M, v = _, d = b, m = w, S.point = i
+            }
+
+            function s() {
+                u(x, M, y, _, b, w, g, p, f, v, d, m, a, t), S.lineEnd = o, o()
+            }
+            var f, h, g, p, v, d, m, y, x, M, _, b, w, S = {
+                point: e,
+                lineStart: r,
+                lineEnd: o,
+                polygonStart: function() {
+                    t.polygonStart(), S.lineStart = c
+                },
+                polygonEnd: function() {
+                    t.polygonEnd(), S.lineStart = r
                 }
+            };
+            return S
+        }
 
-                function Cr(n) {
-                    var t = .5,
-                        e = Math.cos(30 * Dn),
-                        r = 16;
+        function u(t, e, r, a, c, l, s, f, h, g, p, v, d, m) {
+            var y = s - t,
+                x = f - e,
+                M = y * y + x * x;
+            if (M > 4 * i && d--) {
+                var _ = a + g,
+                    b = c + p,
+                    w = l + v,
+                    S = Math.sqrt(_ * _ + b * b + w * w),
+                    k = Math.asin(w /= S),
+                    E = ca(ca(w) - 1) < Na || ca(r - h) < Na ? (r + h) / 2 : Math.atan2(b, _),
+                    A = n(E, k),
+                    C = A[0],
+                    N = A[1],
+                    z = C - t,
+                    L = N - e,
+                    T = x * z - y * L;
+                (T * T / M > i || ca((y * z + x * L) / M - .5) > .3 || o > a * g + c * p + l * v) && (u(t, e, r, a, c, l, C, N, E, _ /= S, b /= S, w, d, m), m.point(C, N), u(C, N, E, _, b, w, s, f, h, g, p, v, d, m))
+            }
+        }
+        var i = .5,
+            o = Math.cos(30 * La),
+            a = 16;
+        return t.precision = function(n) {
+            return arguments.length ? (a = (i = n * n) > 0 && 16, t) : Math.sqrt(i)
+        }, t
+    }
 
-                    function i(n) {
-                        return (r ? o : u)(n)
-                    }
+    function tr(n) {
+        var t = nr(function(t, e) {
+            return n([t * Ta, e * Ta])
+        });
+        return function(n) {
+            return or(t(n))
+        }
+    }
 
-                    function u(t) {
-                        return qr(t, (function(e, r) {
-                            e = n(e, r), t.point(e[0], e[1])
-                        }))
-                    }
+    function er(n) {
+        this.stream = n
+    }
 
-                    function o(t) {
-                        var e, i, u, o, l, c, f, s, h, p, g, v, d = {
-                            point: y,
-                            lineStart: m,
-                            lineEnd: x,
-                            polygonStart: function() {
-                                t.polygonStart(), d.lineStart = b
-                            },
-                            polygonEnd: function() {
-                                t.polygonEnd(), d.lineStart = m
-                            }
-                        };
+    function rr(n, t) {
+        return {
+            point: t,
+            sphere: function() {
+                n.sphere()
+            },
+            lineStart: function() {
+                n.lineStart()
+            },
+            lineEnd: function() {
+                n.lineEnd()
+            },
+            polygonStart: function() {
+                n.polygonStart()
+            },
+            polygonEnd: function() {
+                n.polygonEnd()
+            }
+        }
+    }
 
-                        function y(e, r) {
-                            e = n(e, r), t.point(e[0], e[1])
-                        }
+    function ur(n) {
+        return ir(function() {
+            return n
+        })()
+    }
 
-                        function m() {
-                            s = NaN, d.point = M, t.lineStart()
-                        }
+    function ir(n) {
+        function t(n) {
+            return n = a(n[0] * La, n[1] * La), [n[0] * h + c, l - n[1] * h]
+        }
 
-                        function M(e, i) {
-                            var u = Pe([e, i]),
-                                o = n(e, i);
-                            a(s, h, f, p, g, v, s = o[0], h = o[1], f = e, p = u[0], g = u[1], v = u[2], r, t), t.point(s, h)
-                        }
+        function e(n) {
+            return n = a.invert((n[0] - c) / h, (l - n[1]) / h), n && [n[0] * Ta, n[1] * Ta]
+        }
 
-                        function x() {
-                            d.point = y, t.lineEnd()
-                        }
+        function r() {
+            a = Ye(o = lr(m, y, x), i);
+            var n = i(v, d);
+            return c = g - n[0] * h, l = p + n[1] * h, u()
+        }
 
-                        function b() {
-                            m(), d.point = w, d.lineEnd = _
-                        }
+        function u() {
+            return s && (s.valid = !1, s = null), t
+        }
+        var i, o, a, c, l, s, f = nr(function(n, t) {
+                return n = i(n, t), [n[0] * h + c, l - n[1] * h]
+            }),
+            h = 150,
+            g = 480,
+            p = 250,
+            v = 0,
+            d = 0,
+            m = 0,
+            y = 0,
+            x = 0,
+            M = Cc,
+            _ = Et,
+            b = null,
+            w = null;
+        return t.stream = function(n) {
+                return s && (s.valid = !1), s = or(M(o, f(_(n)))), s.valid = !0, s
+            }, t.clipAngle = function(n) {
+                return arguments.length ? (M = null == n ? (b = n, Cc) : Fe((b = +n) * La), u()) : b
+            }, t.clipExtent = function(n) {
+                return arguments.length ? (w = n, _ = n ? Oe(n[0][0], n[0][1], n[1][0], n[1][1]) : Et, u()) : w
+            }, t.scale = function(n) {
+                return arguments.length ? (h = +n, r()) : h
+            }, t.translate = function(n) {
+                return arguments.length ? (g = +n[0], p = +n[1], r()) : [g, p]
+            }, t.center = function(n) {
+                return arguments.length ? (v = n[0] % 360 * La, d = n[1] % 360 * La, r()) : [v * Ta, d * Ta]
+            }, t.rotate = function(n) {
+                return arguments.length ? (m = n[0] % 360 * La, y = n[1] % 360 * La, x = n.length > 2 ? n[2] % 360 * La : 0, r()) : [m * Ta, y * Ta, x * Ta]
+            }, Bo.rebind(t, f, "precision"),
+            function() {
+                return i = n.apply(this, arguments), t.invert = i.invert && e, r()
+            }
+    }
 
-                        function w(n, t) {
-                            M(e = n, t), i = s, u = h, o = p, l = g, c = v, d.point = M
-                        }
+    function or(n) {
+        return rr(n, function(t, e) {
+            n.point(t * La, e * La)
+        })
+    }
 
-                        function _() {
-                            a(s, h, f, p, g, v, i, u, e, o, l, c, r, t), d.lineEnd = x, x()
-                        }
-                        return d
-                    }
+    function ar(n, t) {
+        return [n, t]
+    }
 
-                    function a(r, i, u, o, l, c, f, s, h, p, g, v, d, y) {
-                        var m = f - r,
-                            M = s - i,
-                            x = m * m + M * M;
-                        if (x > 4 * t && d--) {
-                            var b = o + p,
-                                _ = l + g,
-                                k = c + v,
-                                S = Math.sqrt(b * b + _ * _ + k * k),
-                                N = Math.asin(k /= S),
-                                E = w(w(k) - 1) < Cn || w(u - h) < Cn ? (u + h) / 2 : Math.atan2(_, b),
-                                A = n(E, N),
-                                C = A[0],
-                                z = A[1],
-                                L = C - r,
-                                q = z - i,
-                                T = M * L - m * q;
-                            (T * T / x > t || w((m * L + M * q) / x - .5) > .3 || o * p + l * g + c * v < e) && (a(r, i, u, o, l, c, C, z, E, b /= S, _ /= S, k, d, y), y.point(C, z), a(C, z, E, b, _, k, f, s, h, p, g, v, d, y))
-                        }
-                    }
-                    return i.precision = function(n) {
-                        return arguments.length ? (r = (t = n * n) > 0 && 16, i) : Math.sqrt(t)
-                    }, i
-                }
+    function cr(n, t) {
+        return [n > Ea ? n - Aa : -Ea > n ? n + Aa : n, t]
+    }
 
-                function zr(n) {
-                    var t = Cr((function(t, e) {
-                        return n([t * Pn, e * Pn])
-                    }));
-                    return function(n) {
-                        return Dr(t(n))
-                    }
-                }
+    function lr(n, t, e) {
+        return n ? t || e ? Ye(fr(n), hr(t, e)) : fr(n) : t || e ? hr(t, e) : cr
+    }
 
-                function Lr(n) {
-                    this.stream = n
-                }
+    function sr(n) {
+        return function(t, e) {
+            return t += n, [t > Ea ? t - Aa : -Ea > t ? t + Aa : t, e]
+        }
+    }
 
-                function qr(n, t) {
-                    return {
-                        point: t,
-                        sphere: function() {
-                            n.sphere()
-                        },
-                        lineStart: function() {
-                            n.lineStart()
-                        },
-                        lineEnd: function() {
-                            n.lineEnd()
-                        },
-                        polygonStart: function() {
-                            n.polygonStart()
-                        },
-                        polygonEnd: function() {
-                            n.polygonEnd()
-                        }
-                    }
-                }
+    function fr(n) {
+        var t = sr(n);
+        return t.invert = sr(-n), t
+    }
 
-                function Tr(n) {
-                    return Rr((function() {
-                        return n
-                    }))()
-                }
-
-                function Rr(n) {
-                    var t, e, r, i, o, a, l = Cr((function(n, e) {
-                            return [(n = t(n, e))[0] * c + i, o - n[1] * c]
-                        })),
-                        c = 150,
-                        f = 480,
-                        s = 250,
-                        h = 0,
-                        p = 0,
-                        g = 0,
-                        v = 0,
-                        d = 0,
-                        y = ur,
-                        m = R,
-                        M = null,
-                        x = null;
+    function hr(n, t) {
+        function e(n, t) {
+            var e = Math.cos(t),
+                a = Math.cos(n) * e,
+                c = Math.sin(n) * e,
+                l = Math.sin(t),
+                s = l * r + a * u;
+            return [Math.atan2(c * i - s * o, a * r - l * u), nt(s * i + c * o)]
+        }
+        var r = Math.cos(n),
+            u = Math.sin(n),
+            i = Math.cos(t),
+            o = Math.sin(t);
+        return e.invert = function(n, t) {
+            var e = Math.cos(t),
+                a = Math.cos(n) * e,
+                c = Math.sin(n) * e,
+                l = Math.sin(t),
+                s = l * i - c * o;
+            return [Math.atan2(c * i + l * o, a * r + s * u), nt(s * r - a * u)]
+        }, e
+    }
 
-                    function b(n) {
-                        return [(n = r(n[0] * Dn, n[1] * Dn))[0] * c + i, o - n[1] * c]
-                    }
+    function gr(n, t) {
+        var e = Math.cos(n),
+            r = Math.sin(n);
+        return function(u, i, o, a) {
+            var c = o * t;
+            null != u ? (u = pr(e, u), i = pr(e, i), (o > 0 ? i > u : u > i) && (u += o * Aa)) : (u = n + o * Aa, i = n - .5 * c);
+            for (var l, s = u; o > 0 ? s > i : i > s; s -= c) a.point((l = Me([e, -r * Math.cos(s), -r * Math.sin(s)]))[0], l[1])
+        }
+    }
 
-                    function w(n) {
-                        return (n = r.invert((n[0] - i) / c, (o - n[1]) / c)) && [n[0] * Pn, n[1] * Pn]
-                    }
+    function pr(n, t) {
+        var e = pe(t);
+        e[0] -= n, xe(e);
+        var r = Q(-e[1]);
+        return ((-e[2] < 0 ? -r : r) + 2 * Math.PI - Na) % (2 * Math.PI)
+    }
 
-                    function _() {
-                        r = We(e = jr(g, v, d), t);
-                        var n = t(h, p);
-                        return i = f - n[0] * c, o = s + n[1] * c, k()
-                    }
+    function vr(n, t, e) {
+        var r = Bo.range(n, t - Na, e).concat(t);
+        return function(n) {
+            return r.map(function(t) {
+                return [n, t]
+            })
+        }
+    }
 
-                    function k() {
-                        return a && (a.valid = !1, a = null), b
-                    }
-                    return b.stream = function(n) {
-                            return a && (a.valid = !1), (a = Dr(y(e, l(m(n))))).valid = !0, a
-                        }, b.clipAngle = function(n) {
-                            return arguments.length ? (y = null == n ? (M = n, ur) : or((M = +n) * Dn), k()) : M
-                        }, b.clipExtent = function(n) {
-                            return arguments.length ? (x = n, m = n ? lr(n[0][0], n[0][1], n[1][0], n[1][1]) : R, k()) : x
-                        }, b.scale = function(n) {
-                            return arguments.length ? (c = +n, _()) : c
-                        }, b.translate = function(n) {
-                            return arguments.length ? (f = +n[0], s = +n[1], _()) : [f, s]
-                        }, b.center = function(n) {
-                            return arguments.length ? (h = n[0] % 360 * Dn, p = n[1] % 360 * Dn, _()) : [h * Pn, p * Pn]
-                        }, b.rotate = function(n) {
-                            return arguments.length ? (g = n[0] % 360 * Dn, v = n[1] % 360 * Dn, d = n.length > 2 ? n[2] % 360 * Dn : 0, _()) : [g * Pn, v * Pn, d * Pn]
-                        }, u.rebind(b, l, "precision"),
-                        function() {
-                            return t = n.apply(this, arguments), b.invert = t.invert && w, _()
-                        }
-                }
+    function dr(n, t, e) {
+        var r = Bo.range(n, t - Na, e).concat(t);
+        return function(n) {
+            return r.map(function(t) {
+                return [t, n]
+            })
+        }
+    }
 
-                function Dr(n) {
-                    return qr(n, (function(t, e) {
-                        n.point(t * Dn, e * Dn)
-                    }))
-                }
+    function mr(n) {
+        return n.source
+    }
 
-                function Pr(n, t) {
-                    return [n, t]
-                }
+    function yr(n) {
+        return n.target
+    }
 
-                function Ur(n, t) {
-                    return [n > Ln ? n - qn : n < -Ln ? n + qn : n, t]
-                }
+    function xr(n, t, e, r) {
+        var u = Math.cos(t),
+            i = Math.sin(t),
+            o = Math.cos(r),
+            a = Math.sin(r),
+            c = u * Math.cos(n),
+            l = u * Math.sin(n),
+            s = o * Math.cos(e),
+            f = o * Math.sin(e),
+            h = 2 * Math.asin(Math.sqrt(ut(r - t) + u * o * ut(e - n))),
+            g = 1 / Math.sin(h),
+            p = h ? function(n) {
+                var t = Math.sin(n *= h) * g,
+                    e = Math.sin(h - n) * g,
+                    r = e * c + t * s,
+                    u = e * l + t * f,
+                    o = e * i + t * a;
+                return [Math.atan2(u, r) * Ta, Math.atan2(o, Math.sqrt(r * r + u * u)) * Ta]
+            } : function() {
+                return [n * Ta, t * Ta]
+            };
+        return p.distance = h, p
+    }
 
-                function jr(n, t, e) {
-                    return n ? t || e ? We(Hr(n), Or(t, e)) : Hr(n) : t || e ? Or(t, e) : Ur
-                }
+    function Mr() {
+        function n(n, u) {
+            var i = Math.sin(u *= La),
+                o = Math.cos(u),
+                a = ca((n *= La) - t),
+                c = Math.cos(a);
+            Fc += Math.atan2(Math.sqrt((a = o * Math.sin(a)) * a + (a = r * i - e * o * c) * a), e * i + r * o * c), t = n, e = i, r = o
+        }
+        var t, e, r;
+        Hc.point = function(u, i) {
+            t = u * La, e = Math.sin(i *= La), r = Math.cos(i), Hc.point = n
+        }, Hc.lineEnd = function() {
+            Hc.point = Hc.lineEnd = y
+        }
+    }
 
-                function Fr(n) {
-                    return function(t, e) {
-                        return [(t += n) > Ln ? t - qn : t < -Ln ? t + qn : t, e]
-                    }
-                }
+    function _r(n, t) {
+        function e(t, e) {
+            var r = Math.cos(t),
+                u = Math.cos(e),
+                i = n(r * u);
+            return [i * u * Math.sin(t), i * Math.sin(e)]
+        }
+        return e.invert = function(n, e) {
+            var r = Math.sqrt(n * n + e * e),
+                u = t(r),
+                i = Math.sin(u),
+                o = Math.cos(u);
+            return [Math.atan2(n * i, r * o), Math.asin(r && e * i / r)]
+        }, e
+    }
 
-                function Hr(n) {
-                    var t = Fr(n);
-                    return t.invert = Fr(-n), t
-                }
-
-                function Or(n, t) {
-                    var e = Math.cos(n),
-                        r = Math.sin(n),
-                        i = Math.cos(t),
-                        u = Math.sin(t);
-
-                    function o(n, t) {
-                        var o = Math.cos(t),
-                            a = Math.cos(n) * o,
-                            l = Math.sin(n) * o,
-                            c = Math.sin(t),
-                            f = c * e + a * r;
-                        return [Math.atan2(l * i - f * u, a * e - c * r), Hn(f * i + l * u)]
-                    }
-                    return o.invert = function(n, t) {
-                        var o = Math.cos(t),
-                            a = Math.cos(n) * o,
-                            l = Math.sin(n) * o,
-                            c = Math.sin(t),
-                            f = c * i - l * u;
-                        return [Math.atan2(l * i + c * u, a * e + f * r), Hn(f * e - a * r)]
-                    }, o
-                }
-
-                function Ir(n, t) {
-                    var e = Math.cos(n),
-                        r = Math.sin(n);
-                    return function(i, u, o, a) {
-                        var l = o * t;
-                        null != i ? (i = Yr(e, i), u = Yr(e, u), (o > 0 ? i < u : i > u) && (i += o * qn)) : (i = n + o * qn, u = n - .5 * l);
-                        for (var c, f = i; o > 0 ? f > u : f < u; f -= l) a.point((c = Ie([e, -r * Math.cos(f), -r * Math.sin(f)]))[0], c[1])
-                    }
-                }
+    function br(n, t) {
+        function e(n, t) {
+            o > 0 ? -Ca + Na > t && (t = -Ca + Na) : t > Ca - Na && (t = Ca - Na);
+            var e = o / Math.pow(u(t), i);
+            return [e * Math.sin(i * n), o - e * Math.cos(i * n)]
+        }
+        var r = Math.cos(n),
+            u = function(n) {
+                return Math.tan(Ea / 4 + n / 2)
+            },
+            i = n === t ? Math.sin(n) : Math.log(r / Math.cos(t)) / Math.log(u(t) / u(n)),
+            o = r * Math.pow(u(n), i) / i;
+        return i ? (e.invert = function(n, t) {
+            var e = o - t,
+                r = G(i) * Math.sqrt(n * n + e * e);
+            return [Math.atan2(n, e) / i, 2 * Math.atan(Math.pow(o / r, 1 / i)) - Ca]
+        }, e) : Sr
+    }
 
-                function Yr(n, t) {
-                    var e = Pe(t);
-                    e[0] -= n, Oe(e);
-                    var r = Fn(-e[1]);
-                    return ((-e[2] < 0 ? -r : r) + 2 * Math.PI - Cn) % (2 * Math.PI)
-                }
+    function wr(n, t) {
+        function e(n, t) {
+            var e = i - t;
+            return [e * Math.sin(u * n), i - e * Math.cos(u * n)]
+        }
+        var r = Math.cos(n),
+            u = n === t ? Math.sin(n) : (r - Math.cos(t)) / (t - n),
+            i = r / u + n;
+        return ca(u) < Na ? ar : (e.invert = function(n, t) {
+            var e = i - t;
+            return [Math.atan2(n, e) / u, i - G(u) * Math.sqrt(n * n + e * e)]
+        }, e)
+    }
 
-                function Zr(n, t, e) {
-                    var r = u.range(n, t - Cn, e).concat(t);
-                    return function(n) {
-                        return r.map((function(t) {
-                            return [n, t]
-                        }))
-                    }
-                }
+    function Sr(n, t) {
+        return [n, Math.log(Math.tan(Ea / 4 + t / 2))]
+    }
 
-                function Vr(n, t, e) {
-                    var r = u.range(n, t - Cn, e).concat(t);
-                    return function(n) {
-                        return r.map((function(t) {
-                            return [t, n]
-                        }))
-                    }
+    function kr(n) {
+        var t, e = ur(n),
+            r = e.scale,
+            u = e.translate,
+            i = e.clipExtent;
+        return e.scale = function() {
+            var n = r.apply(e, arguments);
+            return n === e ? t ? e.clipExtent(null) : e : n
+        }, e.translate = function() {
+            var n = u.apply(e, arguments);
+            return n === e ? t ? e.clipExtent(null) : e : n
+        }, e.clipExtent = function(n) {
+            var o = i.apply(e, arguments);
+            if (o === e) {
+                if (t = null == n) {
+                    var a = Ea * r(),
+                        c = u();
+                    i([
+                        [c[0] - a, c[1] - a],
+                        [c[0] + a, c[1] + a]
+                    ])
                 }
+            } else t && (o = null);
+            return o
+        }, e.clipExtent(null)
+    }
 
-                function Xr(n) {
-                    return n.source
-                }
+    function Er(n, t) {
+        return [Math.log(Math.tan(Ea / 4 + t / 2)), -n]
+    }
 
-                function $r(n) {
-                    return n.target
-                }
-                u.geo.path = function() {
-                    var n, t, e, r, i, o = 4.5;
+    function Ar(n) {
+        return n[0]
+    }
 
-                    function a(n) {
-                        return n && ("function" == typeof o && r.pointRadius(+o.apply(this, arguments)), i && i.valid || (i = e(r)), u.geo.stream(n, i)), r.result()
-                    }
+    function Cr(n) {
+        return n[1]
+    }
 
-                    function l() {
-                        return i = null, a
-                    }
-                    return a.area = function(n) {
-                        return sr = 0, u.geo.stream(n, e(yr)), sr
-                    }, a.centroid = function(n) {
-                        return ke = Se = Ne = Ee = Ae = Ce = ze = Le = qe = 0, u.geo.stream(n, e(_r)), qe ? [ze / qe, Le / qe] : Ce ? [Ee / Ce, Ae / Ce] : Ne ? [ke / Ne, Se / Ne] : [NaN, NaN]
-                    }, a.bounds = function(n) {
-                        return vr = dr = -(pr = gr = 1 / 0), u.geo.stream(n, e(Mr)), [
-                            [pr, gr],
-                            [vr, dr]
-                        ]
-                    }, a.projection = function(t) {
-                        return arguments.length ? (e = (n = t) ? t.stream || zr(t) : R, l()) : n
-                    }, a.context = function(n) {
-                        return arguments.length ? (r = null == (t = n) ? new xr : new Ar(n), "function" != typeof o && r.pointRadius(o), l()) : t
-                    }, a.pointRadius = function(n) {
-                        return arguments.length ? (o = "function" == typeof n ? n : (r.pointRadius(+n), +n), a) : o
-                    }, a.projection(u.geo.albersUsa()).context(null)
-                }, u.geo.transform = function(n) {
-                    return {
-                        stream: function(t) {
-                            var e = new Lr(t);
-                            for (var r in n) e[r] = n[r];
-                            return e
-                        }
-                    }
-                }, Lr.prototype = {
-                    point: function(n, t) {
-                        this.stream.point(n, t)
-                    },
-                    sphere: function() {
-                        this.stream.sphere()
-                    },
-                    lineStart: function() {
-                        this.stream.lineStart()
-                    },
-                    lineEnd: function() {
-                        this.stream.lineEnd()
-                    },
-                    polygonStart: function() {
-                        this.stream.polygonStart()
-                    },
-                    polygonEnd: function() {
-                        this.stream.polygonEnd()
-                    }
-                }, u.geo.projection = Tr, u.geo.projectionMutator = Rr, (u.geo.equirectangular = function() {
-                    return Tr(Pr)
-                }).raw = Pr.invert = Pr, u.geo.rotation = function(n) {
-                    function t(t) {
-                        return (t = n(t[0] * Dn, t[1] * Dn))[0] *= Pn, t[1] *= Pn, t
-                    }
-                    return n = jr(n[0] % 360 * Dn, n[1] * Dn, n.length > 2 ? n[2] * Dn : 0), t.invert = function(t) {
-                        return (t = n.invert(t[0] * Dn, t[1] * Dn))[0] *= Pn, t[1] *= Pn, t
-                    }, t
-                }, Ur.invert = Pr, u.geo.circle = function() {
-                    var n, t, e = [0, 0],
-                        r = 6;
-
-                    function i() {
-                        var n = "function" == typeof e ? e.apply(this, arguments) : e,
-                            r = jr(-n[0] * Dn, -n[1] * Dn, 0).invert,
-                            i = [];
-                        return t(null, null, 1, {
-                            point: function(n, t) {
-                                i.push(n = r(n, t)), n[0] *= Pn, n[1] *= Pn
-                            }
-                        }), {
-                            type: "Polygon",
-                            coordinates: [i]
-                        }
-                    }
-                    return i.origin = function(n) {
-                        return arguments.length ? (e = n, i) : e
-                    }, i.angle = function(e) {
-                        return arguments.length ? (t = Ir((n = +e) * Dn, r * Dn), i) : n
-                    }, i.precision = function(e) {
-                        return arguments.length ? (t = Ir(n * Dn, (r = +e) * Dn), i) : r
-                    }, i.angle(90)
-                }, u.geo.distance = function(n, t) {
-                    var e, r = (t[0] - n[0]) * Dn,
-                        i = n[1] * Dn,
-                        u = t[1] * Dn,
-                        o = Math.sin(r),
-                        a = Math.cos(r),
-                        l = Math.sin(i),
-                        c = Math.cos(i),
-                        f = Math.sin(u),
-                        s = Math.cos(u);
-                    return Math.atan2(Math.sqrt((e = s * o) * e + (e = c * f - l * s * a) * e), l * f + c * s * a)
-                }, u.geo.graticule = function() {
-                    var n, t, e, r, i, o, a, l, c, f, s, h, p = 10,
-                        g = p,
-                        v = 90,
-                        d = 360,
-                        y = 2.5;
-
-                    function m() {
-                        return {
-                            type: "MultiLineString",
-                            coordinates: M()
-                        }
-                    }
+    function Nr(n) {
+        for (var t = n.length, e = [0, 1], r = 2, u = 2; t > u; u++) {
+            for (; r > 1 && K(n[e[r - 2]], n[e[r - 1]], n[u]) <= 0;) --r;
+            e[r++] = u
+        }
+        return e.slice(0, r)
+    }
 
-                    function M() {
-                        return u.range(Math.ceil(r / v) * v, e, v).map(s).concat(u.range(Math.ceil(l / d) * d, a, d).map(h)).concat(u.range(Math.ceil(t / p) * p, n, p).filter((function(n) {
-                            return w(n % v) > Cn
-                        })).map(c)).concat(u.range(Math.ceil(o / g) * g, i, g).filter((function(n) {
-                            return w(n % d) > Cn
-                        })).map(f))
-                    }
-                    return m.lines = function() {
-                        return M().map((function(n) {
-                            return {
-                                type: "LineString",
-                                coordinates: n
-                            }
-                        }))
-                    }, m.outline = function() {
-                        return {
-                            type: "Polygon",
-                            coordinates: [s(r).concat(h(a).slice(1), s(e).reverse().slice(1), h(l).reverse().slice(1))]
-                        }
-                    }, m.extent = function(n) {
-                        return arguments.length ? m.majorExtent(n).minorExtent(n) : m.minorExtent()
-                    }, m.majorExtent = function(n) {
-                        return arguments.length ? (r = +n[0][0], e = +n[1][0], l = +n[0][1], a = +n[1][1], r > e && (n = r, r = e, e = n), l > a && (n = l, l = a, a = n), m.precision(y)) : [
-                            [r, l],
-                            [e, a]
-                        ]
-                    }, m.minorExtent = function(e) {
-                        return arguments.length ? (t = +e[0][0], n = +e[1][0], o = +e[0][1], i = +e[1][1], t > n && (e = t, t = n, n = e), o > i && (e = o, o = i, i = e), m.precision(y)) : [
-                            [t, o],
-                            [n, i]
-                        ]
-                    }, m.step = function(n) {
-                        return arguments.length ? m.majorStep(n).minorStep(n) : m.minorStep()
-                    }, m.majorStep = function(n) {
-                        return arguments.length ? (v = +n[0], d = +n[1], m) : [v, d]
-                    }, m.minorStep = function(n) {
-                        return arguments.length ? (p = +n[0], g = +n[1], m) : [p, g]
-                    }, m.precision = function(u) {
-                        return arguments.length ? (y = +u, c = Zr(o, i, 90), f = Vr(t, n, y), s = Zr(l, a, 90), h = Vr(r, e, y), m) : y
-                    }, m.majorExtent([
-                        [-180, -90 + Cn],
-                        [180, 90 - Cn]
-                    ]).minorExtent([
-                        [-180, -80 - Cn],
-                        [180, 80 + Cn]
-                    ])
-                }, u.geo.greatArc = function() {
-                    var n, t, e = Xr,
-                        r = $r;
-
-                    function i() {
-                        return {
-                            type: "LineString",
-                            coordinates: [n || e.apply(this, arguments), t || r.apply(this, arguments)]
-                        }
-                    }
-                    return i.distance = function() {
-                        return u.geo.distance(n || e.apply(this, arguments), t || r.apply(this, arguments))
-                    }, i.source = function(t) {
-                        return arguments.length ? (e = t, n = "function" == typeof t ? null : t, i) : e
-                    }, i.target = function(n) {
-                        return arguments.length ? (r = n, t = "function" == typeof n ? null : n, i) : r
-                    }, i.precision = function() {
-                        return arguments.length ? i : 0
-                    }, i
-                }, u.geo.interpolate = function(n, t) {
-                    return e = n[0] * Dn, r = n[1] * Dn, i = t[0] * Dn, u = t[1] * Dn, o = Math.cos(r), a = Math.sin(r), l = Math.cos(u), c = Math.sin(u), f = o * Math.cos(e), s = o * Math.sin(e), h = l * Math.cos(i), p = l * Math.sin(i), g = 2 * Math.asin(Math.sqrt(In(u - r) + o * l * In(i - e))), v = 1 / Math.sin(g), (d = g ? function(n) {
-                        var t = Math.sin(n *= g) * v,
-                            e = Math.sin(g - n) * v,
-                            r = e * f + t * h,
-                            i = e * s + t * p,
-                            u = e * a + t * c;
-                        return [Math.atan2(i, r) * Pn, Math.atan2(u, Math.sqrt(r * r + i * i)) * Pn]
-                    } : function() {
-                        return [e * Pn, r * Pn]
-                    }).distance = g, d;
-                    var e, r, i, u, o, a, l, c, f, s, h, p, g, v, d
-                }, u.geo.length = function(n) {
-                    return wr = 0, u.geo.stream(n, Br), wr
-                };
-                var Br = {
-                    sphere: j,
-                    point: j,
-                    lineStart: function() {
-                        var n, t, e;
-
-                        function r(r, i) {
-                            var u = Math.sin(i *= Dn),
-                                o = Math.cos(i),
-                                a = w((r *= Dn) - n),
-                                l = Math.cos(a);
-                            wr += Math.atan2(Math.sqrt((a = o * Math.sin(a)) * a + (a = e * u - t * o * l) * a), t * u + e * o * l), n = r, t = u, e = o
-                        }
-                        Br.point = function(i, u) {
-                            n = i * Dn, t = Math.sin(u *= Dn), e = Math.cos(u), Br.point = r
-                        }, Br.lineEnd = function() {
-                            Br.point = Br.lineEnd = j
-                        }
-                    },
-                    lineEnd: j,
-                    polygonStart: j,
-                    polygonEnd: j
-                };
+    function zr(n, t) {
+        return n[0] - t[0] || n[1] - t[1]
+    }
 
-                function Jr(n, t) {
-                    function e(t, e) {
-                        var r = Math.cos(t),
-                            i = Math.cos(e),
-                            u = n(r * i);
-                        return [u * i * Math.sin(t), u * Math.sin(e)]
-                    }
-                    return e.invert = function(n, e) {
-                        var r = Math.sqrt(n * n + e * e),
-                            i = t(r),
-                            u = Math.sin(i),
-                            o = Math.cos(i);
-                        return [Math.atan2(n * u, r * o), Math.asin(r && e * u / r)]
-                    }, e
-                }
-                var Wr = Jr((function(n) {
-                    return Math.sqrt(2 / (1 + n))
-                }), (function(n) {
-                    return 2 * Math.asin(n / 2)
-                }));
-                (u.geo.azimuthalEqualArea = function() {
-                    return Tr(Wr)
-                }).raw = Wr;
-                var Gr = Jr((function(n) {
-                    var t = Math.acos(n);
-                    return t && t / Math.sin(t)
-                }), R);
-
-                function Kr(n, t) {
-                    var e = Math.cos(n),
-                        r = function(n) {
-                            return Math.tan(Ln / 4 + n / 2)
-                        },
-                        i = n === t ? Math.sin(n) : Math.log(e / Math.cos(t)) / Math.log(r(t) / r(n)),
-                        u = e * Math.pow(r(n), i) / i;
-                    if (!i) return ti;
-
-                    function o(n, t) {
-                        u > 0 ? t < -Rn + Cn && (t = -Rn + Cn) : t > Rn - Cn && (t = Rn - Cn);
-                        var e = u / Math.pow(r(t), i);
-                        return [e * Math.sin(i * n), u - e * Math.cos(i * n)]
-                    }
-                    return o.invert = function(n, t) {
-                        var e = u - t,
-                            r = Un(i) * Math.sqrt(n * n + e * e);
-                        return [Math.atan2(n, e) / i, 2 * Math.atan(Math.pow(u / r, 1 / i)) - Rn]
-                    }, o
-                }
-
-                function Qr(n, t) {
-                    var e = Math.cos(n),
-                        r = n === t ? Math.sin(n) : (e - Math.cos(t)) / (t - n),
-                        i = e / r + n;
-                    if (w(r) < Cn) return Pr;
-
-                    function u(n, t) {
-                        var e = i - t;
-                        return [e * Math.sin(r * n), i - e * Math.cos(r * n)]
-                    }
-                    return u.invert = function(n, t) {
-                        var e = i - t;
-                        return [Math.atan2(n, e) / r, i - Un(r) * Math.sqrt(n * n + e * e)]
-                    }, u
-                }(u.geo.azimuthalEquidistant = function() {
-                    return Tr(Gr)
-                }).raw = Gr, (u.geo.conicConformal = function() {
-                    return cr(Kr)
-                }).raw = Kr, (u.geo.conicEquidistant = function() {
-                    return cr(Qr)
-                }).raw = Qr;
-                var ni = Jr((function(n) {
-                    return 1 / n
-                }), Math.atan);
-
-                function ti(n, t) {
-                    return [n, Math.log(Math.tan(Ln / 4 + t / 2))]
-                }
-
-                function ei(n) {
-                    var t, e = Tr(n),
-                        r = e.scale,
-                        i = e.translate,
-                        u = e.clipExtent;
-                    return e.scale = function() {
-                        var n = r.apply(e, arguments);
-                        return n === e ? t ? e.clipExtent(null) : e : n
-                    }, e.translate = function() {
-                        var n = i.apply(e, arguments);
-                        return n === e ? t ? e.clipExtent(null) : e : n
-                    }, e.clipExtent = function(n) {
-                        var o = u.apply(e, arguments);
-                        if (o === e) {
-                            if (t = null == n) {
-                                var a = Ln * r(),
-                                    l = i();
-                                u([
-                                    [l[0] - a, l[1] - a],
-                                    [l[0] + a, l[1] + a]
-                                ])
-                            }
-                        } else t && (o = null);
-                        return o
-                    }, e.clipExtent(null)
-                }(u.geo.gnomonic = function() {
-                    return Tr(ni)
-                }).raw = ni, ti.invert = function(n, t) {
-                    return [n, 2 * Math.atan(Math.exp(t)) - Rn]
-                }, (u.geo.mercator = function() {
-                    return ei(ti)
-                }).raw = ti;
-                var ri = Jr((function() {
-                    return 1
-                }), Math.asin);
-                (u.geo.orthographic = function() {
-                    return Tr(ri)
-                }).raw = ri;
-                var ii = Jr((function(n) {
-                    return 1 / (1 + n)
-                }), (function(n) {
-                    return 2 * Math.atan(n)
-                }));
-
-                function ui(n, t) {
-                    return [Math.log(Math.tan(Ln / 4 + t / 2)), -n]
-                }
-
-                function oi(n) {
-                    return n[0]
-                }
-
-                function ai(n) {
-                    return n[1]
-                }
-
-                function li(n) {
-                    for (var t = n.length, e = [0, 1], r = 2, i = 2; i < t; i++) {
-                        for (; r > 1 && jn(n[e[r - 2]], n[e[r - 1]], n[i]) <= 0;) --r;
-                        e[r++] = i
-                    }
-                    return e.slice(0, r)
-                }
+    function Lr(n, t, e) {
+        return (e[0] - t[0]) * (n[1] - t[1]) < (e[1] - t[1]) * (n[0] - t[0])
+    }
 
-                function ci(n, t) {
-                    return n[0] - t[0] || n[1] - t[1]
-                }(u.geo.stereographic = function() {
-                    return Tr(ii)
-                }).raw = ii, ui.invert = function(n, t) {
-                    return [-t, 2 * Math.atan(Math.exp(n)) - Rn]
-                }, (u.geo.transverseMercator = function() {
-                    var n = ei(ui),
-                        t = n.center,
-                        e = n.rotate;
-                    return n.center = function(n) {
-                        return n ? t([-n[1], n[0]]) : [(n = t())[1], -n[0]]
-                    }, n.rotate = function(n) {
-                        return n ? e([n[0], n[1], n.length > 2 ? n[2] + 90 : 90]) : [(n = e())[0], n[1], n[2] - 90]
-                    }, e([0, 0, 90])
-                }).raw = ui, u.geom = {}, u.geom.hull = function(n) {
-                    var t = oi,
-                        e = ai;
-                    if (arguments.length) return r(n);
-
-                    function r(n) {
-                        if (n.length < 3) return [];
-                        var r, i = Mt(t),
-                            u = Mt(e),
-                            o = n.length,
-                            a = [],
-                            l = [];
-                        for (r = 0; r < o; r++) a.push([+i.call(this, n[r], r), +u.call(this, n[r], r), r]);
-                        for (a.sort(ci), r = 0; r < o; r++) l.push([a[r][0], -a[r][1]]);
-                        var c = li(a),
-                            f = li(l),
-                            s = f[0] === c[0],
-                            h = f[f.length - 1] === c[c.length - 1],
-                            p = [];
-                        for (r = c.length - 1; r >= 0; --r) p.push(n[a[c[r]][2]]);
-                        for (r = +s; r < f.length - h; ++r) p.push(n[a[f[r]][2]]);
-                        return p
-                    }
-                    return r.x = function(n) {
-                        return arguments.length ? (t = n, r) : t
-                    }, r.y = function(n) {
-                        return arguments.length ? (e = n, r) : e
-                    }, r
-                }, u.geom.polygon = function(n) {
-                    return V(n, fi), n
-                };
-                var fi = u.geom.polygon.prototype = [];
+    function Tr(n, t, e, r) {
+        var u = n[0],
+            i = e[0],
+            o = t[0] - u,
+            a = r[0] - i,
+            c = n[1],
+            l = e[1],
+            s = t[1] - c,
+            f = r[1] - l,
+            h = (a * (c - l) - f * (u - i)) / (f * o - a * s);
+        return [u + h * o, c + h * s]
+    }
 
-                function si(n, t, e) {
-                    return (e[0] - t[0]) * (n[1] - t[1]) < (e[1] - t[1]) * (n[0] - t[0])
-                }
+    function qr(n) {
+        var t = n[0],
+            e = n[n.length - 1];
+        return !(t[0] - e[0] || t[1] - e[1])
+    }
 
-                function hi(n, t, e, r) {
-                    var i = n[0],
-                        u = e[0],
-                        o = t[0] - i,
-                        a = r[0] - u,
-                        l = n[1],
-                        c = e[1],
-                        f = t[1] - l,
-                        s = r[1] - c,
-                        h = (a * (l - c) - s * (i - u)) / (s * o - a * f);
-                    return [i + h * o, l + h * f]
-                }
-
-                function pi(n) {
-                    var t = n[0],
-                        e = n[n.length - 1];
-                    return !(t[0] - e[0] || t[1] - e[1])
-                }
-                fi.area = function() {
-                    for (var n, t = -1, e = this.length, r = this[e - 1], i = 0; ++t < e;) n = r, r = this[t], i += n[1] * r[0] - n[0] * r[1];
-                    return .5 * i
-                }, fi.centroid = function(n) {
-                    var t, e, r = -1,
-                        i = this.length,
-                        u = 0,
-                        o = 0,
-                        a = this[i - 1];
-                    for (arguments.length || (n = -1 / (6 * this.area())); ++r < i;) t = a, a = this[r], e = t[0] * a[1] - a[0] * t[1], u += (t[0] + a[0]) * e, o += (t[1] + a[1]) * e;
-                    return [u * n, o * n]
-                }, fi.clip = function(n) {
-                    for (var t, e, r, i, u, o, a = pi(n), l = -1, c = this.length - pi(this), f = this[c - 1]; ++l < c;) {
-                        for (t = n.slice(), n.length = 0, i = this[l], u = t[(r = t.length - a) - 1], e = -1; ++e < r;) si(o = t[e], f, i) ? (si(u, f, i) || n.push(hi(u, o, f, i)), n.push(o)) : si(u, f, i) && n.push(hi(u, o, f, i)), u = o;
-                        a && n.push(n[0]), f = i
-                    }
-                    return n
+    function Rr() {
+        tu(this), this.edge = this.site = this.circle = null
+    }
+
+    function Dr(n) {
+        var t = Kc.pop() || new Rr;
+        return t.site = n, t
+    }
+
+    function Pr(n) {
+        Xr(n), Wc.remove(n), Kc.push(n), tu(n)
+    }
+
+    function Ur(n) {
+        var t = n.circle,
+            e = t.x,
+            r = t.cy,
+            u = {
+                x: e,
+                y: r
+            },
+            i = n.P,
+            o = n.N,
+            a = [n];
+        Pr(n);
+        for (var c = i; c.circle && ca(e - c.circle.x) < Na && ca(r - c.circle.cy) < Na;) i = c.P, a.unshift(c), Pr(c), c = i;
+        a.unshift(c), Xr(c);
+        for (var l = o; l.circle && ca(e - l.circle.x) < Na && ca(r - l.circle.cy) < Na;) o = l.N, a.push(l), Pr(l), l = o;
+        a.push(l), Xr(l);
+        var s, f = a.length;
+        for (s = 1; f > s; ++s) l = a[s], c = a[s - 1], Kr(l.edge, c.site, l.site, u);
+        c = a[0], l = a[f - 1], l.edge = Jr(c.site, l.site, null, u), Vr(c), Vr(l)
+    }
+
+    function jr(n) {
+        for (var t, e, r, u, i = n.x, o = n.y, a = Wc._; a;)
+            if (r = Fr(a, o) - i, r > Na) a = a.L;
+            else {
+                if (u = i - Hr(a, o), !(u > Na)) {
+                    r > -Na ? (t = a.P, e = a) : u > -Na ? (t = a, e = a.N) : t = e = a;
+                    break
+                }
+                if (!a.R) {
+                    t = a;
+                    break
+                }
+                a = a.R
+            } var c = Dr(n);
+        if (Wc.insert(t, c), t || e) {
+            if (t === e) return Xr(t), e = Dr(t.site), Wc.insert(c, e), c.edge = e.edge = Jr(t.site, c.site), Vr(t), Vr(e), void 0;
+            if (!e) return c.edge = Jr(t.site, c.site), void 0;
+            Xr(t), Xr(e);
+            var l = t.site,
+                s = l.x,
+                f = l.y,
+                h = n.x - s,
+                g = n.y - f,
+                p = e.site,
+                v = p.x - s,
+                d = p.y - f,
+                m = 2 * (h * d - g * v),
+                y = h * h + g * g,
+                x = v * v + d * d,
+                M = {
+                    x: (d * y - g * x) / m + s,
+                    y: (h * x - v * y) / m + f
                 };
-                var gi, vi, di, yi, mi, Mi = [],
-                    xi = [];
+            Kr(e.edge, l, p, M), c.edge = Jr(l, n, null, M), e.edge = Jr(n, p, null, M), Vr(t), Vr(e)
+        }
+    }
 
-                function bi() {
-                    Hi(this), this.edge = this.site = this.circle = null
-                }
+    function Fr(n, t) {
+        var e = n.site,
+            r = e.x,
+            u = e.y,
+            i = u - t;
+        if (!i) return r;
+        var o = n.P;
+        if (!o) return -1 / 0;
+        e = o.site;
+        var a = e.x,
+            c = e.y,
+            l = c - t;
+        if (!l) return a;
+        var s = a - r,
+            f = 1 / i - 1 / l,
+            h = s / l;
+        return f ? (-h + Math.sqrt(h * h - 2 * f * (s * s / (-2 * l) - c + l / 2 + u - i / 2))) / f + r : (r + a) / 2
+    }
 
-                function wi(n) {
-                    var t = Mi.pop() || new bi;
-                    return t.site = n, t
-                }
+    function Hr(n, t) {
+        var e = n.N;
+        if (e) return Fr(e, t);
+        var r = n.site;
+        return r.y === t ? r.x : 1 / 0
+    }
 
-                function _i(n) {
-                    qi(n), di.remove(n), Mi.push(n), Hi(n)
-                }
+    function Or(n) {
+        this.site = n, this.edges = []
+    }
 
-                function ki(n) {
-                    var t = n.circle,
-                        e = t.x,
-                        r = t.cy,
-                        i = {
-                            x: e,
-                            y: r
-                        },
-                        u = n.P,
-                        o = n.N,
-                        a = [n];
-                    _i(n);
-                    for (var l = u; l.circle && w(e - l.circle.x) < Cn && w(r - l.circle.cy) < Cn;) u = l.P, a.unshift(l), _i(l), l = u;
-                    a.unshift(l), qi(l);
-                    for (var c = o; c.circle && w(e - c.circle.x) < Cn && w(r - c.circle.cy) < Cn;) o = c.N, a.push(c), _i(c), c = o;
-                    a.push(c), qi(c);
-                    var f, s = a.length;
-                    for (f = 1; f < s; ++f) c = a[f], l = a[f - 1], Ui(c.edge, l.site, c.site, i);
-                    l = a[0], (c = a[s - 1]).edge = Di(l.site, c.site, null, i), Li(l), Li(c)
-                }
-
-                function Si(n) {
-                    for (var t, e, r, i, u = n.x, o = n.y, a = di._; a;)
-                        if ((r = Ni(a, o) - u) > Cn) a = a.L;
-                        else {
-                            if (!((i = u - Ei(a, o)) > Cn)) {
-                                r > -Cn ? (t = a.P, e = a) : i > -Cn ? (t = a, e = a.N) : t = e = a;
+    function Yr(n) {
+        for (var t, e, r, u, i, o, a, c, l, s, f = n[0][0], h = n[1][0], g = n[0][1], p = n[1][1], v = Bc, d = v.length; d--;)
+            if (i = v[d], i && i.prepare())
+                for (a = i.edges, c = a.length, o = 0; c > o;) s = a[o].end(), r = s.x, u = s.y, l = a[++o % c].start(), t = l.x, e = l.y, (ca(r - t) > Na || ca(u - e) > Na) && (a.splice(o, 0, new Qr(Gr(i.site, s, ca(r - f) < Na && p - u > Na ? {
+                    x: f,
+                    y: ca(t - f) < Na ? e : p
+                } : ca(u - p) < Na && h - r > Na ? {
+                    x: ca(e - p) < Na ? t : h,
+                    y: p
+                } : ca(r - h) < Na && u - g > Na ? {
+                    x: h,
+                    y: ca(t - h) < Na ? e : g
+                } : ca(u - g) < Na && r - f > Na ? {
+                    x: ca(e - g) < Na ? t : f,
+                    y: g
+                } : null), i.site, null)), ++c)
+    }
+
+    function Ir(n, t) {
+        return t.angle - n.angle
+    }
+
+    function Zr() {
+        tu(this), this.x = this.y = this.arc = this.site = this.cy = null
+    }
+
+    function Vr(n) {
+        var t = n.P,
+            e = n.N;
+        if (t && e) {
+            var r = t.site,
+                u = n.site,
+                i = e.site;
+            if (r !== i) {
+                var o = u.x,
+                    a = u.y,
+                    c = r.x - o,
+                    l = r.y - a,
+                    s = i.x - o,
+                    f = i.y - a,
+                    h = 2 * (c * f - l * s);
+                if (!(h >= -za)) {
+                    var g = c * c + l * l,
+                        p = s * s + f * f,
+                        v = (f * g - l * p) / h,
+                        d = (c * p - s * g) / h,
+                        f = d + a,
+                        m = Qc.pop() || new Zr;
+                    m.arc = n, m.site = u, m.x = v + o, m.y = f + Math.sqrt(v * v + d * d), m.cy = f, n.circle = m;
+                    for (var y = null, x = Gc._; x;)
+                        if (m.y < x.y || m.y === x.y && m.x <= x.x) {
+                            if (!x.L) {
+                                y = x.P;
                                 break
                             }
-                            if (!a.R) {
-                                t = a;
+                            x = x.L
+                        } else {
+                            if (!x.R) {
+                                y = x;
                                 break
                             }
-                            a = a.R
-                        } var l = wi(n);
-                    if (di.insert(t, l), t || e) {
-                        if (t === e) return qi(t), e = wi(t.site), di.insert(l, e), l.edge = e.edge = Di(t.site, l.site), Li(t), void Li(e);
-                        if (e) {
-                            qi(t), qi(e);
-                            var c = t.site,
-                                f = c.x,
-                                s = c.y,
-                                h = n.x - f,
-                                p = n.y - s,
-                                g = e.site,
-                                v = g.x - f,
-                                d = g.y - s,
-                                y = 2 * (h * d - p * v),
-                                m = h * h + p * p,
-                                M = v * v + d * d,
-                                x = {
-                                    x: (d * m - p * M) / y + f,
-                                    y: (h * M - v * m) / y + s
-                                };
-                            Ui(e.edge, c, g, x), l.edge = Di(c, n, null, x), e.edge = Di(n, g, null, x), Li(t), Li(e)
-                        } else l.edge = Di(t.site, l.site)
-                    }
+                            x = x.R
+                        } Gc.insert(y, m), y || (Jc = m)
                 }
+            }
+        }
+    }
 
-                function Ni(n, t) {
-                    var e = n.site,
-                        r = e.x,
-                        i = e.y,
-                        u = i - t;
-                    if (!u) return r;
-                    var o = n.P;
-                    if (!o) return -1 / 0;
-                    var a = (e = o.site).x,
-                        l = e.y,
-                        c = l - t;
-                    if (!c) return a;
-                    var f = a - r,
-                        s = 1 / u - 1 / c,
-                        h = f / c;
-                    return s ? (-h + Math.sqrt(h * h - 2 * s * (f * f / (-2 * c) - l + c / 2 + i - u / 2))) / s + r : (r + a) / 2
-                }
-
-                function Ei(n, t) {
-                    var e = n.N;
-                    if (e) return Ni(e, t);
-                    var r = n.site;
-                    return r.y === t ? r.x : 1 / 0
-                }
-
-                function Ai(n) {
-                    this.site = n, this.edges = []
-                }
-
-                function Ci(n, t) {
-                    return t.angle - n.angle
-                }
-
-                function zi() {
-                    Hi(this), this.x = this.y = this.arc = this.site = this.cy = null
-                }
-
-                function Li(n) {
-                    var t = n.P,
-                        e = n.N;
-                    if (t && e) {
-                        var r = t.site,
-                            i = n.site,
-                            u = e.site;
-                        if (r !== u) {
-                            var o = i.x,
-                                a = i.y,
-                                l = r.x - o,
-                                c = r.y - a,
-                                f = u.x - o,
-                                s = 2 * (l * (d = u.y - a) - c * f);
-                            if (!(s >= -zn)) {
-                                var h = l * l + c * c,
-                                    p = f * f + d * d,
-                                    g = (d * h - c * p) / s,
-                                    v = (l * p - f * h) / s,
-                                    d = v + a,
-                                    y = xi.pop() || new zi;
-                                y.arc = n, y.site = i, y.x = g + o, y.y = d + Math.sqrt(g * g + v * v), y.cy = d, n.circle = y;
-                                for (var m = null, M = mi._; M;)
-                                    if (y.y < M.y || y.y === M.y && y.x <= M.x) {
-                                        if (!M.L) {
-                                            m = M.P;
-                                            break
-                                        }
-                                        M = M.L
-                                    } else {
-                                        if (!M.R) {
-                                            m = M;
-                                            break
-                                        }
-                                        M = M.R
-                                    } mi.insert(m, y), m || (yi = y)
-                            }
-                        }
-                    }
-                }
+    function Xr(n) {
+        var t = n.circle;
+        t && (t.P || (Jc = t.N), Gc.remove(t), Qc.push(t), tu(t), n.circle = null)
+    }
 
-                function qi(n) {
-                    var t = n.circle;
-                    t && (t.P || (yi = t.N), mi.remove(t), xi.push(t), Hi(t), n.circle = null)
-                }
-
-                function Ti(n, t) {
-                    var e = n.b;
-                    if (e) return !0;
-                    var r, i, u = n.a,
-                        o = t[0][0],
-                        a = t[1][0],
-                        l = t[0][1],
-                        c = t[1][1],
-                        f = n.l,
-                        s = n.r,
-                        h = f.x,
-                        p = f.y,
-                        g = s.x,
-                        v = s.y,
-                        d = (h + g) / 2,
-                        y = (p + v) / 2;
-                    if (v === p) {
-                        if (d < o || d >= a) return;
-                        if (h > g) {
-                            if (u) {
-                                if (u.y >= c) return
-                            } else u = {
-                                x: d,
-                                y: l
-                            };
-                            e = {
-                                x: d,
-                                y: c
-                            }
-                        } else {
-                            if (u) {
-                                if (u.y < l) return
-                            } else u = {
-                                x: d,
-                                y: c
-                            };
-                            e = {
-                                x: d,
-                                y: l
-                            }
-                        }
-                    } else if (i = y - (r = (h - g) / (v - p)) * d, r < -1 || r > 1)
-                        if (h > g) {
-                            if (u) {
-                                if (u.y >= c) return
-                            } else u = {
-                                x: (l - i) / r,
-                                y: l
-                            };
-                            e = {
-                                x: (c - i) / r,
-                                y: c
-                            }
-                        } else {
-                            if (u) {
-                                if (u.y < l) return
-                            } else u = {
-                                x: (c - i) / r,
-                                y: c
-                            };
-                            e = {
-                                x: (l - i) / r,
-                                y: l
-                            }
-                        }
-                    else if (p < v) {
-                        if (u) {
-                            if (u.x >= a) return
-                        } else u = {
-                            x: o,
-                            y: r * o + i
-                        };
-                        e = {
-                            x: a,
-                            y: r * a + i
-                        }
-                    } else {
-                        if (u) {
-                            if (u.x < o) return
-                        } else u = {
-                            x: a,
-                            y: r * a + i
-                        };
-                        e = {
-                            x: o,
-                            y: r * o + i
-                        }
-                    }
-                    return n.a = u, n.b = e, !0
-                }
+    function $r(n) {
+        for (var t, e = $c, r = He(n[0][0], n[0][1], n[1][0], n[1][1]), u = e.length; u--;) t = e[u], (!Br(t, n) || !r(t) || ca(t.a.x - t.b.x) < Na && ca(t.a.y - t.b.y) < Na) && (t.a = t.b = null, e.splice(u, 1))
+    }
 
-                function Ri(n, t) {
-                    this.l = n, this.r = t, this.a = this.b = null
-                }
+    function Br(n, t) {
+        var e = n.b;
+        if (e) return !0;
+        var r, u, i = n.a,
+            o = t[0][0],
+            a = t[1][0],
+            c = t[0][1],
+            l = t[1][1],
+            s = n.l,
+            f = n.r,
+            h = s.x,
+            g = s.y,
+            p = f.x,
+            v = f.y,
+            d = (h + p) / 2,
+            m = (g + v) / 2;
+        if (v === g) {
+            if (o > d || d >= a) return;
+            if (h > p) {
+                if (i) {
+                    if (i.y >= l) return
+                } else i = {
+                    x: d,
+                    y: c
+                };
+                e = {
+                    x: d,
+                    y: l
+                }
+            } else {
+                if (i) {
+                    if (i.y < c) return
+                } else i = {
+                    x: d,
+                    y: l
+                };
+                e = {
+                    x: d,
+                    y: c
+                }
+            }
+        } else if (r = (h - p) / (v - g), u = m - r * d, -1 > r || r > 1)
+            if (h > p) {
+                if (i) {
+                    if (i.y >= l) return
+                } else i = {
+                    x: (c - u) / r,
+                    y: c
+                };
+                e = {
+                    x: (l - u) / r,
+                    y: l
+                }
+            } else {
+                if (i) {
+                    if (i.y < c) return
+                } else i = {
+                    x: (l - u) / r,
+                    y: l
+                };
+                e = {
+                    x: (c - u) / r,
+                    y: c
+                }
+            }
+        else if (v > g) {
+            if (i) {
+                if (i.x >= a) return
+            } else i = {
+                x: o,
+                y: r * o + u
+            };
+            e = {
+                x: a,
+                y: r * a + u
+            }
+        } else {
+            if (i) {
+                if (i.x < o) return
+            } else i = {
+                x: a,
+                y: r * a + u
+            };
+            e = {
+                x: o,
+                y: r * o + u
+            }
+        }
+        return n.a = i, n.b = e, !0
+    }
 
-                function Di(n, t, e, r) {
-                    var i = new Ri(n, t);
-                    return gi.push(i), e && Ui(i, n, t, e), r && Ui(i, t, n, r), vi[n.i].edges.push(new ji(i, n, t)), vi[t.i].edges.push(new ji(i, t, n)), i
-                }
+    function Wr(n, t) {
+        this.l = n, this.r = t, this.a = this.b = null
+    }
 
-                function Pi(n, t, e) {
-                    var r = new Ri(n, null);
-                    return r.a = t, r.b = e, gi.push(r), r
-                }
+    function Jr(n, t, e, r) {
+        var u = new Wr(n, t);
+        return $c.push(u), e && Kr(u, n, t, e), r && Kr(u, t, n, r), Bc[n.i].edges.push(new Qr(u, n, t)), Bc[t.i].edges.push(new Qr(u, t, n)), u
+    }
 
-                function Ui(n, t, e, r) {
-                    n.a || n.b ? n.l === e ? n.b = r : n.a = r : (n.a = r, n.l = t, n.r = e)
-                }
+    function Gr(n, t, e) {
+        var r = new Wr(n, null);
+        return r.a = t, r.b = e, $c.push(r), r
+    }
 
-                function ji(n, t, e) {
-                    var r = n.a,
-                        i = n.b;
-                    this.edge = n, this.site = t, this.angle = e ? Math.atan2(e.y - t.y, e.x - t.x) : n.l === t ? Math.atan2(i.x - r.x, r.y - i.y) : Math.atan2(r.x - i.x, i.y - r.y)
-                }
+    function Kr(n, t, e, r) {
+        n.a || n.b ? n.l === e ? n.b = r : n.a = r : (n.a = r, n.l = t, n.r = e)
+    }
 
-                function Fi() {
-                    this._ = null
-                }
+    function Qr(n, t, e) {
+        var r = n.a,
+            u = n.b;
+        this.edge = n, this.site = t, this.angle = e ? Math.atan2(e.y - t.y, e.x - t.x) : n.l === t ? Math.atan2(u.x - r.x, r.y - u.y) : Math.atan2(r.x - u.x, u.y - r.y)
+    }
 
-                function Hi(n) {
-                    n.U = n.C = n.L = n.R = n.P = n.N = null
-                }
+    function nu() {
+        this._ = null
+    }
 
-                function Oi(n, t) {
-                    var e = t,
-                        r = t.R,
-                        i = e.U;
-                    i ? i.L === e ? i.L = r : i.R = r : n._ = r, r.U = i, e.U = r, e.R = r.L, e.R && (e.R.U = e), r.L = e
-                }
+    function tu(n) {
+        n.U = n.C = n.L = n.R = n.P = n.N = null
+    }
 
-                function Ii(n, t) {
-                    var e = t,
-                        r = t.L,
-                        i = e.U;
-                    i ? i.L === e ? i.L = r : i.R = r : n._ = r, r.U = i, e.U = r, e.L = r.R, e.L && (e.L.U = e), r.R = e
-                }
+    function eu(n, t) {
+        var e = t,
+            r = t.R,
+            u = e.U;
+        u ? u.L === e ? u.L = r : u.R = r : n._ = r, r.U = u, e.U = r, e.R = r.L, e.R && (e.R.U = e), r.L = e
+    }
 
-                function Yi(n) {
-                    for (; n.L;) n = n.L;
-                    return n
-                }
+    function ru(n, t) {
+        var e = t,
+            r = t.L,
+            u = e.U;
+        u ? u.L === e ? u.L = r : u.R = r : n._ = r, r.U = u, e.U = r, e.L = r.R, e.L && (e.L.U = e), r.R = e
+    }
 
-                function Zi(n, t) {
-                    var e, r, i, u = n.sort(Vi).pop();
-                    for (gi = [], vi = new Array(n.length), di = new Fi, mi = new Fi;;)
-                        if (i = yi, u && (!i || u.y < i.y || u.y === i.y && u.x < i.x)) u.x === e && u.y === r || (vi[u.i] = new Ai(u), Si(u), e = u.x, r = u.y), u = n.pop();
-                        else {
-                            if (!i) break;
-                            ki(i.arc)
-                        } t && (function(n) {
-                        for (var t, e = gi, r = ar(n[0][0], n[0][1], n[1][0], n[1][1]), i = e.length; i--;)(!Ti(t = e[i], n) || !r(t) || w(t.a.x - t.b.x) < Cn && w(t.a.y - t.b.y) < Cn) && (t.a = t.b = null, e.splice(i, 1))
-                    }(t), function(n) {
-                        for (var t, e, r, i, u, o, a, l, c, f, s = n[0][0], h = n[1][0], p = n[0][1], g = n[1][1], v = vi, d = v.length; d--;)
-                            if ((u = v[d]) && u.prepare())
-                                for (l = (a = u.edges).length, o = 0; o < l;) r = (f = a[o].end()).x, i = f.y, t = (c = a[++o % l].start()).x, e = c.y, (w(r - t) > Cn || w(i - e) > Cn) && (a.splice(o, 0, new ji(Pi(u.site, f, w(r - s) < Cn && g - i > Cn ? {
-                                    x: s,
-                                    y: w(t - s) < Cn ? e : g
-                                } : w(i - g) < Cn && h - r > Cn ? {
-                                    x: w(e - g) < Cn ? t : h,
-                                    y: g
-                                } : w(r - h) < Cn && i - p > Cn ? {
-                                    x: h,
-                                    y: w(t - h) < Cn ? e : p
-                                } : w(i - p) < Cn && r - s > Cn ? {
-                                    x: w(e - p) < Cn ? t : s,
-                                    y: p
-                                } : null), u.site, null)), ++l)
-                    }(t));
-                    var o = {
-                        cells: vi,
-                        edges: gi
-                    };
-                    return di = mi = gi = vi = null, o
-                }
+    function uu(n) {
+        for (; n.L;) n = n.L;
+        return n
+    }
 
-                function Vi(n, t) {
-                    return t.y - n.y || t.x - n.x
-                }
-                Ai.prototype.prepare = function() {
-                    for (var n, t = this.edges, e = t.length; e--;)(n = t[e].edge).b && n.a || t.splice(e, 1);
-                    return t.sort(Ci), t.length
-                }, ji.prototype = {
-                    start: function() {
-                        return this.edge.l === this.site ? this.edge.a : this.edge.b
-                    },
-                    end: function() {
-                        return this.edge.l === this.site ? this.edge.b : this.edge.a
-                    }
-                }, Fi.prototype = {
-                    insert: function(n, t) {
-                        var e, r, i;
-                        if (n) {
-                            if (t.P = n, t.N = n.N, n.N && (n.N.P = t), n.N = t, n.R) {
-                                for (n = n.R; n.L;) n = n.L;
-                                n.L = t
-                            } else n.R = t;
-                            e = n
-                        } else this._ ? (n = Yi(this._), t.P = null, t.N = n, n.P = n.L = t, e = n) : (t.P = t.N = null, this._ = t, e = null);
-                        for (t.L = t.R = null, t.U = e, t.C = !0, n = t; e && e.C;) e === (r = e.U).L ? (i = r.R) && i.C ? (e.C = i.C = !1, r.C = !0, n = r) : (n === e.R && (Oi(this, e), e = (n = e).U), e.C = !1, r.C = !0, Ii(this, r)) : (i = r.L) && i.C ? (e.C = i.C = !1, r.C = !0, n = r) : (n === e.L && (Ii(this, e), e = (n = e).U), e.C = !1, r.C = !0, Oi(this, r)), e = n.U;
-                        this._.C = !1
-                    },
-                    remove: function(n) {
-                        n.N && (n.N.P = n.P), n.P && (n.P.N = n.N), n.N = n.P = null;
-                        var t, e, r, i = n.U,
-                            u = n.L,
-                            o = n.R;
-                        if (e = u ? o ? Yi(o) : u : o, i ? i.L === n ? i.L = e : i.R = e : this._ = e, u && o ? (r = e.C, e.C = n.C, e.L = u, u.U = e, e !== o ? (i = e.U, e.U = n.U, n = e.R, i.L = n, e.R = o, o.U = e) : (e.U = i, i = e, n = e.R)) : (r = n.C, n = e), n && (n.U = i), !r)
-                            if (n && n.C) n.C = !1;
-                            else {
-                                do {
-                                    if (n === this._) break;
-                                    if (n === i.L) {
-                                        if ((t = i.R).C && (t.C = !1, i.C = !0, Oi(this, i), t = i.R), t.L && t.L.C || t.R && t.R.C) {
-                                            t.R && t.R.C || (t.L.C = !1, t.C = !0, Ii(this, t), t = i.R), t.C = i.C, i.C = t.R.C = !1, Oi(this, i), n = this._;
-                                            break
-                                        }
-                                    } else if ((t = i.L).C && (t.C = !1, i.C = !0, Ii(this, i), t = i.L), t.L && t.L.C || t.R && t.R.C) {
-                                        t.L && t.L.C || (t.R.C = !1, t.C = !0, Oi(this, t), t = i.L), t.C = i.C, i.C = t.L.C = !1, Ii(this, i), n = this._;
-                                        break
-                                    }
-                                    t.C = !0, n = i, i = i.U
-                                } while (!n.C);
-                                n && (n.C = !1)
-                            }
-                    }
-                }, u.geom.voronoi = function(n) {
-                    var t = oi,
-                        e = ai,
-                        r = t,
-                        i = e,
-                        u = Xi;
-                    if (n) return o(n);
-
-                    function o(n) {
-                        var t = new Array(n.length),
-                            e = u[0][0],
-                            r = u[0][1],
-                            i = u[1][0],
-                            o = u[1][1];
-                        return Zi(a(n), u).cells.forEach((function(u, a) {
-                            var l = u.edges,
-                                c = u.site;
-                            (t[a] = l.length ? l.map((function(n) {
-                                var t = n.start();
-                                return [t.x, t.y]
-                            })) : c.x >= e && c.x <= i && c.y >= r && c.y <= o ? [
-                                [e, o],
-                                [i, o],
-                                [i, r],
-                                [e, r]
-                            ] : []).point = n[a]
-                        })), t
-                    }
+    function iu(n, t) {
+        var e, r, u, i = n.sort(ou).pop();
+        for ($c = [], Bc = new Array(n.length), Wc = new nu, Gc = new nu;;)
+            if (u = Jc, i && (!u || i.y < u.y || i.y === u.y && i.x < u.x))(i.x !== e || i.y !== r) && (Bc[i.i] = new Or(i), jr(i), e = i.x, r = i.y), i = n.pop();
+            else {
+                if (!u) break;
+                Ur(u.arc)
+            } t && ($r(t), Yr(t));
+        var o = {
+            cells: Bc,
+            edges: $c
+        };
+        return Wc = Gc = $c = Bc = null, o
+    }
 
-                    function a(n) {
-                        return n.map((function(n, t) {
-                            return {
-                                x: Math.round(r(n, t) / Cn) * Cn,
-                                y: Math.round(i(n, t) / Cn) * Cn,
-                                i: t
-                            }
-                        }))
-                    }
-                    return o.links = function(n) {
-                        return Zi(a(n)).edges.filter((function(n) {
-                            return n.l && n.r
-                        })).map((function(t) {
-                            return {
-                                source: n[t.l.i],
-                                target: n[t.r.i]
-                            }
-                        }))
-                    }, o.triangles = function(n) {
-                        var t = [];
-                        return Zi(a(n)).cells.forEach((function(e, r) {
-                            for (var i, u, o, a, l = e.site, c = e.edges.sort(Ci), f = -1, s = c.length, h = c[s - 1].edge, p = h.l === l ? h.r : h.l; ++f < s;) h, i = p, p = (h = c[f].edge).l === l ? h.r : h.l, r < i.i && r < p.i && (o = i, a = p, ((u = l).x - a.x) * (o.y - u.y) - (u.x - o.x) * (a.y - u.y) < 0) && t.push([n[r], n[i.i], n[p.i]])
-                        })), t
-                    }, o.x = function(n) {
-                        return arguments.length ? (r = Mt(t = n), o) : t
-                    }, o.y = function(n) {
-                        return arguments.length ? (i = Mt(e = n), o) : e
-                    }, o.clipExtent = function(n) {
-                        return arguments.length ? (u = null == n ? Xi : n, o) : u === Xi ? null : u
-                    }, o.size = function(n) {
-                        return arguments.length ? o.clipExtent(n && [
-                            [0, 0], n
-                        ]) : u === Xi ? null : u && u[1]
-                    }, o
-                };
-                var Xi = [
-                    [-1e6, -1e6],
-                    [1e6, 1e6]
-                ];
+    function ou(n, t) {
+        return t.y - n.y || t.x - n.x
+    }
 
-                function $i(n) {
-                    return n.x
-                }
+    function au(n, t, e) {
+        return (n.x - e.x) * (t.y - n.y) - (n.x - t.x) * (e.y - n.y)
+    }
 
-                function Bi(n) {
-                    return n.y
-                }
+    function cu(n) {
+        return n.x
+    }
 
-                function Ji(n, t, e, r, i, u) {
-                    if (!n(t, e, r, i, u)) {
-                        var o = .5 * (e + i),
-                            a = .5 * (r + u),
-                            l = t.nodes;
-                        l[0] && Ji(n, l[0], e, r, o, a), l[1] && Ji(n, l[1], o, r, i, a), l[2] && Ji(n, l[2], e, a, o, u), l[3] && Ji(n, l[3], o, a, i, u)
-                    }
-                }
+    function lu(n) {
+        return n.y
+    }
 
-                function Wi(n, t, e, r, i, u, o) {
-                    var a, l = 1 / 0;
-                    return function n(c, f, s, h, p) {
-                        if (!(f > u || s > o || h < r || p < i)) {
-                            if (g = c.point) {
-                                var g, v = t - c.x,
-                                    d = e - c.y,
-                                    y = v * v + d * d;
-                                if (y < l) {
-                                    var m = Math.sqrt(l = y);
-                                    r = t - m, i = e - m, u = t + m, o = e + m, a = g
-                                }
-                            }
-                            for (var M = c.nodes, x = .5 * (f + h), b = .5 * (s + p), w = (e >= b) << 1 | t >= x, _ = w + 4; w < _; ++w)
-                                if (c = M[3 & w]) switch (3 & w) {
-                                    case 0:
-                                        n(c, f, s, x, b);
-                                        break;
-                                    case 1:
-                                        n(c, x, s, h, b);
-                                        break;
-                                    case 2:
-                                        n(c, f, b, x, p);
-                                        break;
-                                    case 3:
-                                        n(c, x, b, h, p)
-                                }
-                        }
-                    }(n, r, i, u, o), a
-                }
+    function su() {
+        return {
+            leaf: !0,
+            nodes: [],
+            point: null,
+            x: null,
+            y: null
+        }
+    }
 
-                function Gi(n, t) {
-                    n = u.rgb(n), t = u.rgb(t);
-                    var e = n.r,
-                        r = n.g,
-                        i = n.b,
-                        o = t.r - e,
-                        a = t.g - r,
-                        l = t.b - i;
-                    return function(n) {
-                        return "#" + ht(Math.round(e + o * n)) + ht(Math.round(r + a * n)) + ht(Math.round(i + l * n))
-                    }
-                }
+    function fu(n, t, e, r, u, i) {
+        if (!n(t, e, r, u, i)) {
+            var o = .5 * (e + u),
+                a = .5 * (r + i),
+                c = t.nodes;
+            c[0] && fu(n, c[0], e, r, o, a), c[1] && fu(n, c[1], o, r, u, a), c[2] && fu(n, c[2], e, a, o, i), c[3] && fu(n, c[3], o, a, u, i)
+        }
+    }
 
-                function Ki(n, t) {
-                    var e, r = {},
-                        i = {};
-                    for (e in n) e in t ? r[e] = ru(n[e], t[e]) : i[e] = n[e];
-                    for (e in t) e in n || (i[e] = t[e]);
-                    return function(n) {
-                        for (e in r) i[e] = r[e](n);
-                        return i
-                    }
-                }
+    function hu(n, t) {
+        n = Bo.rgb(n), t = Bo.rgb(t);
+        var e = n.r,
+            r = n.g,
+            u = n.b,
+            i = t.r - e,
+            o = t.g - r,
+            a = t.b - u;
+        return function(n) {
+            return "#" + xt(Math.round(e + i * n)) + xt(Math.round(r + o * n)) + xt(Math.round(u + a * n))
+        }
+    }
 
-                function Qi(n, t) {
-                    return n = +n, t = +t,
-                        function(e) {
-                            return n * (1 - e) + t * e
-                        }
-                }
+    function gu(n, t) {
+        var e, r = {},
+            u = {};
+        for (e in n) e in t ? r[e] = du(n[e], t[e]) : u[e] = n[e];
+        for (e in t) e in n || (u[e] = t[e]);
+        return function(n) {
+            for (e in r) u[e] = r[e](n);
+            return u
+        }
+    }
 
-                function nu(n, t) {
-                    var e, r, i, u = tu.lastIndex = eu.lastIndex = 0,
-                        o = -1,
-                        a = [],
-                        l = [];
-                    for (n += "", t += "";
-                        (e = tu.exec(n)) && (r = eu.exec(t));)(i = r.index) > u && (i = t.slice(u, i), a[o] ? a[o] += i : a[++o] = i), (e = e[0]) === (r = r[0]) ? a[o] ? a[o] += r : a[++o] = r : (a[++o] = null, l.push({
-                        i: o,
-                        x: Qi(e, r)
-                    })), u = eu.lastIndex;
-                    return u < t.length && (i = t.slice(u), a[o] ? a[o] += i : a[++o] = i), a.length < 2 ? l[0] ? (t = l[0].x, function(n) {
-                        return t(n) + ""
-                    }) : function() {
-                        return t
-                    } : (t = l.length, function(n) {
-                        for (var e, r = 0; r < t; ++r) a[(e = l[r]).i] = e.x(n);
-                        return a.join("")
-                    })
-                }
-                u.geom.delaunay = function(n) {
-                    return u.geom.voronoi().triangles(n)
-                }, u.geom.quadtree = function(n, t, e, r, i) {
-                    var u, o = oi,
-                        a = ai;
-                    if (u = arguments.length) return o = $i, a = Bi, 3 === u && (i = e, r = t, e = t = 0), l(n);
-
-                    function l(n) {
-                        var l, c, f, s, h, p, g, v, d, y = Mt(o),
-                            m = Mt(a);
-                        if (null != t) p = t, g = e, v = r, d = i;
-                        else if (v = d = -(p = g = 1 / 0), c = [], f = [], h = n.length, u)
-                            for (s = 0; s < h; ++s)(l = n[s]).x < p && (p = l.x), l.y < g && (g = l.y), l.x > v && (v = l.x), l.y > d && (d = l.y), c.push(l.x), f.push(l.y);
-                        else
-                            for (s = 0; s < h; ++s) {
-                                var M = +y(l = n[s], s),
-                                    x = +m(l, s);
-                                M < p && (p = M), x < g && (g = x), M > v && (v = M), x > d && (d = x), c.push(M), f.push(x)
-                            }
-                        var b = v - p,
-                            _ = d - g;
+    function pu(n, t) {
+        return n = +n, t = +t,
+            function(e) {
+                return n * (1 - e) + t * e
+            }
+    }
 
-                        function k(n, t, e, r, i, u, o, a) {
-                            if (!isNaN(e) && !isNaN(r))
-                                if (n.leaf) {
-                                    var l = n.x,
-                                        c = n.y;
-                                    if (null != l)
-                                        if (w(l - e) + w(c - r) < .01) S(n, t, e, r, i, u, o, a);
-                                        else {
-                                            var f = n.point;
-                                            n.x = n.y = n.point = null, S(n, f, l, c, i, u, o, a), S(n, t, e, r, i, u, o, a)
-                                        }
-                                    else n.x = e, n.y = r, n.point = t
-                                } else S(n, t, e, r, i, u, o, a)
-                        }
+    function vu(n, t) {
+        var e, r, u, i = tl.lastIndex = el.lastIndex = 0,
+            o = -1,
+            a = [],
+            c = [];
+        for (n += "", t += "";
+            (e = tl.exec(n)) && (r = el.exec(t));)(u = r.index) > i && (u = t.slice(i, u), a[o] ? a[o] += u : a[++o] = u), (e = e[0]) === (r = r[0]) ? a[o] ? a[o] += r : a[++o] = r : (a[++o] = null, c.push({
+            i: o,
+            x: pu(e, r)
+        })), i = el.lastIndex;
+        return i < t.length && (u = t.slice(i), a[o] ? a[o] += u : a[++o] = u), a.length < 2 ? c[0] ? (t = c[0].x, function(n) {
+            return t(n) + ""
+        }) : function() {
+            return t
+        } : (t = c.length, function(n) {
+            for (var e, r = 0; t > r; ++r) a[(e = c[r]).i] = e.x(n);
+            return a.join("")
+        })
+    }
 
-                        function S(n, t, e, r, i, u, o, a) {
-                            var l = .5 * (i + o),
-                                c = .5 * (u + a),
-                                f = e >= l,
-                                s = r >= c,
-                                h = s << 1 | f;
-                            n.leaf = !1, f ? i = l : o = l, s ? u = c : a = c, k(n = n.nodes[h] || (n.nodes[h] = {
-                                leaf: !0,
-                                nodes: [],
-                                point: null,
-                                x: null,
-                                y: null
-                            }), t, e, r, i, u, o, a)
-                        }
-                        b > _ ? d = g + b : v = p + _;
-                        var N = {
-                            leaf: !0,
-                            nodes: [],
-                            point: null,
-                            x: null,
-                            y: null,
-                            add: function(n) {
-                                k(N, n, +y(n, ++s), +m(n, s), p, g, v, d)
-                            },
-                            visit: function(n) {
-                                Ji(n, N, p, g, v, d)
-                            },
-                            find: function(n) {
-                                return Wi(N, n[0], n[1], p, g, v, d)
-                            }
-                        };
-                        if (s = -1, null == t) {
-                            for (; ++s < h;) k(N, n[s], c[s], f[s], p, g, v, d);
-                            --s
-                        } else n.forEach(N.add);
-                        return c = f = n = l = null, N
-                    }
-                    return l.x = function(n) {
-                        return arguments.length ? (o = n, l) : o
-                    }, l.y = function(n) {
-                        return arguments.length ? (a = n, l) : a
-                    }, l.extent = function(n) {
-                        return arguments.length ? (null == n ? t = e = r = i = null : (t = +n[0][0], e = +n[0][1], r = +n[1][0], i = +n[1][1]), l) : null == t ? null : [
-                            [t, e],
-                            [r, i]
-                        ]
-                    }, l.size = function(n) {
-                        return arguments.length ? (null == n ? t = e = r = i = null : (t = e = 0, r = +n[0], i = +n[1]), l) : null == t ? null : [r - t, i - e]
-                    }, l
-                }, u.interpolateRgb = Gi, u.interpolateObject = Ki, u.interpolateNumber = Qi, u.interpolateString = nu;
-                var tu = /[-+]?(?:\d+\.?\d*|\.?\d+)(?:[eE][-+]?\d+)?/g,
-                    eu = new RegExp(tu.source, "g");
-
-                function ru(n, t) {
-                    for (var e, r = u.interpolators.length; --r >= 0 && !(e = u.interpolators[r](n, t)););
-                    return e
-                }
-
-                function iu(n, t) {
-                    var e, r = [],
-                        i = [],
-                        u = n.length,
-                        o = t.length,
-                        a = Math.min(n.length, t.length);
-                    for (e = 0; e < a; ++e) r.push(ru(n[e], t[e]));
-                    for (; e < u; ++e) i[e] = n[e];
-                    for (; e < o; ++e) i[e] = t[e];
-                    return function(n) {
-                        for (e = 0; e < a; ++e) i[e] = r[e](n);
-                        return i
-                    }
-                }
-                u.interpolate = ru, u.interpolators = [function(n, t) {
-                    var e = typeof t;
-                    return ("string" === e ? mt.has(t.toLowerCase()) || /^(#|rgb\(|hsl\()/i.test(t) ? Gi : nu : t instanceof $n ? Gi : Array.isArray(t) ? iu : "object" === e && isNaN(t) ? Ki : Qi)(n, t)
-                }], u.interpolateArray = iu;
-                var uu = function() {
-                        return R
-                    },
-                    ou = u.map({
-                        linear: uu,
-                        poly: function(n) {
-                            return function(t) {
-                                return Math.pow(t, n)
-                            }
-                        },
-                        quad: function() {
-                            return su
-                        },
-                        cubic: function() {
-                            return hu
-                        },
-                        sin: function() {
-                            return gu
-                        },
-                        exp: function() {
-                            return vu
-                        },
-                        circle: function() {
-                            return du
-                        },
-                        elastic: function(n, t) {
-                            var e;
-                            arguments.length < 2 && (t = .45);
-                            arguments.length ? e = t / qn * Math.asin(1 / n) : (n = 1, e = t / 4);
-                            return function(r) {
-                                return 1 + n * Math.pow(2, -10 * r) * Math.sin((r - e) * qn / t)
-                            }
-                        },
-                        back: function(n) {
-                            n || (n = 1.70158);
-                            return function(t) {
-                                return t * t * ((n + 1) * t - n)
-                            }
-                        },
-                        bounce: function() {
-                            return yu
-                        }
-                    }),
-                    au = u.map({
-                        in: R,
-                        out: cu,
-                        "in-out": fu,
-                        "out-in": function(n) {
-                            return fu(cu(n))
-                        }
-                    });
+    function du(n, t) {
+        for (var e, r = Bo.interpolators.length; --r >= 0 && !(e = Bo.interpolators[r](n, t)););
+        return e
+    }
 
-                function lu(n) {
-                    return function(t) {
-                        return t <= 0 ? 0 : t >= 1 ? 1 : n(t)
-                    }
-                }
+    function mu(n, t) {
+        var e, r = [],
+            u = [],
+            i = n.length,
+            o = t.length,
+            a = Math.min(n.length, t.length);
+        for (e = 0; a > e; ++e) r.push(du(n[e], t[e]));
+        for (; i > e; ++e) u[e] = n[e];
+        for (; o > e; ++e) u[e] = t[e];
+        return function(n) {
+            for (e = 0; a > e; ++e) u[e] = r[e](n);
+            return u
+        }
+    }
 
-                function cu(n) {
-                    return function(t) {
-                        return 1 - n(1 - t)
-                    }
-                }
+    function yu(n) {
+        return function(t) {
+            return 0 >= t ? 0 : t >= 1 ? 1 : n(t)
+        }
+    }
 
-                function fu(n) {
-                    return function(t) {
-                        return .5 * (t < .5 ? n(2 * t) : 2 - n(2 - 2 * t))
-                    }
-                }
+    function xu(n) {
+        return function(t) {
+            return 1 - n(1 - t)
+        }
+    }
 
-                function su(n) {
-                    return n * n
-                }
+    function Mu(n) {
+        return function(t) {
+            return .5 * (.5 > t ? n(2 * t) : 2 - n(2 - 2 * t))
+        }
+    }
 
-                function hu(n) {
-                    return n * n * n
-                }
+    function _u(n) {
+        return n * n
+    }
 
-                function pu(n) {
-                    if (n <= 0) return 0;
-                    if (n >= 1) return 1;
-                    var t = n * n,
-                        e = t * n;
-                    return 4 * (n < .5 ? e : 3 * (n - t) + e - .75)
-                }
+    function bu(n) {
+        return n * n * n
+    }
 
-                function gu(n) {
-                    return 1 - Math.cos(n * Rn)
-                }
+    function wu(n) {
+        if (0 >= n) return 0;
+        if (n >= 1) return 1;
+        var t = n * n,
+            e = t * n;
+        return 4 * (.5 > n ? e : 3 * (n - t) + e - .75)
+    }
 
-                function vu(n) {
-                    return Math.pow(2, 10 * (n - 1))
-                }
+    function Su(n) {
+        return function(t) {
+            return Math.pow(t, n)
+        }
+    }
 
-                function du(n) {
-                    return 1 - Math.sqrt(1 - n * n)
-                }
+    function ku(n) {
+        return 1 - Math.cos(n * Ca)
+    }
 
-                function yu(n) {
-                    return n < 1 / 2.75 ? 7.5625 * n * n : n < 2 / 2.75 ? 7.5625 * (n -= 1.5 / 2.75) * n + .75 : n < 2.5 / 2.75 ? 7.5625 * (n -= 2.25 / 2.75) * n + .9375 : 7.5625 * (n -= 2.625 / 2.75) * n + .984375
-                }
+    function Eu(n) {
+        return Math.pow(2, 10 * (n - 1))
+    }
 
-                function mu(n, t) {
-                    return t -= n,
-                        function(e) {
-                            return Math.round(n + t * e)
-                        }
-                }
+    function Au(n) {
+        return 1 - Math.sqrt(1 - n * n)
+    }
 
-                function Mu(n) {
-                    var t, e, r, i = [n.a, n.b],
-                        u = [n.c, n.d],
-                        o = bu(i),
-                        a = xu(i, u),
-                        l = bu(((t = u)[0] += (r = -a) * (e = i)[0], t[1] += r * e[1], t)) || 0;
-                    i[0] * u[1] < u[0] * i[1] && (i[0] *= -1, i[1] *= -1, o *= -1, a *= -1), this.rotate = (o ? Math.atan2(i[1], i[0]) : Math.atan2(-u[0], u[1])) * Pn, this.translate = [n.e, n.f], this.scale = [o, l], this.skew = l ? Math.atan2(a, l) * Pn : 0
-                }
-
-                function xu(n, t) {
-                    return n[0] * t[0] + n[1] * t[1]
-                }
-
-                function bu(n) {
-                    var t = Math.sqrt(xu(n, n));
-                    return t && (n[0] /= t, n[1] /= t), t
-                }
-                u.ease = function(n) {
-                    var t = n.indexOf("-"),
-                        e = t >= 0 ? n.slice(0, t) : n,
-                        r = t >= 0 ? n.slice(t + 1) : "in";
-                    return e = ou.get(e) || uu, lu((r = au.get(r) || R)(e.apply(null, o.call(arguments, 1))))
-                }, u.interpolateHcl = function(n, t) {
-                    n = u.hcl(n), t = u.hcl(t);
-                    var e = n.h,
-                        r = n.c,
-                        i = n.l,
-                        o = t.h - e,
-                        a = t.c - r,
-                        l = t.l - i;
-                    isNaN(a) && (a = 0, r = isNaN(r) ? t.c : r);
-                    isNaN(o) ? (o = 0, e = isNaN(e) ? t.h : e) : o > 180 ? o -= 360 : o < -180 && (o += 360);
-                    return function(n) {
-                        return Qn(e + o * n, r + a * n, i + l * n) + ""
-                    }
-                }, u.interpolateHsl = function(n, t) {
-                    n = u.hsl(n), t = u.hsl(t);
-                    var e = n.h,
-                        r = n.s,
-                        i = n.l,
-                        o = t.h - e,
-                        a = t.s - r,
-                        l = t.l - i;
-                    isNaN(a) && (a = 0, r = isNaN(r) ? t.s : r);
-                    isNaN(o) ? (o = 0, e = isNaN(e) ? t.h : e) : o > 180 ? o -= 360 : o < -180 && (o += 360);
-                    return function(n) {
-                        return Wn(e + o * n, r + a * n, i + l * n) + ""
-                    }
-                }, u.interpolateLab = function(n, t) {
-                    n = u.lab(n), t = u.lab(t);
-                    var e = n.l,
-                        r = n.a,
-                        i = n.b,
-                        o = t.l - e,
-                        a = t.a - r,
-                        l = t.b - i;
-                    return function(n) {
-                        return rt(e + o * n, r + a * n, i + l * n) + ""
-                    }
-                }, u.interpolateRound = mu, u.transform = function(n) {
-                    var t = l.createElementNS(u.ns.prefix.svg, "g");
-                    return (u.transform = function(n) {
-                        if (null != n) {
-                            t.setAttribute("transform", n);
-                            var e = t.transform.baseVal.consolidate()
-                        }
-                        return new Mu(e ? e.matrix : wu)
-                    })(n)
-                }, Mu.prototype.toString = function() {
-                    return "translate(" + this.translate + ")rotate(" + this.rotate + ")skewX(" + this.skew + ")scale(" + this.scale + ")"
-                };
-                var wu = {
-                    a: 1,
-                    b: 0,
-                    c: 0,
-                    d: 1,
-                    e: 0,
-                    f: 0
-                };
+    function Cu(n, t) {
+        var e;
+        return arguments.length < 2 && (t = .45), arguments.length ? e = t / Aa * Math.asin(1 / n) : (n = 1, e = t / 4),
+            function(r) {
+                return 1 + n * Math.pow(2, -10 * r) * Math.sin((r - e) * Aa / t)
+            }
+    }
 
-                function _u(n) {
-                    return n.length ? n.pop() + "," : ""
-                }
+    function Nu(n) {
+        return n || (n = 1.70158),
+            function(t) {
+                return t * t * ((n + 1) * t - n)
+            }
+    }
 
-                function ku(n, t) {
-                    var e = [],
-                        r = [];
-                    return n = u.transform(n), t = u.transform(t),
-                        function(n, t, e, r) {
-                            if (n[0] !== t[0] || n[1] !== t[1]) {
-                                var i = e.push("translate(", null, ",", null, ")");
-                                r.push({
-                                    i: i - 4,
-                                    x: Qi(n[0], t[0])
-                                }, {
-                                    i: i - 2,
-                                    x: Qi(n[1], t[1])
-                                })
-                            } else(t[0] || t[1]) && e.push("translate(" + t + ")")
-                        }(n.translate, t.translate, e, r),
-                        function(n, t, e, r) {
-                            n !== t ? (n - t > 180 ? t += 360 : t - n > 180 && (n += 360), r.push({
-                                i: e.push(_u(e) + "rotate(", null, ")") - 2,
-                                x: Qi(n, t)
-                            })) : t && e.push(_u(e) + "rotate(" + t + ")")
-                        }(n.rotate, t.rotate, e, r),
-                        function(n, t, e, r) {
-                            n !== t ? r.push({
-                                i: e.push(_u(e) + "skewX(", null, ")") - 2,
-                                x: Qi(n, t)
-                            }) : t && e.push(_u(e) + "skewX(" + t + ")")
-                        }(n.skew, t.skew, e, r),
-                        function(n, t, e, r) {
-                            if (n[0] !== t[0] || n[1] !== t[1]) {
-                                var i = e.push(_u(e) + "scale(", null, ",", null, ")");
-                                r.push({
-                                    i: i - 4,
-                                    x: Qi(n[0], t[0])
-                                }, {
-                                    i: i - 2,
-                                    x: Qi(n[1], t[1])
-                                })
-                            } else 1 === t[0] && 1 === t[1] || e.push(_u(e) + "scale(" + t + ")")
-                        }(n.scale, t.scale, e, r), n = t = null,
-                        function(n) {
-                            for (var t, i = -1, u = r.length; ++i < u;) e[(t = r[i]).i] = t.x(n);
-                            return e.join("")
-                        }
-                }
+    function zu(n) {
+        return 1 / 2.75 > n ? 7.5625 * n * n : 2 / 2.75 > n ? 7.5625 * (n -= 1.5 / 2.75) * n + .75 : 2.5 / 2.75 > n ? 7.5625 * (n -= 2.25 / 2.75) * n + .9375 : 7.5625 * (n -= 2.625 / 2.75) * n + .984375
+    }
 
-                function Su(n, t) {
-                    return t = (t -= n = +n) || 1 / t,
-                        function(e) {
-                            return (e - n) / t
-                        }
-                }
+    function Lu(n, t) {
+        n = Bo.hcl(n), t = Bo.hcl(t);
+        var e = n.h,
+            r = n.c,
+            u = n.l,
+            i = t.h - e,
+            o = t.c - r,
+            a = t.l - u;
+        return isNaN(o) && (o = 0, r = isNaN(r) ? t.c : r), isNaN(i) ? (i = 0, e = isNaN(e) ? t.h : e) : i > 180 ? i -= 360 : -180 > i && (i += 360),
+            function(n) {
+                return lt(e + i * n, r + o * n, u + a * n) + ""
+            }
+    }
 
-                function Nu(n, t) {
-                    return t = (t -= n = +n) || 1 / t,
-                        function(e) {
-                            return Math.max(0, Math.min(1, (e - n) / t))
-                        }
-                }
+    function Tu(n, t) {
+        n = Bo.hsl(n), t = Bo.hsl(t);
+        var e = n.h,
+            r = n.s,
+            u = n.l,
+            i = t.h - e,
+            o = t.s - r,
+            a = t.l - u;
+        return isNaN(o) && (o = 0, r = isNaN(r) ? t.s : r), isNaN(i) ? (i = 0, e = isNaN(e) ? t.h : e) : i > 180 ? i -= 360 : -180 > i && (i += 360),
+            function(n) {
+                return at(e + i * n, r + o * n, u + a * n) + ""
+            }
+    }
 
-                function Eu(n) {
-                    for (var t = n.source, e = n.target, r = function(n, t) {
-                            if (n === t) return n;
-                            var e = Au(n),
-                                r = Au(t),
-                                i = e.pop(),
-                                u = r.pop(),
-                                o = null;
-                            for (; i === u;) o = i, i = e.pop(), u = r.pop();
-                            return o
-                        }(t, e), i = [t]; t !== r;) t = t.parent, i.push(t);
-                    for (var u = i.length; e !== r;) i.splice(u, 0, e), e = e.parent;
-                    return i
-                }
+    function qu(n, t) {
+        n = Bo.lab(n), t = Bo.lab(t);
+        var e = n.l,
+            r = n.a,
+            u = n.b,
+            i = t.l - e,
+            o = t.a - r,
+            a = t.b - u;
+        return function(n) {
+            return ft(e + i * n, r + o * n, u + a * n) + ""
+        }
+    }
 
-                function Au(n) {
-                    for (var t = [], e = n.parent; null != e;) t.push(n), n = e, e = e.parent;
-                    return t.push(n), t
-                }
+    function Ru(n, t) {
+        return t -= n,
+            function(e) {
+                return Math.round(n + t * e)
+            }
+    }
 
-                function Cu(n) {
-                    n.fixed |= 2
-                }
+    function Du(n) {
+        var t = [n.a, n.b],
+            e = [n.c, n.d],
+            r = Uu(t),
+            u = Pu(t, e),
+            i = Uu(ju(e, t, -u)) || 0;
+        t[0] * e[1] < e[0] * t[1] && (t[0] *= -1, t[1] *= -1, r *= -1, u *= -1), this.rotate = (r ? Math.atan2(t[1], t[0]) : Math.atan2(-e[0], e[1])) * Ta, this.translate = [n.e, n.f], this.scale = [r, i], this.skew = i ? Math.atan2(u, i) * Ta : 0
+    }
 
-                function zu(n) {
-                    n.fixed &= -7
-                }
+    function Pu(n, t) {
+        return n[0] * t[0] + n[1] * t[1]
+    }
 
-                function Lu(n) {
-                    n.fixed |= 4, n.px = n.x, n.py = n.y
-                }
+    function Uu(n) {
+        var t = Math.sqrt(Pu(n, n));
+        return t && (n[0] /= t, n[1] /= t), t
+    }
 
-                function qu(n) {
-                    n.fixed &= -5
-                }
-                u.interpolateTransform = ku, u.layout = {}, u.layout.bundle = function() {
-                    return function(n) {
-                        for (var t = [], e = -1, r = n.length; ++e < r;) t.push(Eu(n[e]));
-                        return t
-                    }
-                }, u.layout.chord = function() {
-                    var n, t, e, r, i, o, a, l = {},
-                        c = 0;
-
-                    function f() {
-                        var l, f, h, p, g, v = {},
-                            d = [],
-                            y = u.range(r),
-                            m = [];
-                        for (n = [], t = [], l = 0, p = -1; ++p < r;) {
-                            for (f = 0, g = -1; ++g < r;) f += e[p][g];
-                            d.push(f), m.push(u.range(r)), l += f
-                        }
-                        for (i && y.sort((function(n, t) {
-                                return i(d[n], d[t])
-                            })), o && m.forEach((function(n, t) {
-                                n.sort((function(n, r) {
-                                    return o(e[t][n], e[t][r])
-                                }))
-                            })), l = (qn - c * r) / l, f = 0, p = -1; ++p < r;) {
-                            for (h = f, g = -1; ++g < r;) {
-                                var M = y[p],
-                                    x = m[M][g],
-                                    b = e[M][x],
-                                    w = f,
-                                    _ = f += b * l;
-                                v[M + "-" + x] = {
-                                    index: M,
-                                    subindex: x,
-                                    startAngle: w,
-                                    endAngle: _,
-                                    value: b
-                                }
-                            }
-                            t[M] = {
-                                index: M,
-                                startAngle: h,
-                                endAngle: f,
-                                value: d[M]
-                            }, f += c
-                        }
-                        for (p = -1; ++p < r;)
-                            for (g = p - 1; ++g < r;) {
-                                var k = v[p + "-" + g],
-                                    S = v[g + "-" + p];
-                                (k.value || S.value) && n.push(k.value < S.value ? {
-                                    source: S,
-                                    target: k
-                                } : {
-                                    source: k,
-                                    target: S
-                                })
-                            }
-                        a && s()
-                    }
+    function ju(n, t, e) {
+        return n[0] += e * t[0], n[1] += e * t[1], n
+    }
 
-                    function s() {
-                        n.sort((function(n, t) {
-                            return a((n.source.value + n.target.value) / 2, (t.source.value + t.target.value) / 2)
-                        }))
-                    }
-                    return l.matrix = function(i) {
-                        return arguments.length ? (r = (e = i) && e.length, n = t = null, l) : e
-                    }, l.padding = function(e) {
-                        return arguments.length ? (c = e, n = t = null, l) : c
-                    }, l.sortGroups = function(e) {
-                        return arguments.length ? (i = e, n = t = null, l) : i
-                    }, l.sortSubgroups = function(t) {
-                        return arguments.length ? (o = t, n = null, l) : o
-                    }, l.sortChords = function(t) {
-                        return arguments.length ? (a = t, n && s(), l) : a
-                    }, l.chords = function() {
-                        return n || f(), n
-                    }, l.groups = function() {
-                        return t || f(), t
-                    }, l
-                }, u.layout.force = function() {
-                    var n, t, e, r, i, o, a = {},
-                        l = u.dispatch("start", "tick", "end"),
-                        c = [1, 1],
-                        f = .9,
-                        s = Tu,
-                        h = Ru,
-                        p = -30,
-                        g = Du,
-                        v = .1,
-                        d = .64,
-                        y = [],
-                        m = [];
-
-                    function M(n) {
-                        return function(t, e, r, i) {
-                            if (t.point !== n) {
-                                var u = t.cx - n.x,
-                                    o = t.cy - n.y,
-                                    a = i - e,
-                                    l = u * u + o * o;
-                                if (a * a / d < l) {
-                                    if (l < g) {
-                                        var c = t.charge / l;
-                                        n.px -= u * c, n.py -= o * c
-                                    }
-                                    return !0
-                                }
-                                if (t.point && l && l < g) {
-                                    c = t.pointCharge / l;
-                                    n.px -= u * c, n.py -= o * c
-                                }
-                            }
-                            return !t.charge
-                        }
-                    }
+    function Fu(n, t) {
+        var e, r = [],
+            u = [],
+            i = Bo.transform(n),
+            o = Bo.transform(t),
+            a = i.translate,
+            c = o.translate,
+            l = i.rotate,
+            s = o.rotate,
+            f = i.skew,
+            h = o.skew,
+            g = i.scale,
+            p = o.scale;
+        return a[0] != c[0] || a[1] != c[1] ? (r.push("translate(", null, ",", null, ")"), u.push({
+                i: 1,
+                x: pu(a[0], c[0])
+            }, {
+                i: 3,
+                x: pu(a[1], c[1])
+            })) : c[0] || c[1] ? r.push("translate(" + c + ")") : r.push(""), l != s ? (l - s > 180 ? s += 360 : s - l > 180 && (l += 360), u.push({
+                i: r.push(r.pop() + "rotate(", null, ")") - 2,
+                x: pu(l, s)
+            })) : s && r.push(r.pop() + "rotate(" + s + ")"), f != h ? u.push({
+                i: r.push(r.pop() + "skewX(", null, ")") - 2,
+                x: pu(f, h)
+            }) : h && r.push(r.pop() + "skewX(" + h + ")"), g[0] != p[0] || g[1] != p[1] ? (e = r.push(r.pop() + "scale(", null, ",", null, ")"), u.push({
+                i: e - 4,
+                x: pu(g[0], p[0])
+            }, {
+                i: e - 2,
+                x: pu(g[1], p[1])
+            })) : (1 != p[0] || 1 != p[1]) && r.push(r.pop() + "scale(" + p + ")"), e = u.length,
+            function(n) {
+                for (var t, i = -1; ++i < e;) r[(t = u[i]).i] = t.x(n);
+                return r.join("")
+            }
+    }
 
-                    function x(n) {
-                        n.px = u.event.x, n.py = u.event.y, a.resume()
-                    }
-                    return a.tick = function() {
-                        if ((e *= .99) < .005) return n = null, l.end({
-                            type: "end",
-                            alpha: e = 0
-                        }), !0;
-                        var t, a, s, h, g, d, x, b, w, _ = y.length,
-                            k = m.length;
-                        for (a = 0; a < k; ++a) h = (s = m[a]).source, (d = (b = (g = s.target).x - h.x) * b + (w = g.y - h.y) * w) && (b *= d = e * i[a] * ((d = Math.sqrt(d)) - r[a]) / d, w *= d, g.x -= b * (x = h.weight + g.weight ? h.weight / (h.weight + g.weight) : .5), g.y -= w * x, h.x += b * (x = 1 - x), h.y += w * x);
-                        if ((x = e * v) && (b = c[0] / 2, w = c[1] / 2, a = -1, x))
-                            for (; ++a < _;)(s = y[a]).x += (b - s.x) * x, s.y += (w - s.y) * x;
-                        if (p)
-                            for (! function n(t, e, r) {
-                                    var i = 0,
-                                        u = 0;
-                                    if (t.charge = 0, !t.leaf)
-                                        for (var o, a = t.nodes, l = a.length, c = -1; ++c < l;) null != (o = a[c]) && (n(o, e, r), t.charge += o.charge, i += o.charge * o.cx, u += o.charge * o.cy);
-                                    if (t.point) {
-                                        t.leaf || (t.point.x += Math.random() - .5, t.point.y += Math.random() - .5);
-                                        var f = e * r[t.point.index];
-                                        t.charge += t.pointCharge = f, i += f * t.point.x, u += f * t.point.y
-                                    }
-                                    t.cx = i / t.charge, t.cy = u / t.charge
-                                }(t = u.geom.quadtree(y), e, o), a = -1; ++a < _;)(s = y[a]).fixed || t.visit(M(s));
-                        for (a = -1; ++a < _;)(s = y[a]).fixed ? (s.x = s.px, s.y = s.py) : (s.x -= (s.px - (s.px = s.x)) * f, s.y -= (s.py - (s.py = s.y)) * f);
-                        l.tick({
-                            type: "tick",
-                            alpha: e
-                        })
-                    }, a.nodes = function(n) {
-                        return arguments.length ? (y = n, a) : y
-                    }, a.links = function(n) {
-                        return arguments.length ? (m = n, a) : m
-                    }, a.size = function(n) {
-                        return arguments.length ? (c = n, a) : c
-                    }, a.linkDistance = function(n) {
-                        return arguments.length ? (s = "function" == typeof n ? n : +n, a) : s
-                    }, a.distance = a.linkDistance, a.linkStrength = function(n) {
-                        return arguments.length ? (h = "function" == typeof n ? n : +n, a) : h
-                    }, a.friction = function(n) {
-                        return arguments.length ? (f = +n, a) : f
-                    }, a.charge = function(n) {
-                        return arguments.length ? (p = "function" == typeof n ? n : +n, a) : p
-                    }, a.chargeDistance = function(n) {
-                        return arguments.length ? (g = n * n, a) : Math.sqrt(g)
-                    }, a.gravity = function(n) {
-                        return arguments.length ? (v = +n, a) : v
-                    }, a.theta = function(n) {
-                        return arguments.length ? (d = n * n, a) : Math.sqrt(d)
-                    }, a.alpha = function(t) {
-                        return arguments.length ? (t = +t, e ? t > 0 ? e = t : (n.c = null, n.t = NaN, n = null, l.end({
-                            type: "end",
-                            alpha: e = 0
-                        })) : t > 0 && (l.start({
-                            type: "start",
-                            alpha: e = t
-                        }), n = Et(a.tick)), a) : e
-                    }, a.start = function() {
-                        var n, t, e, u = y.length,
-                            l = m.length,
-                            f = c[0],
-                            g = c[1];
-                        for (n = 0; n < u; ++n)(e = y[n]).index = n, e.weight = 0;
-                        for (n = 0; n < l; ++n) "number" == typeof(e = m[n]).source && (e.source = y[e.source]), "number" == typeof e.target && (e.target = y[e.target]), ++e.source.weight, ++e.target.weight;
-                        for (n = 0; n < u; ++n) e = y[n], isNaN(e.x) && (e.x = v("x", f)), isNaN(e.y) && (e.y = v("y", g)), isNaN(e.px) && (e.px = e.x), isNaN(e.py) && (e.py = e.y);
-                        if (r = [], "function" == typeof s)
-                            for (n = 0; n < l; ++n) r[n] = +s.call(this, m[n], n);
-                        else
-                            for (n = 0; n < l; ++n) r[n] = s;
-                        if (i = [], "function" == typeof h)
-                            for (n = 0; n < l; ++n) i[n] = +h.call(this, m[n], n);
-                        else
-                            for (n = 0; n < l; ++n) i[n] = h;
-                        if (o = [], "function" == typeof p)
-                            for (n = 0; n < u; ++n) o[n] = +p.call(this, y[n], n);
-                        else
-                            for (n = 0; n < u; ++n) o[n] = p;
-
-                        function v(e, r) {
-                            if (!t) {
-                                for (t = new Array(u), c = 0; c < u; ++c) t[c] = [];
-                                for (c = 0; c < l; ++c) {
-                                    var i = m[c];
-                                    t[i.source.index].push(i.target), t[i.target.index].push(i.source)
-                                }
-                            }
-                            for (var o, a = t[n], c = -1, f = a.length; ++c < f;)
-                                if (!isNaN(o = a[c][e])) return o;
-                            return Math.random() * r
-                        }
-                        return a.resume()
-                    }, a.resume = function() {
-                        return a.alpha(.1)
-                    }, a.stop = function() {
-                        return a.alpha(0)
-                    }, a.drag = function() {
-                        if (t || (t = u.behavior.drag().origin(R).on("dragstart.force", Cu).on("drag.force", x).on("dragend.force", zu)), !arguments.length) return t;
-                        this.on("mouseover.force", Lu).on("mouseout.force", qu).call(t)
-                    }, u.rebind(a, l, "on")
-                };
-                var Tu = 20,
-                    Ru = 1,
-                    Du = 1 / 0;
+    function Hu(n, t) {
+        return t = (t -= n = +n) || 1 / t,
+            function(e) {
+                return (e - n) / t
+            }
+    }
 
-                function Pu(n, t) {
-                    return u.rebind(n, t, "sort", "children", "value"), n.nodes = n, n.links = Iu, n
-                }
+    function Ou(n, t) {
+        return t = (t -= n = +n) || 1 / t,
+            function(e) {
+                return Math.max(0, Math.min(1, (e - n) / t))
+            }
+    }
 
-                function Uu(n, t) {
-                    for (var e = [n]; null != (n = e.pop());)
-                        if (t(n), (i = n.children) && (r = i.length))
-                            for (var r, i; --r >= 0;) e.push(i[r])
-                }
+    function Yu(n) {
+        for (var t = n.source, e = n.target, r = Zu(t, e), u = [t]; t !== r;) t = t.parent, u.push(t);
+        for (var i = u.length; e !== r;) u.splice(i, 0, e), e = e.parent;
+        return u
+    }
 
-                function ju(n, t) {
-                    for (var e = [n], r = []; null != (n = e.pop());)
-                        if (r.push(n), (u = n.children) && (i = u.length))
-                            for (var i, u, o = -1; ++o < i;) e.push(u[o]);
-                    for (; null != (n = r.pop());) t(n)
-                }
+    function Iu(n) {
+        for (var t = [], e = n.parent; null != e;) t.push(n), n = e, e = e.parent;
+        return t.push(n), t
+    }
 
-                function Fu(n) {
-                    return n.children
-                }
+    function Zu(n, t) {
+        if (n === t) return n;
+        for (var e = Iu(n), r = Iu(t), u = e.pop(), i = r.pop(), o = null; u === i;) o = u, u = e.pop(), i = r.pop();
+        return o
+    }
 
-                function Hu(n) {
-                    return n.value
-                }
+    function Vu(n) {
+        n.fixed |= 2
+    }
 
-                function Ou(n, t) {
-                    return t.value - n.value
-                }
+    function Xu(n) {
+        n.fixed &= -7
+    }
 
-                function Iu(n) {
-                    return u.merge(n.map((function(n) {
-                        return (n.children || []).map((function(t) {
-                            return {
-                                source: n,
-                                target: t
-                            }
-                        }))
-                    })))
-                }
-                u.layout.hierarchy = function() {
-                    var n = Ou,
-                        t = Fu,
-                        e = Hu;
-
-                    function r(i) {
-                        var u, o = [i],
-                            a = [];
-                        for (i.depth = 0; null != (u = o.pop());)
-                            if (a.push(u), (c = t.call(r, u, u.depth)) && (l = c.length)) {
-                                for (var l, c, f; --l >= 0;) o.push(f = c[l]), f.parent = u, f.depth = u.depth + 1;
-                                e && (u.value = 0), u.children = c
-                            } else e && (u.value = +e.call(r, u, u.depth) || 0), delete u.children;
-                        return ju(i, (function(t) {
-                            var r, i;
-                            n && (r = t.children) && r.sort(n), e && (i = t.parent) && (i.value += t.value)
-                        })), a
-                    }
-                    return r.sort = function(t) {
-                        return arguments.length ? (n = t, r) : n
-                    }, r.children = function(n) {
-                        return arguments.length ? (t = n, r) : t
-                    }, r.value = function(n) {
-                        return arguments.length ? (e = n, r) : e
-                    }, r.revalue = function(n) {
-                        return e && (Uu(n, (function(n) {
-                            n.children && (n.value = 0)
-                        })), ju(n, (function(n) {
-                            var t;
-                            n.children || (n.value = +e.call(r, n, n.depth) || 0), (t = n.parent) && (t.value += n.value)
-                        }))), n
-                    }, r
-                }, u.layout.partition = function() {
-                    var n = u.layout.hierarchy(),
-                        t = [1, 1];
-
-                    function e(e, r) {
-                        var i = n.call(this, e, r);
-                        return function n(t, e, r, i) {
-                            var u = t.children;
-                            if (t.x = e, t.y = t.depth * i, t.dx = r, t.dy = i, u && (o = u.length)) {
-                                var o, a, l, c = -1;
-                                for (r = t.value ? r / t.value : 0; ++c < o;) n(a = u[c], e, l = a.value * r, i), e += l
-                            }
-                        }(i[0], 0, t[0], t[1] / function n(t) {
-                            var e = t.children,
-                                r = 0;
-                            if (e && (i = e.length))
-                                for (var i, u = -1; ++u < i;) r = Math.max(r, n(e[u]));
-                            return 1 + r
-                        }(i[0])), i
-                    }
-                    return e.size = function(n) {
-                        return arguments.length ? (t = n, e) : t
-                    }, Pu(e, n)
-                }, u.layout.pie = function() {
-                    var n = Number,
-                        t = Yu,
-                        e = 0,
-                        r = qn,
-                        i = 0;
-
-                    function o(a) {
-                        var l, c = a.length,
-                            f = a.map((function(t, e) {
-                                return +n.call(o, t, e)
-                            })),
-                            s = +("function" == typeof e ? e.apply(this, arguments) : e),
-                            h = ("function" == typeof r ? r.apply(this, arguments) : r) - s,
-                            p = Math.min(Math.abs(h) / c, +("function" == typeof i ? i.apply(this, arguments) : i)),
-                            g = p * (h < 0 ? -1 : 1),
-                            v = u.sum(f),
-                            d = v ? (h - c * g) / v : 0,
-                            y = u.range(c),
-                            m = [];
-                        return null != t && y.sort(t === Yu ? function(n, t) {
-                            return f[t] - f[n]
-                        } : function(n, e) {
-                            return t(a[n], a[e])
-                        }), y.forEach((function(n) {
-                            m[n] = {
-                                data: a[n],
-                                value: l = f[n],
-                                startAngle: s,
-                                endAngle: s += l * d + g,
-                                padAngle: p
-                            }
-                        })), m
-                    }
-                    return o.value = function(t) {
-                        return arguments.length ? (n = t, o) : n
-                    }, o.sort = function(n) {
-                        return arguments.length ? (t = n, o) : t
-                    }, o.startAngle = function(n) {
-                        return arguments.length ? (e = n, o) : e
-                    }, o.endAngle = function(n) {
-                        return arguments.length ? (r = n, o) : r
-                    }, o.padAngle = function(n) {
-                        return arguments.length ? (i = n, o) : i
-                    }, o
-                };
-                var Yu = {};
+    function $u(n) {
+        n.fixed |= 4, n.px = n.x, n.py = n.y
+    }
 
-                function Zu(n) {
-                    return n.x
-                }
+    function Bu(n) {
+        n.fixed &= -5
+    }
 
-                function Vu(n) {
-                    return n.y
-                }
+    function Wu(n, t, e) {
+        var r = 0,
+            u = 0;
+        if (n.charge = 0, !n.leaf)
+            for (var i, o = n.nodes, a = o.length, c = -1; ++c < a;) i = o[c], null != i && (Wu(i, t, e), n.charge += i.charge, r += i.charge * i.cx, u += i.charge * i.cy);
+        if (n.point) {
+            n.leaf || (n.point.x += Math.random() - .5, n.point.y += Math.random() - .5);
+            var l = t * e[n.point.index];
+            n.charge += n.pointCharge = l, r += l * n.point.x, u += l * n.point.y
+        }
+        n.cx = r / n.charge, n.cy = u / n.charge
+    }
 
-                function Xu(n, t, e) {
-                    n.y0 = t, n.y = e
-                }
-                u.layout.stack = function() {
-                    var n = R,
-                        t = Ju,
-                        e = Wu,
-                        r = Xu,
-                        i = Zu,
-                        o = Vu;
-
-                    function a(l, c) {
-                        if (!(p = l.length)) return l;
-                        var f = l.map((function(t, e) {
-                                return n.call(a, t, e)
-                            })),
-                            s = f.map((function(n) {
-                                return n.map((function(n, t) {
-                                    return [i.call(a, n, t), o.call(a, n, t)]
-                                }))
-                            })),
-                            h = t.call(a, s, c);
-                        f = u.permute(f, h), s = u.permute(s, h);
-                        var p, g, v, d, y = e.call(a, s, c),
-                            m = f[0].length;
-                        for (v = 0; v < m; ++v)
-                            for (r.call(a, f[0][v], d = y[v], s[0][v][1]), g = 1; g < p; ++g) r.call(a, f[g][v], d += s[g - 1][v][1], s[g][v][1]);
-                        return l
-                    }
-                    return a.values = function(t) {
-                        return arguments.length ? (n = t, a) : n
-                    }, a.order = function(n) {
-                        return arguments.length ? (t = "function" == typeof n ? n : $u.get(n) || Ju, a) : t
-                    }, a.offset = function(n) {
-                        return arguments.length ? (e = "function" == typeof n ? n : Bu.get(n) || Wu, a) : e
-                    }, a.x = function(n) {
-                        return arguments.length ? (i = n, a) : i
-                    }, a.y = function(n) {
-                        return arguments.length ? (o = n, a) : o
-                    }, a.out = function(n) {
-                        return arguments.length ? (r = n, a) : r
-                    }, a
-                };
-                var $u = u.map({
-                        "inside-out": function(n) {
-                            var t, e, r = n.length,
-                                i = n.map(Gu),
-                                o = n.map(Ku),
-                                a = u.range(r).sort((function(n, t) {
-                                    return i[n] - i[t]
-                                })),
-                                l = 0,
-                                c = 0,
-                                f = [],
-                                s = [];
-                            for (t = 0; t < r; ++t) e = a[t], l < c ? (l += o[e], f.push(e)) : (c += o[e], s.push(e));
-                            return s.reverse().concat(f)
-                        },
-                        reverse: function(n) {
-                            return u.range(n.length).reverse()
-                        },
-                        default: Ju
-                    }),
-                    Bu = u.map({
-                        silhouette: function(n) {
-                            var t, e, r, i = n.length,
-                                u = n[0].length,
-                                o = [],
-                                a = 0,
-                                l = [];
-                            for (e = 0; e < u; ++e) {
-                                for (t = 0, r = 0; t < i; t++) r += n[t][e][1];
-                                r > a && (a = r), o.push(r)
-                            }
-                            for (e = 0; e < u; ++e) l[e] = (a - o[e]) / 2;
-                            return l
-                        },
-                        wiggle: function(n) {
-                            var t, e, r, i, u, o, a, l, c, f = n.length,
-                                s = n[0],
-                                h = s.length,
-                                p = [];
-                            for (p[0] = l = c = 0, e = 1; e < h; ++e) {
-                                for (t = 0, i = 0; t < f; ++t) i += n[t][e][1];
-                                for (t = 0, u = 0, a = s[e][0] - s[e - 1][0]; t < f; ++t) {
-                                    for (r = 0, o = (n[t][e][1] - n[t][e - 1][1]) / (2 * a); r < t; ++r) o += (n[r][e][1] - n[r][e - 1][1]) / a;
-                                    u += o * n[t][e][1]
-                                }
-                                p[e] = l -= i ? u / i * a : 0, l < c && (c = l)
-                            }
-                            for (e = 0; e < h; ++e) p[e] -= c;
-                            return p
-                        },
-                        expand: function(n) {
-                            var t, e, r, i = n.length,
-                                u = n[0].length,
-                                o = 1 / i,
-                                a = [];
-                            for (e = 0; e < u; ++e) {
-                                for (t = 0, r = 0; t < i; t++) r += n[t][e][1];
-                                if (r)
-                                    for (t = 0; t < i; t++) n[t][e][1] /= r;
-                                else
-                                    for (t = 0; t < i; t++) n[t][e][1] = o
-                            }
-                            for (e = 0; e < u; ++e) a[e] = 0;
-                            return a
-                        },
-                        zero: Wu
-                    });
+    function Ju(n, t) {
+        return Bo.rebind(n, t, "sort", "children", "value"), n.nodes = n, n.links = ei, n
+    }
 
-                function Ju(n) {
-                    return u.range(n.length)
-                }
+    function Gu(n, t) {
+        for (var e = [n]; null != (n = e.pop());)
+            if (t(n), (u = n.children) && (r = u.length))
+                for (var r, u; --r >= 0;) e.push(u[r])
+    }
 
-                function Wu(n) {
-                    for (var t = -1, e = n[0].length, r = []; ++t < e;) r[t] = 0;
-                    return r
-                }
+    function Ku(n, t) {
+        for (var e = [n], r = []; null != (n = e.pop());)
+            if (r.push(n), (i = n.children) && (u = i.length))
+                for (var u, i, o = -1; ++o < u;) e.push(i[o]);
+        for (; null != (n = r.pop());) t(n)
+    }
 
-                function Gu(n) {
-                    for (var t, e = 1, r = 0, i = n[0][1], u = n.length; e < u; ++e)(t = n[e][1]) > i && (r = e, i = t);
-                    return r
-                }
+    function Qu(n) {
+        return n.children
+    }
 
-                function Ku(n) {
-                    return n.reduce(Qu, 0)
-                }
+    function ni(n) {
+        return n.value
+    }
 
-                function Qu(n, t) {
-                    return n + t[1]
-                }
+    function ti(n, t) {
+        return t.value - n.value
+    }
 
-                function no(n, t) {
-                    return to(n, Math.ceil(Math.log(t.length) / Math.LN2 + 1))
+    function ei(n) {
+        return Bo.merge(n.map(function(n) {
+            return (n.children || []).map(function(t) {
+                return {
+                    source: n,
+                    target: t
                 }
+            })
+        }))
+    }
 
-                function to(n, t) {
-                    for (var e = -1, r = +n[0], i = (n[1] - r) / t, u = []; ++e <= t;) u[e] = i * e + r;
-                    return u
-                }
+    function ri(n) {
+        return n.x
+    }
 
-                function eo(n) {
-                    return [u.min(n), u.max(n)]
-                }
+    function ui(n) {
+        return n.y
+    }
 
-                function ro(n, t) {
-                    return n.value - t.value
-                }
+    function ii(n, t, e) {
+        n.y0 = t, n.y = e
+    }
 
-                function io(n, t) {
-                    var e = n._pack_next;
-                    n._pack_next = t, t._pack_prev = n, t._pack_next = e, e._pack_prev = t
-                }
+    function oi(n) {
+        return Bo.range(n.length)
+    }
 
-                function uo(n, t) {
-                    n._pack_next = t, t._pack_prev = n
-                }
+    function ai(n) {
+        for (var t = -1, e = n[0].length, r = []; ++t < e;) r[t] = 0;
+        return r
+    }
 
-                function oo(n, t) {
-                    var e = t.x - n.x,
-                        r = t.y - n.y,
-                        i = n.r + t.r;
-                    return .999 * i * i > e * e + r * r
-                }
+    function ci(n) {
+        for (var t, e = 1, r = 0, u = n[0][1], i = n.length; i > e; ++e)(t = n[e][1]) > u && (r = e, u = t);
+        return r
+    }
 
-                function ao(n) {
-                    if ((t = n.children) && (l = t.length)) {
-                        var t, e, r, i, u, o, a, l, c = 1 / 0,
-                            f = -1 / 0,
-                            s = 1 / 0,
-                            h = -1 / 0;
-                        if (t.forEach(lo), (e = t[0]).x = -e.r, e.y = 0, M(e), l > 1 && ((r = t[1]).x = r.r, r.y = 0, M(r), l > 2))
-                            for (fo(e, r, i = t[2]), M(i), io(e, i), e._pack_prev = i, io(i, r), r = e._pack_next, u = 3; u < l; u++) {
-                                fo(e, r, i = t[u]);
-                                var p = 0,
-                                    g = 1,
-                                    v = 1;
-                                for (o = r._pack_next; o !== r; o = o._pack_next, g++)
-                                    if (oo(o, i)) {
-                                        p = 1;
-                                        break
-                                    } if (1 == p)
-                                    for (a = e._pack_prev; a !== o._pack_prev && !oo(a, i); a = a._pack_prev, v++);
-                                p ? (g < v || g == v && r.r < e.r ? uo(e, r = o) : uo(e = a, r), u--) : (io(e, i), r = i, M(i))
-                            }
-                        var d = (c + f) / 2,
-                            y = (s + h) / 2,
-                            m = 0;
-                        for (u = 0; u < l; u++)(i = t[u]).x -= d, i.y -= y, m = Math.max(m, i.r + Math.sqrt(i.x * i.x + i.y * i.y));
-                        n.r = m, t.forEach(co)
-                    }
+    function li(n) {
+        return n.reduce(si, 0)
+    }
 
-                    function M(n) {
-                        c = Math.min(n.x - n.r, c), f = Math.max(n.x + n.r, f), s = Math.min(n.y - n.r, s), h = Math.max(n.y + n.r, h)
-                    }
-                }
+    function si(n, t) {
+        return n + t[1]
+    }
 
-                function lo(n) {
-                    n._pack_next = n._pack_prev = n
-                }
+    function fi(n, t) {
+        return hi(n, Math.ceil(Math.log(t.length) / Math.LN2 + 1))
+    }
 
-                function co(n) {
-                    delete n._pack_next, delete n._pack_prev
-                }
+    function hi(n, t) {
+        for (var e = -1, r = +n[0], u = (n[1] - r) / t, i = []; ++e <= t;) i[e] = u * e + r;
+        return i
+    }
 
-                function fo(n, t, e) {
-                    var r = n.r + e.r,
-                        i = t.x - n.x,
-                        u = t.y - n.y;
-                    if (r && (i || u)) {
-                        var o = t.r + e.r,
-                            a = i * i + u * u,
-                            l = .5 + ((r *= r) - (o *= o)) / (2 * a),
-                            c = Math.sqrt(Math.max(0, 2 * o * (r + a) - (r -= a) * r - o * o)) / (2 * a);
-                        e.x = n.x + l * i + c * u, e.y = n.y + l * u - c * i
-                    } else e.x = n.x + r, e.y = n.y
-                }
+    function gi(n) {
+        return [Bo.min(n), Bo.max(n)]
+    }
 
-                function so(n, t) {
-                    return n.parent == t.parent ? 1 : 2
-                }
+    function pi(n, t) {
+        return n.value - t.value
+    }
 
-                function ho(n) {
-                    var t = n.children;
-                    return t.length ? t[0] : n.t
-                }
+    function vi(n, t) {
+        var e = n._pack_next;
+        n._pack_next = t, t._pack_prev = n, t._pack_next = e, e._pack_prev = t
+    }
 
-                function po(n) {
-                    var t, e = n.children;
-                    return (t = e.length) ? e[t - 1] : n.t
-                }
+    function di(n, t) {
+        n._pack_next = t, t._pack_prev = n
+    }
 
-                function go(n, t, e) {
-                    var r = e / (t.i - n.i);
-                    t.c -= r, t.s += e, n.c += r, t.z += e, t.m += e
-                }
+    function mi(n, t) {
+        var e = t.x - n.x,
+            r = t.y - n.y,
+            u = n.r + t.r;
+        return .999 * u * u > e * e + r * r
+    }
 
-                function vo(n, t, e) {
-                    return n.a.parent === t.parent ? n.a : e
-                }
+    function yi(n) {
+        function t(n) {
+            s = Math.min(n.x - n.r, s), f = Math.max(n.x + n.r, f), h = Math.min(n.y - n.r, h), g = Math.max(n.y + n.r, g)
+        }
+        if ((e = n.children) && (l = e.length)) {
+            var e, r, u, i, o, a, c, l, s = 1 / 0,
+                f = -1 / 0,
+                h = 1 / 0,
+                g = -1 / 0;
+            if (e.forEach(xi), r = e[0], r.x = -r.r, r.y = 0, t(r), l > 1 && (u = e[1], u.x = u.r, u.y = 0, t(u), l > 2))
+                for (i = e[2], bi(r, u, i), t(i), vi(r, i), r._pack_prev = i, vi(i, u), u = r._pack_next, o = 3; l > o; o++) {
+                    bi(r, u, i = e[o]);
+                    var p = 0,
+                        v = 1,
+                        d = 1;
+                    for (a = u._pack_next; a !== u; a = a._pack_next, v++)
+                        if (mi(a, i)) {
+                            p = 1;
+                            break
+                        } if (1 == p)
+                        for (c = r._pack_prev; c !== a._pack_prev && !mi(c, i); c = c._pack_prev, d++);
+                    p ? (d > v || v == d && u.r < r.r ? di(r, u = a) : di(r = c, u), o--) : (vi(r, i), u = i, t(i))
+                }
+            var m = (s + f) / 2,
+                y = (h + g) / 2,
+                x = 0;
+            for (o = 0; l > o; o++) i = e[o], i.x -= m, i.y -= y, x = Math.max(x, i.r + Math.sqrt(i.x * i.x + i.y * i.y));
+            n.r = x, e.forEach(Mi)
+        }
+    }
 
-                function yo(n) {
-                    return {
-                        x: n.x,
-                        y: n.y,
-                        dx: n.dx,
-                        dy: n.dy
-                    }
-                }
+    function xi(n) {
+        n._pack_next = n._pack_prev = n
+    }
 
-                function mo(n, t) {
-                    var e = n.x + t[3],
-                        r = n.y + t[0],
-                        i = n.dx - t[1] - t[3],
-                        u = n.dy - t[0] - t[2];
-                    return i < 0 && (e += i / 2, i = 0), u < 0 && (r += u / 2, u = 0), {
-                        x: e,
-                        y: r,
-                        dx: i,
-                        dy: u
-                    }
-                }
+    function Mi(n) {
+        delete n._pack_next, delete n._pack_prev
+    }
 
-                function Mo(n) {
-                    var t = n[0],
-                        e = n[n.length - 1];
-                    return t < e ? [t, e] : [e, t]
-                }
+    function _i(n, t, e, r) {
+        var u = n.children;
+        if (n.x = t += r * n.x, n.y = e += r * n.y, n.r *= r, u)
+            for (var i = -1, o = u.length; ++i < o;) _i(u[i], t, e, r)
+    }
 
-                function xo(n) {
-                    return n.rangeExtent ? n.rangeExtent() : Mo(n.range())
-                }
+    function bi(n, t, e) {
+        var r = n.r + e.r,
+            u = t.x - n.x,
+            i = t.y - n.y;
+        if (r && (u || i)) {
+            var o = t.r + e.r,
+                a = u * u + i * i;
+            o *= o, r *= r;
+            var c = .5 + (r - o) / (2 * a),
+                l = Math.sqrt(Math.max(0, 2 * o * (r + a) - (r -= a) * r - o * o)) / (2 * a);
+            e.x = n.x + c * u + l * i, e.y = n.y + c * i - l * u
+        } else e.x = n.x + r, e.y = n.y
+    }
 
-                function bo(n, t, e, r) {
-                    var i = e(n[0], n[1]),
-                        u = r(t[0], t[1]);
-                    return function(n) {
-                        return u(i(n))
-                    }
-                }
+    function wi(n, t) {
+        return n.parent == t.parent ? 1 : 2
+    }
 
-                function wo(n, t) {
-                    var e, r = 0,
-                        i = n.length - 1,
-                        u = n[r],
-                        o = n[i];
-                    return o < u && (e = r, r = i, i = e, e = u, u = o, o = e), n[r] = t.floor(u), n[i] = t.ceil(o), n
-                }
+    function Si(n) {
+        var t = n.children;
+        return t.length ? t[0] : n.t
+    }
 
-                function _o(n) {
-                    return n ? {
-                        floor: function(t) {
-                            return Math.floor(t / n) * n
-                        },
-                        ceil: function(t) {
-                            return Math.ceil(t / n) * n
-                        }
-                    } : ko
-                }
-                u.layout.histogram = function() {
-                    var n = !0,
-                        t = Number,
-                        e = eo,
-                        r = no;
-
-                    function i(i, o) {
-                        for (var a, l, c = [], f = i.map(t, this), s = e.call(this, f, o), h = r.call(this, s, f, o), p = (o = -1, f.length), g = h.length - 1, v = n ? 1 : 1 / p; ++o < g;)(a = c[o] = []).dx = h[o + 1] - (a.x = h[o]), a.y = 0;
-                        if (g > 0)
-                            for (o = -1; ++o < p;)(l = f[o]) >= s[0] && l <= s[1] && ((a = c[u.bisect(h, l, 1, g) - 1]).y += v, a.push(i[o]));
-                        return c
-                    }
-                    return i.value = function(n) {
-                        return arguments.length ? (t = n, i) : t
-                    }, i.range = function(n) {
-                        return arguments.length ? (e = Mt(n), i) : e
-                    }, i.bins = function(n) {
-                        return arguments.length ? (r = "number" == typeof n ? function(t) {
-                            return to(t, n)
-                        } : Mt(n), i) : r
-                    }, i.frequency = function(t) {
-                        return arguments.length ? (n = !!t, i) : n
-                    }, i
-                }, u.layout.pack = function() {
-                    var n, t = u.layout.hierarchy().sort(ro),
-                        e = 0,
-                        r = [1, 1];
-
-                    function i(i, u) {
-                        var o = t.call(this, i, u),
-                            a = o[0],
-                            l = r[0],
-                            c = r[1],
-                            f = null == n ? Math.sqrt : "function" == typeof n ? n : function() {
-                                return n
-                            };
-                        if (a.x = a.y = 0, ju(a, (function(n) {
-                                n.r = +f(n.value)
-                            })), ju(a, ao), e) {
-                            var s = e * (n ? 1 : Math.max(2 * a.r / l, 2 * a.r / c)) / 2;
-                            ju(a, (function(n) {
-                                n.r += s
-                            })), ju(a, ao), ju(a, (function(n) {
-                                n.r -= s
-                            }))
-                        }
-                        return function n(t, e, r, i) {
-                            var u = t.children;
-                            if (t.x = e += i * t.x, t.y = r += i * t.y, t.r *= i, u)
-                                for (var o = -1, a = u.length; ++o < a;) n(u[o], e, r, i)
-                        }(a, l / 2, c / 2, n ? 1 : 1 / Math.max(2 * a.r / l, 2 * a.r / c)), o
-                    }
-                    return i.size = function(n) {
-                        return arguments.length ? (r = n, i) : r
-                    }, i.radius = function(t) {
-                        return arguments.length ? (n = null == t || "function" == typeof t ? t : +t, i) : n
-                    }, i.padding = function(n) {
-                        return arguments.length ? (e = +n, i) : e
-                    }, Pu(i, t)
-                }, u.layout.tree = function() {
-                    var n = u.layout.hierarchy().sort(null).value(null),
-                        t = so,
-                        e = [1, 1],
-                        r = null;
-
-                    function i(i, u) {
-                        var c = n.call(this, i, u),
-                            f = c[0],
-                            s = function(n) {
-                                var t, e = {
-                                        A: null,
-                                        children: [n]
-                                    },
-                                    r = [e];
-                                for (; null != (t = r.pop());)
-                                    for (var i, u = t.children, o = 0, a = u.length; o < a; ++o) r.push((u[o] = i = {
-                                        _: u[o],
-                                        parent: t,
-                                        children: (i = u[o].children) && i.slice() || [],
-                                        A: null,
-                                        a: null,
-                                        z: 0,
-                                        m: 0,
-                                        c: 0,
-                                        s: 0,
-                                        t: null,
-                                        i: o
-                                    }).a = i);
-                                return e.children[0]
-                            }(f);
-                        if (ju(s, o), s.parent.m = -s.z, Uu(s, a), r) Uu(f, l);
-                        else {
-                            var h = f,
-                                p = f,
-                                g = f;
-                            Uu(f, (function(n) {
-                                n.x < h.x && (h = n), n.x > p.x && (p = n), n.depth > g.depth && (g = n)
-                            }));
-                            var v = t(h, p) / 2 - h.x,
-                                d = e[0] / (p.x + t(p, h) / 2 + v),
-                                y = e[1] / (g.depth || 1);
-                            Uu(f, (function(n) {
-                                n.x = (n.x + v) * d, n.y = n.depth * y
-                            }))
-                        }
-                        return c
-                    }
+    function ki(n) {
+        var t, e = n.children;
+        return (t = e.length) ? e[t - 1] : n.t
+    }
 
-                    function o(n) {
-                        var e = n.children,
-                            r = n.parent.children,
-                            i = n.i ? r[n.i - 1] : null;
-                        if (e.length) {
-                            ! function(n) {
-                                var t, e = 0,
-                                    r = 0,
-                                    i = n.children,
-                                    u = i.length;
-                                for (; --u >= 0;)(t = i[u]).z += e, t.m += e, e += t.s + (r += t.c)
-                            }(n);
-                            var u = (e[0].z + e[e.length - 1].z) / 2;
-                            i ? (n.z = i.z + t(n._, i._), n.m = n.z - u) : n.z = u
-                        } else i && (n.z = i.z + t(n._, i._));
-                        n.parent.A = function(n, e, r) {
-                            if (e) {
-                                for (var i, u = n, o = n, a = e, l = u.parent.children[0], c = u.m, f = o.m, s = a.m, h = l.m; a = po(a), u = ho(u), a && u;) l = ho(l), (o = po(o)).a = n, (i = a.z + s - u.z - c + t(a._, u._)) > 0 && (go(vo(a, n, r), n, i), c += i, f += i), s += a.m, c += u.m, h += l.m, f += o.m;
-                                a && !po(o) && (o.t = a, o.m += s - f), u && !ho(l) && (l.t = u, l.m += c - h, r = n)
-                            }
-                            return r
-                        }(n, i, n.parent.A || r[0])
-                    }
+    function Ei(n, t, e) {
+        var r = e / (t.i - n.i);
+        t.c -= r, t.s += e, n.c += r, t.z += e, t.m += e
+    }
 
-                    function a(n) {
-                        n._.x = n.z + n.parent.m, n.m += n.parent.m
-                    }
+    function Ai(n) {
+        for (var t, e = 0, r = 0, u = n.children, i = u.length; --i >= 0;) t = u[i], t.z += e, t.m += e, e += t.s + (r += t.c)
+    }
 
-                    function l(n) {
-                        n.x *= e[0], n.y = n.depth * e[1]
-                    }
-                    return i.separation = function(n) {
-                        return arguments.length ? (t = n, i) : t
-                    }, i.size = function(n) {
-                        return arguments.length ? (r = null == (e = n) ? l : null, i) : r ? null : e
-                    }, i.nodeSize = function(n) {
-                        return arguments.length ? (r = null == (e = n) ? null : l, i) : r ? e : null
-                    }, Pu(i, n)
-                }, u.layout.cluster = function() {
-                    var n = u.layout.hierarchy().sort(null).value(null),
-                        t = so,
-                        e = [1, 1],
-                        r = !1;
-
-                    function i(i, o) {
-                        var a, l = n.call(this, i, o),
-                            c = l[0],
-                            f = 0;
-                        ju(c, (function(n) {
-                            var e = n.children;
-                            e && e.length ? (n.x = function(n) {
-                                return n.reduce((function(n, t) {
-                                    return n + t.x
-                                }), 0) / n.length
-                            }(e), n.y = function(n) {
-                                return 1 + u.max(n, (function(n) {
-                                    return n.y
-                                }))
-                            }(e)) : (n.x = a ? f += t(n, a) : 0, n.y = 0, a = n)
-                        }));
-                        var s = function n(t) {
-                                var e = t.children;
-                                return e && e.length ? n(e[0]) : t
-                            }(c),
-                            h = function n(t) {
-                                var e, r = t.children;
-                                return r && (e = r.length) ? n(r[e - 1]) : t
-                            }(c),
-                            p = s.x - t(s, h) / 2,
-                            g = h.x + t(h, s) / 2;
-                        return ju(c, r ? function(n) {
-                            n.x = (n.x - c.x) * e[0], n.y = (c.y - n.y) * e[1]
-                        } : function(n) {
-                            n.x = (n.x - p) / (g - p) * e[0], n.y = (1 - (c.y ? n.y / c.y : 1)) * e[1]
-                        }), l
-                    }
-                    return i.separation = function(n) {
-                        return arguments.length ? (t = n, i) : t
-                    }, i.size = function(n) {
-                        return arguments.length ? (r = null == (e = n), i) : r ? null : e
-                    }, i.nodeSize = function(n) {
-                        return arguments.length ? (r = null != (e = n), i) : r ? e : null
-                    }, Pu(i, n)
-                }, u.layout.treemap = function() {
-                    var n, t = u.layout.hierarchy(),
-                        e = Math.round,
-                        r = [1, 1],
-                        i = null,
-                        o = yo,
-                        a = !1,
-                        l = "squarify",
-                        c = .5 * (1 + Math.sqrt(5));
+    function Ci(n, t, e) {
+        return n.a.parent === t.parent ? n.a : e
+    }
 
-                    function f(n, t) {
-                        for (var e, r, i = -1, u = n.length; ++i < u;) r = (e = n[i]).value * (t < 0 ? 0 : t), e.area = isNaN(r) || r <= 0 ? 0 : r
-                    }
+    function Ni(n) {
+        return 1 + Bo.max(n, function(n) {
+            return n.y
+        })
+    }
 
-                    function s(n) {
-                        var t = n.children;
-                        if (t && t.length) {
-                            var e, r, i, u = o(n),
-                                a = [],
-                                c = t.slice(),
-                                h = 1 / 0,
-                                v = "slice" === l ? u.dx : "dice" === l ? u.dy : "slice-dice" === l ? 1 & n.depth ? u.dy : u.dx : Math.min(u.dx, u.dy);
-                            for (f(c, u.dx * u.dy / n.value), a.area = 0;
-                                (i = c.length) > 0;) a.push(e = c[i - 1]), a.area += e.area, "squarify" !== l || (r = p(a, v)) <= h ? (c.pop(), h = r) : (a.area -= a.pop().area, g(a, v, u, !1), v = Math.min(u.dx, u.dy), a.length = a.area = 0, h = 1 / 0);
-                            a.length && (g(a, v, u, !0), a.length = a.area = 0), t.forEach(s)
-                        }
-                    }
+    function zi(n) {
+        return n.reduce(function(n, t) {
+            return n + t.x
+        }, 0) / n.length
+    }
 
-                    function h(n) {
-                        var t = n.children;
-                        if (t && t.length) {
-                            var e, r = o(n),
-                                i = t.slice(),
-                                u = [];
-                            for (f(i, r.dx * r.dy / n.value), u.area = 0; e = i.pop();) u.push(e), u.area += e.area, null != e.z && (g(u, e.z ? r.dx : r.dy, r, !i.length), u.length = u.area = 0);
-                            t.forEach(h)
-                        }
-                    }
+    function Li(n) {
+        var t = n.children;
+        return t && t.length ? Li(t[0]) : n
+    }
 
-                    function p(n, t) {
-                        for (var e, r = n.area, i = 0, u = 1 / 0, o = -1, a = n.length; ++o < a;)(e = n[o].area) && (e < u && (u = e), e > i && (i = e));
-                        return t *= t, (r *= r) ? Math.max(t * i * c / r, r / (t * u * c)) : 1 / 0
-                    }
+    function Ti(n) {
+        var t, e = n.children;
+        return e && (t = e.length) ? Ti(e[t - 1]) : n
+    }
 
-                    function g(n, t, r, i) {
-                        var u, o = -1,
-                            a = n.length,
-                            l = r.x,
-                            c = r.y,
-                            f = t ? e(n.area / t) : 0;
-                        if (t == r.dx) {
-                            for ((i || f > r.dy) && (f = r.dy); ++o < a;)(u = n[o]).x = l, u.y = c, u.dy = f, l += u.dx = Math.min(r.x + r.dx - l, f ? e(u.area / f) : 0);
-                            u.z = !0, u.dx += r.x + r.dx - l, r.y += f, r.dy -= f
-                        } else {
-                            for ((i || f > r.dx) && (f = r.dx); ++o < a;)(u = n[o]).x = l, u.y = c, u.dx = f, c += u.dy = Math.min(r.y + r.dy - c, f ? e(u.area / f) : 0);
-                            u.z = !1, u.dy += r.y + r.dy - c, r.x += f, r.dx -= f
-                        }
-                    }
+    function qi(n) {
+        return {
+            x: n.x,
+            y: n.y,
+            dx: n.dx,
+            dy: n.dy
+        }
+    }
 
-                    function v(e) {
-                        var i = n || t(e),
-                            u = i[0];
-                        return u.x = u.y = 0, u.value ? (u.dx = r[0], u.dy = r[1]) : u.dx = u.dy = 0, n && t.revalue(u), f([u], u.dx * u.dy / u.value), (n ? h : s)(u), a && (n = i), i
-                    }
-                    return v.size = function(n) {
-                        return arguments.length ? (r = n, v) : r
-                    }, v.padding = function(n) {
-                        if (!arguments.length) return i;
-
-                        function t(t) {
-                            var e = n.call(v, t, t.depth);
-                            return null == e ? yo(t) : mo(t, "number" == typeof e ? [e, e, e, e] : e)
-                        }
+    function Ri(n, t) {
+        var e = n.x + t[3],
+            r = n.y + t[0],
+            u = n.dx - t[1] - t[3],
+            i = n.dy - t[0] - t[2];
+        return 0 > u && (e += u / 2, u = 0), 0 > i && (r += i / 2, i = 0), {
+            x: e,
+            y: r,
+            dx: u,
+            dy: i
+        }
+    }
 
-                        function e(t) {
-                            return mo(t, n)
-                        }
-                        var r;
-                        return o = null == (i = n) ? yo : "function" == (r = typeof n) ? t : "number" === r ? (n = [n, n, n, n], e) : e, v
-                    }, v.round = function(n) {
-                        return arguments.length ? (e = n ? Math.round : Number, v) : e != Number
-                    }, v.sticky = function(t) {
-                        return arguments.length ? (a = t, n = null, v) : a
-                    }, v.ratio = function(n) {
-                        return arguments.length ? (c = n, v) : c
-                    }, v.mode = function(n) {
-                        return arguments.length ? (l = n + "", v) : l
-                    }, Pu(v, t)
-                }, u.random = {
-                    normal: function(n, t) {
-                        var e = arguments.length;
-                        return e < 2 && (t = 1), e < 1 && (n = 0),
-                            function() {
-                                var e, r, i;
-                                do {
-                                    i = (e = 2 * Math.random() - 1) * e + (r = 2 * Math.random() - 1) * r
-                                } while (!i || i > 1);
-                                return n + t * e * Math.sqrt(-2 * Math.log(i) / i)
-                            }
-                    },
-                    logNormal: function() {
-                        var n = u.random.normal.apply(u, arguments);
-                        return function() {
-                            return Math.exp(n())
-                        }
-                    },
-                    bates: function(n) {
-                        var t = u.random.irwinHall(n);
-                        return function() {
-                            return t() / n
-                        }
-                    },
-                    irwinHall: function(n) {
-                        return function() {
-                            for (var t = 0, e = 0; e < n; e++) t += Math.random();
-                            return t
-                        }
-                    }
-                }, u.scale = {};
-                var ko = {
-                    floor: R,
-                    ceil: R
-                };
+    function Di(n) {
+        var t = n[0],
+            e = n[n.length - 1];
+        return e > t ? [t, e] : [e, t]
+    }
 
-                function So(n, t, e, r) {
-                    var i = [],
-                        o = [],
-                        a = 0,
-                        l = Math.min(n.length, t.length) - 1;
-                    for (n[l] < n[0] && (n = n.slice().reverse(), t = t.slice().reverse()); ++a <= l;) i.push(e(n[a - 1], n[a])), o.push(r(t[a - 1], t[a]));
-                    return function(t) {
-                        var e = u.bisect(n, t, 1, l) - 1;
-                        return o[e](i[e](t))
-                    }
-                }
+    function Pi(n) {
+        return n.rangeExtent ? n.rangeExtent() : Di(n.range())
+    }
 
-                function No(n, t) {
-                    return u.rebind(n, t, "range", "rangeRound", "interpolate", "clamp")
-                }
+    function Ui(n, t, e, r) {
+        var u = e(n[0], n[1]),
+            i = r(t[0], t[1]);
+        return function(n) {
+            return i(u(n))
+        }
+    }
 
-                function Eo(n, t) {
-                    return wo(n, _o(Ao(n, t)[2])), wo(n, _o(Ao(n, t)[2])), n
-                }
+    function ji(n, t) {
+        var e, r = 0,
+            u = n.length - 1,
+            i = n[r],
+            o = n[u];
+        return i > o && (e = r, r = u, u = e, e = i, i = o, o = e), n[r] = t.floor(i), n[u] = t.ceil(o), n
+    }
 
-                function Ao(n, t) {
-                    null == t && (t = 10);
-                    var e = Mo(n),
-                        r = e[1] - e[0],
-                        i = Math.pow(10, Math.floor(Math.log(r / t) / Math.LN10)),
-                        u = t / r * i;
-                    return u <= .15 ? i *= 10 : u <= .35 ? i *= 5 : u <= .75 && (i *= 2), e[0] = Math.ceil(e[0] / i) * i, e[1] = Math.floor(e[1] / i) * i + .5 * i, e[2] = i, e
-                }
+    function Fi(n) {
+        return n ? {
+            floor: function(t) {
+                return Math.floor(t / n) * n
+            },
+            ceil: function(t) {
+                return Math.ceil(t / n) * n
+            }
+        } : gl
+    }
 
-                function Co(n, t) {
-                    return u.range.apply(u, Ao(n, t))
-                }
+    function Hi(n, t, e, r) {
+        var u = [],
+            i = [],
+            o = 0,
+            a = Math.min(n.length, t.length) - 1;
+        for (n[a] < n[0] && (n = n.slice().reverse(), t = t.slice().reverse()); ++o <= a;) u.push(e(n[o - 1], n[o])), i.push(r(t[o - 1], t[o]));
+        return function(t) {
+            var e = Bo.bisect(n, t, 1, a) - 1;
+            return i[e](u[e](t))
+        }
+    }
 
-                function zo(n, t, e) {
-                    var r = Ao(n, t);
-                    if (e) {
-                        var i = Rt.exec(e);
-                        if (i.shift(), "s" === i[8]) {
-                            var o = u.formatPrefix(Math.max(w(r[0]), w(r[1])));
-                            return i[7] || (i[7] = "." + qo(o.scale(r[2]))), i[8] = "f", e = u.format(i.join("")),
-                                function(n) {
-                                    return e(o.scale(n)) + o.symbol
-                                }
-                        }
-                        i[7] || (i[7] = "." + function(n, t) {
-                            var e = qo(t[2]);
-                            return n in Lo ? Math.abs(e - qo(Math.max(w(t[0]), w(t[1])))) + +("e" !== n) : e - 2 * ("%" === n)
-                        }(i[8], r)), e = i.join("")
-                    } else e = ",." + qo(r[2]) + "f";
-                    return u.format(e)
-                }
-                u.scale.linear = function() {
-                    return function n(t, e, r, i) {
-                        var u, o;
-
-                        function a() {
-                            var n = Math.min(t.length, e.length) > 2 ? So : bo,
-                                a = i ? Nu : Su;
-                            return u = n(t, e, a, r), o = n(e, t, a, ru), l
-                        }
+    function Oi(n, t, e, r) {
+        function u() {
+            var u = Math.min(n.length, t.length) > 2 ? Hi : Ui,
+                c = r ? Ou : Hu;
+            return o = u(n, t, c, e), a = u(t, n, c, du), i
+        }
 
-                        function l(n) {
-                            return u(n)
-                        }
-                        return l.invert = function(n) {
-                            return o(n)
-                        }, l.domain = function(n) {
-                            return arguments.length ? (t = n.map(Number), a()) : t
-                        }, l.range = function(n) {
-                            return arguments.length ? (e = n, a()) : e
-                        }, l.rangeRound = function(n) {
-                            return l.range(n).interpolate(mu)
-                        }, l.clamp = function(n) {
-                            return arguments.length ? (i = n, a()) : i
-                        }, l.interpolate = function(n) {
-                            return arguments.length ? (r = n, a()) : r
-                        }, l.ticks = function(n) {
-                            return Co(t, n)
-                        }, l.tickFormat = function(n, e) {
-                            return zo(t, n, e)
-                        }, l.nice = function(n) {
-                            return Eo(t, n), a()
-                        }, l.copy = function() {
-                            return n(t, e, r, i)
-                        }, a()
-                    }([0, 1], [0, 1], ru, !1)
-                };
-                var Lo = {
-                    s: 1,
-                    g: 1,
-                    p: 1,
-                    r: 1,
-                    e: 1
-                };
+        function i(n) {
+            return o(n)
+        }
+        var o, a;
+        return i.invert = function(n) {
+            return a(n)
+        }, i.domain = function(t) {
+            return arguments.length ? (n = t.map(Number), u()) : n
+        }, i.range = function(n) {
+            return arguments.length ? (t = n, u()) : t
+        }, i.rangeRound = function(n) {
+            return i.range(n).interpolate(Ru)
+        }, i.clamp = function(n) {
+            return arguments.length ? (r = n, u()) : r
+        }, i.interpolate = function(n) {
+            return arguments.length ? (e = n, u()) : e
+        }, i.ticks = function(t) {
+            return Vi(n, t)
+        }, i.tickFormat = function(t, e) {
+            return Xi(n, t, e)
+        }, i.nice = function(t) {
+            return Ii(n, t), u()
+        }, i.copy = function() {
+            return Oi(n, t, e, r)
+        }, u()
+    }
 
-                function qo(n) {
-                    return -Math.floor(Math.log(n) / Math.LN10 + .01)
-                }
-                u.scale.log = function() {
-                    return function n(t, e, r, i) {
-                        function o(n) {
-                            return (r ? Math.log(n < 0 ? 0 : n) : -Math.log(n > 0 ? 0 : -n)) / Math.log(e)
-                        }
+    function Yi(n, t) {
+        return Bo.rebind(n, t, "range", "rangeRound", "interpolate", "clamp")
+    }
 
-                        function a(n) {
-                            return r ? Math.pow(e, n) : -Math.pow(e, -n)
-                        }
+    function Ii(n, t) {
+        return ji(n, Fi(Zi(n, t)[2]))
+    }
 
-                        function l(n) {
-                            return t(o(n))
-                        }
-                        return l.invert = function(n) {
-                            return a(t.invert(n))
-                        }, l.domain = function(n) {
-                            return arguments.length ? (r = n[0] >= 0, t.domain((i = n.map(Number)).map(o)), l) : i
-                        }, l.base = function(n) {
-                            return arguments.length ? (e = +n, t.domain(i.map(o)), l) : e
-                        }, l.nice = function() {
-                            var n = wo(i.map(o), r ? Math : Ro);
-                            return t.domain(n), i = n.map(a), l
-                        }, l.ticks = function() {
-                            var n = Mo(i),
-                                t = [],
-                                u = n[0],
-                                l = n[1],
-                                c = Math.floor(o(u)),
-                                f = Math.ceil(o(l)),
-                                s = e % 1 ? 2 : e;
-                            if (isFinite(f - c)) {
-                                if (r) {
-                                    for (; c < f; c++)
-                                        for (var h = 1; h < s; h++) t.push(a(c) * h);
-                                    t.push(a(c))
-                                } else
-                                    for (t.push(a(c)); c++ < f;)
-                                        for (h = s - 1; h > 0; h--) t.push(a(c) * h);
-                                for (c = 0; t[c] < u; c++);
-                                for (f = t.length; t[f - 1] > l; f--);
-                                t = t.slice(c, f)
-                            }
-                            return t
-                        }, l.tickFormat = function(n, t) {
-                            if (!arguments.length) return To;
-                            arguments.length < 2 ? t = To : "function" != typeof t && (t = u.format(t));
-                            var r = Math.max(1, e * n / l.ticks().length);
-                            return function(n) {
-                                var i = n / a(Math.round(o(n)));
-                                return i * e < e - .5 && (i *= e), i <= r ? t(n) : ""
-                            }
-                        }, l.copy = function() {
-                            return n(t.copy(), e, r, i)
-                        }, No(l, t)
-                    }(u.scale.linear().domain([0, 1]), 10, !0, [1, 10])
-                };
-                var To = u.format(".0e"),
-                    Ro = {
-                        floor: function(n) {
-                            return -Math.ceil(-n)
-                        },
-                        ceil: function(n) {
-                            return -Math.floor(-n)
-                        }
-                    };
+    function Zi(n, t) {
+        null == t && (t = 10);
+        var e = Di(n),
+            r = e[1] - e[0],
+            u = Math.pow(10, Math.floor(Math.log(r / t) / Math.LN10)),
+            i = t / r * u;
+        return .15 >= i ? u *= 10 : .35 >= i ? u *= 5 : .75 >= i && (u *= 2), e[0] = Math.ceil(e[0] / u) * u, e[1] = Math.floor(e[1] / u) * u + .5 * u, e[2] = u, e
+    }
 
-                function Do(n) {
-                    return function(t) {
-                        return t < 0 ? -Math.pow(-t, n) : Math.pow(t, n)
-                    }
-                }
-                u.scale.pow = function() {
-                    return function n(t, e, r) {
-                        var i = Do(e),
-                            u = Do(1 / e);
+    function Vi(n, t) {
+        return Bo.range.apply(Bo, Zi(n, t))
+    }
 
-                        function o(n) {
-                            return t(i(n))
-                        }
-                        return o.invert = function(n) {
-                            return u(t.invert(n))
-                        }, o.domain = function(n) {
-                            return arguments.length ? (t.domain((r = n.map(Number)).map(i)), o) : r
-                        }, o.ticks = function(n) {
-                            return Co(r, n)
-                        }, o.tickFormat = function(n, t) {
-                            return zo(r, n, t)
-                        }, o.nice = function(n) {
-                            return o.domain(Eo(r, n))
-                        }, o.exponent = function(n) {
-                            return arguments.length ? (i = Do(e = n), u = Do(1 / e), t.domain(r.map(i)), o) : e
-                        }, o.copy = function() {
-                            return n(t.copy(), e, r)
-                        }, No(o, t)
-                    }(u.scale.linear(), 1, [0, 1])
-                }, u.scale.sqrt = function() {
-                    return u.scale.pow().exponent(.5)
-                }, u.scale.ordinal = function() {
-                    return function n(t, e) {
-                        var r, i, o;
+    function Xi(n, t, e) {
+        var r = Zi(n, t);
+        if (e) {
+            var u = tc.exec(e);
+            if (u.shift(), "s" === u[8]) {
+                var i = Bo.formatPrefix(Math.max(ca(r[0]), ca(r[1])));
+                return u[7] || (u[7] = "." + $i(i.scale(r[2]))), u[8] = "f", e = Bo.format(u.join("")),
+                    function(n) {
+                        return e(i.scale(n)) + i.symbol
+                    }
+            }
+            u[7] || (u[7] = "." + Bi(u[8], r)), e = u.join("")
+        } else e = ",." + $i(r[2]) + "f";
+        return Bo.format(e)
+    }
 
-                        function a(n) {
-                            return i[((r.get(n) || ("range" === e.t ? r.set(n, t.push(n)) : NaN)) - 1) % i.length]
-                        }
+    function $i(n) {
+        return -Math.floor(Math.log(n) / Math.LN10 + .01)
+    }
 
-                        function l(n, e) {
-                            return u.range(t.length).map((function(t) {
-                                return n + e * t
-                            }))
-                        }
-                        return a.domain = function(n) {
-                            if (!arguments.length) return t;
-                            t = [], r = new S;
-                            for (var i, u = -1, o = n.length; ++u < o;) r.has(i = n[u]) || r.set(i, t.push(i));
-                            return a[e.t].apply(a, e.a)
-                        }, a.range = function(n) {
-                            return arguments.length ? (i = n, o = 0, e = {
-                                t: "range",
-                                a: arguments
-                            }, a) : i
-                        }, a.rangePoints = function(n, r) {
-                            arguments.length < 2 && (r = 0);
-                            var u = n[0],
-                                c = n[1],
-                                f = t.length < 2 ? (u = (u + c) / 2, 0) : (c - u) / (t.length - 1 + r);
-                            return i = l(u + f * r / 2, f), o = 0, e = {
-                                t: "rangePoints",
-                                a: arguments
-                            }, a
-                        }, a.rangeRoundPoints = function(n, r) {
-                            arguments.length < 2 && (r = 0);
-                            var u = n[0],
-                                c = n[1],
-                                f = t.length < 2 ? (u = c = Math.round((u + c) / 2), 0) : (c - u) / (t.length - 1 + r) | 0;
-                            return i = l(u + Math.round(f * r / 2 + (c - u - (t.length - 1 + r) * f) / 2), f), o = 0, e = {
-                                t: "rangeRoundPoints",
-                                a: arguments
-                            }, a
-                        }, a.rangeBands = function(n, r, u) {
-                            arguments.length < 2 && (r = 0), arguments.length < 3 && (u = r);
-                            var c = n[1] < n[0],
-                                f = n[c - 0],
-                                s = n[1 - c],
-                                h = (s - f) / (t.length - r + 2 * u);
-                            return i = l(f + h * u, h), c && i.reverse(), o = h * (1 - r), e = {
-                                t: "rangeBands",
-                                a: arguments
-                            }, a
-                        }, a.rangeRoundBands = function(n, r, u) {
-                            arguments.length < 2 && (r = 0), arguments.length < 3 && (u = r);
-                            var c = n[1] < n[0],
-                                f = n[c - 0],
-                                s = n[1 - c],
-                                h = Math.floor((s - f) / (t.length - r + 2 * u));
-                            return i = l(f + Math.round((s - f - (t.length - r) * h) / 2), h), c && i.reverse(), o = Math.round(h * (1 - r)), e = {
-                                t: "rangeRoundBands",
-                                a: arguments
-                            }, a
-                        }, a.rangeBand = function() {
-                            return o
-                        }, a.rangeExtent = function() {
-                            return Mo(e.a[0])
-                        }, a.copy = function() {
-                            return n(t, e)
-                        }, a.domain(t)
-                    }([], {
-                        t: "range",
-                        a: [
-                            []
-                        ]
-                    })
-                }, u.scale.category10 = function() {
-                    return u.scale.ordinal().range(Po)
-                }, u.scale.category20 = function() {
-                    return u.scale.ordinal().range(Uo)
-                }, u.scale.category20b = function() {
-                    return u.scale.ordinal().range(jo)
-                }, u.scale.category20c = function() {
-                    return u.scale.ordinal().range(Fo)
-                };
-                var Po = [2062260, 16744206, 2924588, 14034728, 9725885, 9197131, 14907330, 8355711, 12369186, 1556175].map(ft),
-                    Uo = [2062260, 11454440, 16744206, 16759672, 2924588, 10018698, 14034728, 16750742, 9725885, 12955861, 9197131, 12885140, 14907330, 16234194, 8355711, 13092807, 12369186, 14408589, 1556175, 10410725].map(ft),
-                    jo = [3750777, 5395619, 7040719, 10264286, 6519097, 9216594, 11915115, 13556636, 9202993, 12426809, 15186514, 15190932, 8666169, 11356490, 14049643, 15177372, 8077683, 10834324, 13528509, 14589654].map(ft),
-                    Fo = [3244733, 7057110, 10406625, 13032431, 15095053, 16616764, 16625259, 16634018, 3253076, 7652470, 10607003, 13101504, 7695281, 10394312, 12369372, 14342891, 6513507, 9868950, 12434877, 14277081].map(ft);
-
-                function Ho() {
-                    return 0
-                }
-                u.scale.quantile = function() {
-                    return function n(t, e) {
-                        var r;
-
-                        function i() {
-                            var n = 0,
-                                i = e.length;
-                            for (r = []; ++n < i;) r[n - 1] = u.quantile(t, n / i);
-                            return o
-                        }
+    function Bi(n, t) {
+        var e = $i(t[2]);
+        return n in pl ? Math.abs(e - $i(Math.max(ca(t[0]), ca(t[1])))) + +("e" !== n) : e - 2 * ("%" === n)
+    }
 
-                        function o(n) {
-                            if (!isNaN(n = +n)) return e[u.bisect(r, n)]
-                        }
-                        return o.domain = function(n) {
-                            return arguments.length ? (t = n.map(y).filter(m).sort(d), i()) : t
-                        }, o.range = function(n) {
-                            return arguments.length ? (e = n, i()) : e
-                        }, o.quantiles = function() {
-                            return r
-                        }, o.invertExtent = function(n) {
-                            return (n = e.indexOf(n)) < 0 ? [NaN, NaN] : [n > 0 ? r[n - 1] : t[0], n < r.length ? r[n] : t[t.length - 1]]
-                        }, o.copy = function() {
-                            return n(t, e)
-                        }, i()
-                    }([], [])
-                }, u.scale.quantize = function() {
-                    return function n(t, e, r) {
-                        var i, u;
+    function Wi(n, t, e, r) {
+        function u(n) {
+            return (e ? Math.log(0 > n ? 0 : n) : -Math.log(n > 0 ? 0 : -n)) / Math.log(t)
+        }
 
-                        function o(n) {
-                            return r[Math.max(0, Math.min(u, Math.floor(i * (n - t))))]
-                        }
+        function i(n) {
+            return e ? Math.pow(t, n) : -Math.pow(t, -n)
+        }
 
-                        function a() {
-                            return i = r.length / (e - t), u = r.length - 1, o
-                        }
-                        return o.domain = function(n) {
-                            return arguments.length ? (t = +n[0], e = +n[n.length - 1], a()) : [t, e]
-                        }, o.range = function(n) {
-                            return arguments.length ? (r = n, a()) : r
-                        }, o.invertExtent = function(n) {
-                            return [n = (n = r.indexOf(n)) < 0 ? NaN : n / i + t, n + 1 / i]
-                        }, o.copy = function() {
-                            return n(t, e, r)
-                        }, a()
-                    }(0, 1, [0, 1])
-                }, u.scale.threshold = function() {
-                    return function n(t, e) {
-                        function r(n) {
-                            if (n <= n) return e[u.bisect(t, n)]
-                        }
-                        return r.domain = function(n) {
-                            return arguments.length ? (t = n, r) : t
-                        }, r.range = function(n) {
-                            return arguments.length ? (e = n, r) : e
-                        }, r.invertExtent = function(n) {
-                            return n = e.indexOf(n), [t[n - 1], t[n]]
-                        }, r.copy = function() {
-                            return n(t, e)
-                        }, r
-                    }([.5], [0, 1])
-                }, u.scale.identity = function() {
-                    return function n(t) {
-                        function e(n) {
-                            return +n
-                        }
-                        return e.invert = e, e.domain = e.range = function(n) {
-                            return arguments.length ? (t = n.map(e), e) : t
-                        }, e.ticks = function(n) {
-                            return Co(t, n)
-                        }, e.tickFormat = function(n, e) {
-                            return zo(t, n, e)
-                        }, e.copy = function() {
-                            return n(t)
-                        }, e
-                    }([0, 1])
-                }, u.svg = {}, u.svg.arc = function() {
-                    var n = Io,
-                        t = Yo,
-                        e = Ho,
-                        r = Oo,
-                        i = Zo,
-                        u = Vo,
-                        o = Xo;
-
-                    function a() {
-                        var a = Math.max(0, +n.apply(this, arguments)),
-                            c = Math.max(0, +t.apply(this, arguments)),
-                            f = i.apply(this, arguments) - Rn,
-                            s = u.apply(this, arguments) - Rn,
-                            h = Math.abs(s - f),
-                            p = f > s ? 0 : 1;
-                        if (c < a && (g = c, c = a, a = g), h >= Tn) return l(c, p) + (a ? l(a, 1 - p) : "") + "Z";
-                        var g, v, d, y, m, M, x, b, w, _, k, S, N = 0,
-                            E = 0,
-                            A = [];
-                        if ((y = (+o.apply(this, arguments) || 0) / 2) && (d = r === Oo ? Math.sqrt(a * a + c * c) : +r.apply(this, arguments), p || (E *= -1), c && (E = Hn(d / c * Math.sin(y))), a && (N = Hn(d / a * Math.sin(y)))), c) {
-                            m = c * Math.cos(f + E), M = c * Math.sin(f + E), x = c * Math.cos(s - E), b = c * Math.sin(s - E);
-                            var C = Math.abs(s - f - 2 * E) <= Ln ? 0 : 1;
-                            if (E && $o(m, M, x, b) === p ^ C) {
-                                var z = (f + s) / 2;
-                                m = c * Math.cos(z), M = c * Math.sin(z), x = b = null
-                            }
-                        } else m = M = 0;
-                        if (a) {
-                            w = a * Math.cos(s - N), _ = a * Math.sin(s - N), k = a * Math.cos(f + N), S = a * Math.sin(f + N);
-                            var L = Math.abs(f - s + 2 * N) <= Ln ? 0 : 1;
-                            if (N && $o(w, _, k, S) === 1 - p ^ L) {
-                                var q = (f + s) / 2;
-                                w = a * Math.cos(q), _ = a * Math.sin(q), k = S = null
-                            }
-                        } else w = _ = 0;
-                        if (h > Cn && (g = Math.min(Math.abs(c - a) / 2, +e.apply(this, arguments))) > .001) {
-                            v = a < c ^ p ? 0 : 1;
-                            var T = g,
-                                R = g;
-                            if (h < Ln) {
-                                var D = null == k ? [w, _] : null == x ? [m, M] : hi([m, M], [k, S], [x, b], [w, _]),
-                                    P = m - D[0],
-                                    U = M - D[1],
-                                    j = x - D[0],
-                                    F = b - D[1],
-                                    H = 1 / Math.sin(Math.acos((P * j + U * F) / (Math.sqrt(P * P + U * U) * Math.sqrt(j * j + F * F))) / 2),
-                                    O = Math.sqrt(D[0] * D[0] + D[1] * D[1]);
-                                R = Math.min(g, (a - O) / (H - 1)), T = Math.min(g, (c - O) / (H + 1))
-                            }
-                            if (null != x) {
-                                var I = Bo(null == k ? [w, _] : [k, S], [m, M], c, T, p),
-                                    Y = Bo([x, b], [w, _], c, T, p);
-                                g === T ? A.push("M", I[0], "A", T, ",", T, " 0 0,", v, " ", I[1], "A", c, ",", c, " 0 ", 1 - p ^ $o(I[1][0], I[1][1], Y[1][0], Y[1][1]), ",", p, " ", Y[1], "A", T, ",", T, " 0 0,", v, " ", Y[0]) : A.push("M", I[0], "A", T, ",", T, " 0 1,", v, " ", Y[0])
-                            } else A.push("M", m, ",", M);
-                            if (null != k) {
-                                var Z = Bo([m, M], [k, S], a, -R, p),
-                                    V = Bo([w, _], null == x ? [m, M] : [x, b], a, -R, p);
-                                g === R ? A.push("L", V[0], "A", R, ",", R, " 0 0,", v, " ", V[1], "A", a, ",", a, " 0 ", p ^ $o(V[1][0], V[1][1], Z[1][0], Z[1][1]), ",", 1 - p, " ", Z[1], "A", R, ",", R, " 0 0,", v, " ", Z[0]) : A.push("L", V[0], "A", R, ",", R, " 0 0,", v, " ", Z[0])
-                            } else A.push("L", w, ",", _)
-                        } else A.push("M", m, ",", M), null != x && A.push("A", c, ",", c, " 0 ", C, ",", p, " ", x, ",", b), A.push("L", w, ",", _), null != k && A.push("A", a, ",", a, " 0 ", L, ",", 1 - p, " ", k, ",", S);
-                        return A.push("Z"), A.join("")
-                    }
+        function o(t) {
+            return n(u(t))
+        }
+        return o.invert = function(t) {
+            return i(n.invert(t))
+        }, o.domain = function(t) {
+            return arguments.length ? (e = t[0] >= 0, n.domain((r = t.map(Number)).map(u)), o) : r
+        }, o.base = function(e) {
+            return arguments.length ? (t = +e, n.domain(r.map(u)), o) : t
+        }, o.nice = function() {
+            var t = ji(r.map(u), e ? Math : dl);
+            return n.domain(t), r = t.map(i), o
+        }, o.ticks = function() {
+            var n = Di(r),
+                o = [],
+                a = n[0],
+                c = n[1],
+                l = Math.floor(u(a)),
+                s = Math.ceil(u(c)),
+                f = t % 1 ? 2 : t;
+            if (isFinite(s - l)) {
+                if (e) {
+                    for (; s > l; l++)
+                        for (var h = 1; f > h; h++) o.push(i(l) * h);
+                    o.push(i(l))
+                } else
+                    for (o.push(i(l)); l++ < s;)
+                        for (var h = f - 1; h > 0; h--) o.push(i(l) * h);
+                for (l = 0; o[l] < a; l++);
+                for (s = o.length; o[s - 1] > c; s--);
+                o = o.slice(l, s)
+            }
+            return o
+        }, o.tickFormat = function(n, t) {
+            if (!arguments.length) return vl;
+            arguments.length < 2 ? t = vl : "function" != typeof t && (t = Bo.format(t));
+            var r, a = Math.max(.1, n / o.ticks().length),
+                c = e ? (r = 1e-12, Math.ceil) : (r = -1e-12, Math.floor);
+            return function(n) {
+                return n / i(c(u(n) + r)) <= a ? t(n) : ""
+            }
+        }, o.copy = function() {
+            return Wi(n.copy(), t, e, r)
+        }, Yi(o, n)
+    }
 
-                    function l(n, t) {
-                        return "M0," + n + "A" + n + "," + n + " 0 1," + t + " 0," + -n + "A" + n + "," + n + " 0 1," + t + " 0," + n
-                    }
-                    return a.innerRadius = function(t) {
-                        return arguments.length ? (n = Mt(t), a) : n
-                    }, a.outerRadius = function(n) {
-                        return arguments.length ? (t = Mt(n), a) : t
-                    }, a.cornerRadius = function(n) {
-                        return arguments.length ? (e = Mt(n), a) : e
-                    }, a.padRadius = function(n) {
-                        return arguments.length ? (r = n == Oo ? Oo : Mt(n), a) : r
-                    }, a.startAngle = function(n) {
-                        return arguments.length ? (i = Mt(n), a) : i
-                    }, a.endAngle = function(n) {
-                        return arguments.length ? (u = Mt(n), a) : u
-                    }, a.padAngle = function(n) {
-                        return arguments.length ? (o = Mt(n), a) : o
-                    }, a.centroid = function() {
-                        var e = (+n.apply(this, arguments) + +t.apply(this, arguments)) / 2,
-                            r = (+i.apply(this, arguments) + +u.apply(this, arguments)) / 2 - Rn;
-                        return [Math.cos(r) * e, Math.sin(r) * e]
-                    }, a
-                };
-                var Oo = "auto";
+    function Ji(n, t, e) {
+        function r(t) {
+            return n(u(t))
+        }
+        var u = Gi(t),
+            i = Gi(1 / t);
+        return r.invert = function(t) {
+            return i(n.invert(t))
+        }, r.domain = function(t) {
+            return arguments.length ? (n.domain((e = t.map(Number)).map(u)), r) : e
+        }, r.ticks = function(n) {
+            return Vi(e, n)
+        }, r.tickFormat = function(n, t) {
+            return Xi(e, n, t)
+        }, r.nice = function(n) {
+            return r.domain(Ii(e, n))
+        }, r.exponent = function(o) {
+            return arguments.length ? (u = Gi(t = o), i = Gi(1 / t), n.domain(e.map(u)), r) : t
+        }, r.copy = function() {
+            return Ji(n.copy(), t, e)
+        }, Yi(r, n)
+    }
 
-                function Io(n) {
-                    return n.innerRadius
-                }
+    function Gi(n) {
+        return function(t) {
+            return 0 > t ? -Math.pow(-t, n) : Math.pow(t, n)
+        }
+    }
 
-                function Yo(n) {
-                    return n.outerRadius
-                }
+    function Ki(n, t) {
+        function e(e) {
+            return i[((u.get(e) || ("range" === t.t ? u.set(e, n.push(e)) : 0 / 0)) - 1) % i.length]
+        }
 
-                function Zo(n) {
-                    return n.startAngle
-                }
-
-                function Vo(n) {
-                    return n.endAngle
-                }
-
-                function Xo(n) {
-                    return n && n.padAngle
-                }
-
-                function $o(n, t, e, r) {
-                    return (n - e) * t - (t - r) * n > 0 ? 0 : 1
-                }
-
-                function Bo(n, t, e, r, i) {
-                    var u = n[0] - t[0],
-                        o = n[1] - t[1],
-                        a = (i ? r : -r) / Math.sqrt(u * u + o * o),
-                        l = a * o,
-                        c = -a * u,
-                        f = n[0] + l,
-                        s = n[1] + c,
-                        h = t[0] + l,
-                        p = t[1] + c,
-                        g = (f + h) / 2,
-                        v = (s + p) / 2,
-                        d = h - f,
-                        y = p - s,
-                        m = d * d + y * y,
-                        M = e - r,
-                        x = f * p - h * s,
-                        b = (y < 0 ? -1 : 1) * Math.sqrt(Math.max(0, M * M * m - x * x)),
-                        w = (x * y - d * b) / m,
-                        _ = (-x * d - y * b) / m,
-                        k = (x * y + d * b) / m,
-                        S = (-x * d + y * b) / m,
-                        N = w - g,
-                        E = _ - v,
-                        A = k - g,
-                        C = S - v;
-                    return N * N + E * E > A * A + C * C && (w = k, _ = S), [
-                        [w - l, _ - c],
-                        [w * e / M, _ * e / M]
-                    ]
-                }
-
-                function Jo(n) {
-                    var t = oi,
-                        e = ai,
-                        r = Ge,
-                        i = Go,
-                        u = i.key,
-                        o = .7;
-
-                    function a(u) {
-                        var a, l = [],
-                            c = [],
-                            f = -1,
-                            s = u.length,
-                            h = Mt(t),
-                            p = Mt(e);
+        function r(t, e) {
+            return Bo.range(n.length).map(function(n) {
+                return t + e * n
+            })
+        }
+        var u, i, o;
+        return e.domain = function(r) {
+            if (!arguments.length) return n;
+            n = [], u = new a;
+            for (var i, o = -1, c = r.length; ++o < c;) u.has(i = r[o]) || u.set(i, n.push(i));
+            return e[t.t].apply(e, t.a)
+        }, e.range = function(n) {
+            return arguments.length ? (i = n, o = 0, t = {
+                t: "range",
+                a: arguments
+            }, e) : i
+        }, e.rangePoints = function(u, a) {
+            arguments.length < 2 && (a = 0);
+            var c = u[0],
+                l = u[1],
+                s = (l - c) / (Math.max(1, n.length - 1) + a);
+            return i = r(n.length < 2 ? (c + l) / 2 : c + s * a / 2, s), o = 0, t = {
+                t: "rangePoints",
+                a: arguments
+            }, e
+        }, e.rangeBands = function(u, a, c) {
+            arguments.length < 2 && (a = 0), arguments.length < 3 && (c = a);
+            var l = u[1] < u[0],
+                s = u[l - 0],
+                f = u[1 - l],
+                h = (f - s) / (n.length - a + 2 * c);
+            return i = r(s + h * c, h), l && i.reverse(), o = h * (1 - a), t = {
+                t: "rangeBands",
+                a: arguments
+            }, e
+        }, e.rangeRoundBands = function(u, a, c) {
+            arguments.length < 2 && (a = 0), arguments.length < 3 && (c = a);
+            var l = u[1] < u[0],
+                s = u[l - 0],
+                f = u[1 - l],
+                h = Math.floor((f - s) / (n.length - a + 2 * c)),
+                g = f - s - (n.length - a) * h;
+            return i = r(s + Math.round(g / 2), h), l && i.reverse(), o = Math.round(h * (1 - a)), t = {
+                t: "rangeRoundBands",
+                a: arguments
+            }, e
+        }, e.rangeBand = function() {
+            return o
+        }, e.rangeExtent = function() {
+            return Di(t.a[0])
+        }, e.copy = function() {
+            return Ki(n, t)
+        }, e.domain(n)
+    }
 
-                        function g() {
-                            l.push("M", i(n(c), o))
-                        }
-                        for (; ++f < s;) r.call(this, a = u[f], f) ? c.push([+h.call(this, a, f), +p.call(this, a, f)]) : c.length && (g(), c = []);
-                        return c.length && g(), l.length ? l.join("") : null
-                    }
-                    return a.x = function(n) {
-                        return arguments.length ? (t = n, a) : t
-                    }, a.y = function(n) {
-                        return arguments.length ? (e = n, a) : e
-                    }, a.defined = function(n) {
-                        return arguments.length ? (r = n, a) : r
-                    }, a.interpolate = function(n) {
-                        return arguments.length ? (u = "function" == typeof n ? i = n : (i = Wo.get(n) || Go).key, a) : u
-                    }, a.tension = function(n) {
-                        return arguments.length ? (o = n, a) : o
-                    }, a
-                }
-                u.svg.line = function() {
-                    return Jo(R)
-                };
-                var Wo = u.map({
-                    linear: Go,
-                    "linear-closed": Ko,
-                    step: function(n) {
-                        var t = 0,
-                            e = n.length,
-                            r = n[0],
-                            i = [r[0], ",", r[1]];
-                        for (; ++t < e;) i.push("H", (r[0] + (r = n[t])[0]) / 2, "V", r[1]);
-                        e > 1 && i.push("H", r[0]);
-                        return i.join("")
-                    },
-                    "step-before": Qo,
-                    "step-after": na,
-                    basis: ra,
-                    "basis-open": function(n) {
-                        if (n.length < 4) return Go(n);
-                        var t, e = [],
-                            r = -1,
-                            i = n.length,
-                            u = [0],
-                            o = [0];
-                        for (; ++r < 3;) t = n[r], u.push(t[0]), o.push(t[1]);
-                        e.push(ia(aa, u) + "," + ia(aa, o)), --r;
-                        for (; ++r < i;) t = n[r], u.shift(), u.push(t[0]), o.shift(), o.push(t[1]), la(e, u, o);
-                        return e.join("")
-                    },
-                    "basis-closed": function(n) {
-                        var t, e, r = -1,
-                            i = n.length,
-                            u = i + 4,
-                            o = [],
-                            a = [];
-                        for (; ++r < 4;) e = n[r % i], o.push(e[0]), a.push(e[1]);
-                        t = [ia(aa, o), ",", ia(aa, a)], --r;
-                        for (; ++r < u;) e = n[r % i], o.shift(), o.push(e[0]), a.shift(), a.push(e[1]), la(t, o, a);
-                        return t.join("")
-                    },
-                    bundle: function(n, t) {
-                        var e = n.length - 1;
-                        if (e)
-                            for (var r, i, u = n[0][0], o = n[0][1], a = n[e][0] - u, l = n[e][1] - o, c = -1; ++c <= e;) r = n[c], i = c / e, r[0] = t * r[0] + (1 - t) * (u + i * a), r[1] = t * r[1] + (1 - t) * (o + i * l);
-                        return ra(n)
-                    },
-                    cardinal: function(n, t) {
-                        return n.length < 3 ? Go(n) : n[0] + ta(n, ea(n, t))
-                    },
-                    "cardinal-open": function(n, t) {
-                        return n.length < 4 ? Go(n) : n[1] + ta(n.slice(1, -1), ea(n, t))
-                    },
-                    "cardinal-closed": function(n, t) {
-                        return n.length < 3 ? Ko(n) : n[0] + ta((n.push(n[0]), n), ea([n[n.length - 2]].concat(n, [n[1]]), t))
-                    },
-                    monotone: function(n) {
-                        return n.length < 3 ? Go(n) : n[0] + ta(n, function(n) {
-                            var t, e, r, i, u = [],
-                                o = function(n) {
-                                    var t = 0,
-                                        e = n.length - 1,
-                                        r = [],
-                                        i = n[0],
-                                        u = n[1],
-                                        o = r[0] = ca(i, u);
-                                    for (; ++t < e;) r[t] = (o + (o = ca(i = u, u = n[t + 1]))) / 2;
-                                    return r[t] = o, r
-                                }(n),
-                                a = -1,
-                                l = n.length - 1;
-                            for (; ++a < l;) t = ca(n[a], n[a + 1]), w(t) < Cn ? o[a] = o[a + 1] = 0 : (e = o[a] / t, r = o[a + 1] / t, (i = e * e + r * r) > 9 && (i = 3 * t / Math.sqrt(i), o[a] = i * e, o[a + 1] = i * r));
-                            a = -1;
-                            for (; ++a <= l;) i = (n[Math.min(l, a + 1)][0] - n[Math.max(0, a - 1)][0]) / (6 * (1 + o[a] * o[a])), u.push([i || 0, o[a] * i || 0]);
-                            return u
-                        }(n))
-                    }
-                });
+    function Qi(r, u) {
+        function i() {
+            var n = 0,
+                t = u.length;
+            for (a = []; ++n < t;) a[n - 1] = Bo.quantile(r, n / t);
+            return o
+        }
 
-                function Go(n) {
-                    return n.length > 1 ? n.join("L") : n + "Z"
-                }
+        function o(n) {
+            return isNaN(n = +n) ? void 0 : u[Bo.bisect(a, n)]
+        }
+        var a;
+        return o.domain = function(u) {
+            return arguments.length ? (r = u.map(t).filter(e).sort(n), i()) : r
+        }, o.range = function(n) {
+            return arguments.length ? (u = n, i()) : u
+        }, o.quantiles = function() {
+            return a
+        }, o.invertExtent = function(n) {
+            return n = u.indexOf(n), 0 > n ? [0 / 0, 0 / 0] : [n > 0 ? a[n - 1] : r[0], n < a.length ? a[n] : r[r.length - 1]]
+        }, o.copy = function() {
+            return Qi(r, u)
+        }, i()
+    }
 
-                function Ko(n) {
-                    return n.join("L") + "Z"
-                }
+    function no(n, t, e) {
+        function r(t) {
+            return e[Math.max(0, Math.min(o, Math.floor(i * (t - n))))]
+        }
 
-                function Qo(n) {
-                    for (var t = 0, e = n.length, r = n[0], i = [r[0], ",", r[1]]; ++t < e;) i.push("V", (r = n[t])[1], "H", r[0]);
-                    return i.join("")
-                }
+        function u() {
+            return i = e.length / (t - n), o = e.length - 1, r
+        }
+        var i, o;
+        return r.domain = function(e) {
+            return arguments.length ? (n = +e[0], t = +e[e.length - 1], u()) : [n, t]
+        }, r.range = function(n) {
+            return arguments.length ? (e = n, u()) : e
+        }, r.invertExtent = function(t) {
+            return t = e.indexOf(t), t = 0 > t ? 0 / 0 : t / i + n, [t, t + 1 / i]
+        }, r.copy = function() {
+            return no(n, t, e)
+        }, u()
+    }
 
-                function na(n) {
-                    for (var t = 0, e = n.length, r = n[0], i = [r[0], ",", r[1]]; ++t < e;) i.push("H", (r = n[t])[0], "V", r[1]);
-                    return i.join("")
-                }
+    function to(n, t) {
+        function e(e) {
+            return e >= e ? t[Bo.bisect(n, e)] : void 0
+        }
+        return e.domain = function(t) {
+            return arguments.length ? (n = t, e) : n
+        }, e.range = function(n) {
+            return arguments.length ? (t = n, e) : t
+        }, e.invertExtent = function(e) {
+            return e = t.indexOf(e), [n[e - 1], n[e]]
+        }, e.copy = function() {
+            return to(n, t)
+        }, e
+    }
 
-                function ta(n, t) {
-                    if (t.length < 1 || n.length != t.length && n.length != t.length + 2) return Go(n);
-                    var e = n.length != t.length,
-                        r = "",
-                        i = n[0],
-                        u = n[1],
-                        o = t[0],
-                        a = o,
-                        l = 1;
-                    if (e && (r += "Q" + (u[0] - 2 * o[0] / 3) + "," + (u[1] - 2 * o[1] / 3) + "," + u[0] + "," + u[1], i = n[1], l = 2), t.length > 1) {
-                        a = t[1], u = n[l], l++, r += "C" + (i[0] + o[0]) + "," + (i[1] + o[1]) + "," + (u[0] - a[0]) + "," + (u[1] - a[1]) + "," + u[0] + "," + u[1];
-                        for (var c = 2; c < t.length; c++, l++) u = n[l], a = t[c], r += "S" + (u[0] - a[0]) + "," + (u[1] - a[1]) + "," + u[0] + "," + u[1]
-                    }
-                    if (e) {
-                        var f = n[l];
-                        r += "Q" + (u[0] + 2 * a[0] / 3) + "," + (u[1] + 2 * a[1] / 3) + "," + f[0] + "," + f[1]
-                    }
-                    return r
-                }
+    function eo(n) {
+        function t(n) {
+            return +n
+        }
+        return t.invert = t, t.domain = t.range = function(e) {
+            return arguments.length ? (n = e.map(t), t) : n
+        }, t.ticks = function(t) {
+            return Vi(n, t)
+        }, t.tickFormat = function(t, e) {
+            return Xi(n, t, e)
+        }, t.copy = function() {
+            return eo(n)
+        }, t
+    }
 
-                function ea(n, t) {
-                    for (var e, r = [], i = (1 - t) / 2, u = n[0], o = n[1], a = 1, l = n.length; ++a < l;) e = u, u = o, o = n[a], r.push([i * (o[0] - e[0]), i * (o[1] - e[1])]);
-                    return r
-                }
-
-                function ra(n) {
-                    if (n.length < 3) return Go(n);
-                    var t = 1,
-                        e = n.length,
-                        r = n[0],
-                        i = r[0],
-                        u = r[1],
-                        o = [i, i, i, (r = n[1])[0]],
-                        a = [u, u, u, r[1]],
-                        l = [i, ",", u, "L", ia(aa, o), ",", ia(aa, a)];
-                    for (n.push(n[e - 1]); ++t <= e;) r = n[t], o.shift(), o.push(r[0]), a.shift(), a.push(r[1]), la(l, o, a);
-                    return n.pop(), l.push("L", r), l.join("")
-                }
-
-                function ia(n, t) {
-                    return n[0] * t[0] + n[1] * t[1] + n[2] * t[2] + n[3] * t[3]
-                }
-                Wo.forEach((function(n, t) {
-                    t.key = n, t.closed = /-closed$/.test(n)
-                }));
-                var ua = [0, 2 / 3, 1 / 3, 0],
-                    oa = [0, 1 / 3, 2 / 3, 0],
-                    aa = [0, 1 / 6, 2 / 3, 1 / 6];
-
-                function la(n, t, e) {
-                    n.push("C", ia(ua, t), ",", ia(ua, e), ",", ia(oa, t), ",", ia(oa, e), ",", ia(aa, t), ",", ia(aa, e))
-                }
-
-                function ca(n, t) {
-                    return (t[1] - n[1]) / (t[0] - n[0])
-                }
-
-                function fa(n) {
-                    for (var t, e, r, i = -1, u = n.length; ++i < u;) e = (t = n[i])[0], r = t[1] - Rn, t[0] = e * Math.cos(r), t[1] = e * Math.sin(r);
-                    return n
-                }
-
-                function sa(n) {
-                    var t = oi,
-                        e = oi,
-                        r = 0,
-                        i = ai,
-                        u = Ge,
-                        o = Go,
-                        a = o.key,
-                        l = o,
-                        c = "L",
-                        f = .7;
-
-                    function s(a) {
-                        var s, h, p, g = [],
-                            v = [],
-                            d = [],
-                            y = -1,
-                            m = a.length,
-                            M = Mt(t),
-                            x = Mt(r),
-                            b = t === e ? function() {
-                                return h
-                            } : Mt(e),
-                            w = r === i ? function() {
-                                return p
-                            } : Mt(i);
+    function ro(n) {
+        return n.innerRadius
+    }
 
-                        function _() {
-                            g.push("M", o(n(d), f), c, l(n(v.reverse()), f), "Z")
-                        }
-                        for (; ++y < m;) u.call(this, s = a[y], y) ? (v.push([h = +M.call(this, s, y), p = +x.call(this, s, y)]), d.push([+b.call(this, s, y), +w.call(this, s, y)])) : v.length && (_(), v = [], d = []);
-                        return v.length && _(), g.length ? g.join("") : null
-                    }
-                    return s.x = function(n) {
-                        return arguments.length ? (t = e = n, s) : e
-                    }, s.x0 = function(n) {
-                        return arguments.length ? (t = n, s) : t
-                    }, s.x1 = function(n) {
-                        return arguments.length ? (e = n, s) : e
-                    }, s.y = function(n) {
-                        return arguments.length ? (r = i = n, s) : i
-                    }, s.y0 = function(n) {
-                        return arguments.length ? (r = n, s) : r
-                    }, s.y1 = function(n) {
-                        return arguments.length ? (i = n, s) : i
-                    }, s.defined = function(n) {
-                        return arguments.length ? (u = n, s) : u
-                    }, s.interpolate = function(n) {
-                        return arguments.length ? (a = "function" == typeof n ? o = n : (o = Wo.get(n) || Go).key, l = o.reverse || o, c = o.closed ? "M" : "L", s) : a
-                    }, s.tension = function(n) {
-                        return arguments.length ? (f = n, s) : f
-                    }, s
-                }
-
-                function ha(n) {
-                    return n.radius
-                }
-
-                function pa(n) {
-                    return [n.x, n.y]
-                }
-
-                function ga(n) {
-                    return function() {
-                        var t = n.apply(this, arguments),
-                            e = t[0],
-                            r = t[1] - Rn;
-                        return [e * Math.cos(r), e * Math.sin(r)]
-                    }
-                }
+    function uo(n) {
+        return n.outerRadius
+    }
 
-                function va() {
-                    return 64
-                }
+    function io(n) {
+        return n.startAngle
+    }
 
-                function da() {
-                    return "circle"
-                }
+    function oo(n) {
+        return n.endAngle
+    }
 
-                function ya(n) {
-                    var t = Math.sqrt(n / Ln);
-                    return "M0," + t + "A" + t + "," + t + " 0 1,1 0," + -t + "A" + t + "," + t + " 0 1,1 0," + t + "Z"
-                }
-                u.svg.line.radial = function() {
-                    var n = Jo(fa);
-                    return n.radius = n.x, delete n.x, n.angle = n.y, delete n.y, n
-                }, Qo.reverse = na, na.reverse = Qo, u.svg.area = function() {
-                    return sa(R)
-                }, u.svg.area.radial = function() {
-                    var n = sa(fa);
-                    return n.radius = n.x, delete n.x, n.innerRadius = n.x0, delete n.x0, n.outerRadius = n.x1, delete n.x1, n.angle = n.y, delete n.y, n.startAngle = n.y0, delete n.y0, n.endAngle = n.y1, delete n.y1, n
-                }, u.svg.chord = function() {
-                    var n = Xr,
-                        t = $r,
-                        e = ha,
-                        r = Zo,
-                        i = Vo;
-
-                    function u(e, r) {
-                        var i, u, c = o(this, n, e, r),
-                            f = o(this, t, e, r);
-                        return "M" + c.p0 + a(c.r, c.p1, c.a1 - c.a0) + (u = f, ((i = c).a0 == u.a0 && i.a1 == u.a1 ? l(c.r, c.p1, c.r, c.p0) : l(c.r, c.p1, f.r, f.p0) + a(f.r, f.p1, f.a1 - f.a0) + l(f.r, f.p1, c.r, c.p0)) + "Z")
-                    }
+    function ao(n) {
+        function t(t) {
+            function o() {
+                l.push("M", i(n(s), a))
+            }
+            for (var c, l = [], s = [], f = -1, h = t.length, g = kt(e), p = kt(r); ++f < h;) u.call(this, c = t[f], f) ? s.push([+g.call(this, c, f), +p.call(this, c, f)]) : s.length && (o(), s = []);
+            return s.length && o(), l.length ? l.join("") : null
+        }
+        var e = Ar,
+            r = Cr,
+            u = Ae,
+            i = co,
+            o = i.key,
+            a = .7;
+        return t.x = function(n) {
+            return arguments.length ? (e = n, t) : e
+        }, t.y = function(n) {
+            return arguments.length ? (r = n, t) : r
+        }, t.defined = function(n) {
+            return arguments.length ? (u = n, t) : u
+        }, t.interpolate = function(n) {
+            return arguments.length ? (o = "function" == typeof n ? i = n : (i = wl.get(n) || co).key, t) : o
+        }, t.tension = function(n) {
+            return arguments.length ? (a = n, t) : a
+        }, t
+    }
 
-                    function o(n, t, u, o) {
-                        var a = t.call(n, u, o),
-                            l = e.call(n, a, o),
-                            c = r.call(n, a, o) - Rn,
-                            f = i.call(n, a, o) - Rn;
-                        return {
-                            r: l,
-                            a0: c,
-                            a1: f,
-                            p0: [l * Math.cos(c), l * Math.sin(c)],
-                            p1: [l * Math.cos(f), l * Math.sin(f)]
-                        }
-                    }
+    function co(n) {
+        return n.join("L")
+    }
 
-                    function a(n, t, e) {
-                        return "A" + n + "," + n + " 0 " + +(e > Ln) + ",1 " + t
-                    }
+    function lo(n) {
+        return co(n) + "Z"
+    }
 
-                    function l(n, t, e, r) {
-                        return "Q 0,0 " + r
-                    }
-                    return u.radius = function(n) {
-                        return arguments.length ? (e = Mt(n), u) : e
-                    }, u.source = function(t) {
-                        return arguments.length ? (n = Mt(t), u) : n
-                    }, u.target = function(n) {
-                        return arguments.length ? (t = Mt(n), u) : t
-                    }, u.startAngle = function(n) {
-                        return arguments.length ? (r = Mt(n), u) : r
-                    }, u.endAngle = function(n) {
-                        return arguments.length ? (i = Mt(n), u) : i
-                    }, u
-                }, u.svg.diagonal = function() {
-                    var n = Xr,
-                        t = $r,
-                        e = pa;
-
-                    function r(r, i) {
-                        var u = n.call(this, r, i),
-                            o = t.call(this, r, i),
-                            a = (u.y + o.y) / 2,
-                            l = [u, {
-                                x: u.x,
-                                y: a
-                            }, {
-                                x: o.x,
-                                y: a
-                            }, o];
-                        return "M" + (l = l.map(e))[0] + "C" + l[1] + " " + l[2] + " " + l[3]
-                    }
-                    return r.source = function(t) {
-                        return arguments.length ? (n = Mt(t), r) : n
-                    }, r.target = function(n) {
-                        return arguments.length ? (t = Mt(n), r) : t
-                    }, r.projection = function(n) {
-                        return arguments.length ? (e = n, r) : e
-                    }, r
-                }, u.svg.diagonal.radial = function() {
-                    var n = u.svg.diagonal(),
-                        t = pa,
-                        e = n.projection;
-                    return n.projection = function(n) {
-                        return arguments.length ? e(ga(t = n)) : t
-                    }, n
-                }, u.svg.symbol = function() {
-                    var n = da,
-                        t = va;
+    function so(n) {
+        for (var t = 0, e = n.length, r = n[0], u = [r[0], ",", r[1]]; ++t < e;) u.push("H", (r[0] + (r = n[t])[0]) / 2, "V", r[1]);
+        return e > 1 && u.push("H", r[0]), u.join("")
+    }
 
-                    function e(e, r) {
-                        return (ma.get(n.call(this, e, r)) || ya)(t.call(this, e, r))
-                    }
-                    return e.type = function(t) {
-                        return arguments.length ? (n = Mt(t), e) : n
-                    }, e.size = function(n) {
-                        return arguments.length ? (t = Mt(n), e) : t
-                    }, e
-                };
-                var ma = u.map({
-                    circle: ya,
-                    cross: function(n) {
-                        var t = Math.sqrt(n / 5) / 2;
-                        return "M" + -3 * t + "," + -t + "H" + -t + "V" + -3 * t + "H" + t + "V" + -t + "H" + 3 * t + "V" + t + "H" + t + "V" + 3 * t + "H" + -t + "V" + t + "H" + -3 * t + "Z"
-                    },
-                    diamond: function(n) {
-                        var t = Math.sqrt(n / (2 * xa)),
-                            e = t * xa;
-                        return "M0," + -t + "L" + e + ",0 0," + t + " " + -e + ",0Z"
-                    },
-                    square: function(n) {
-                        var t = Math.sqrt(n) / 2;
-                        return "M" + -t + "," + -t + "L" + t + "," + -t + " " + t + "," + t + " " + -t + "," + t + "Z"
-                    },
-                    "triangle-down": function(n) {
-                        var t = Math.sqrt(n / Ma),
-                            e = t * Ma / 2;
-                        return "M0," + e + "L" + t + "," + -e + " " + -t + "," + -e + "Z"
-                    },
-                    "triangle-up": function(n) {
-                        var t = Math.sqrt(n / Ma),
-                            e = t * Ma / 2;
-                        return "M0," + -e + "L" + t + "," + e + " " + -t + "," + e + "Z"
-                    }
-                });
-                u.svg.symbolTypes = ma.keys();
-                var Ma = Math.sqrt(3),
-                    xa = Math.tan(30 * Dn);
-                W.transition = function(n) {
-                    for (var t, e, r = ka || ++Ea, i = za(n), u = [], o = Sa || {
-                            time: Date.now(),
-                            ease: pu,
-                            delay: 0,
-                            duration: 250
-                        }, a = -1, l = this.length; ++a < l;) {
-                        u.push(t = []);
-                        for (var c = this[a], f = -1, s = c.length; ++f < s;)(e = c[f]) && La(e, f, i, r, o), t.push(e)
-                    }
-                    return _a(u, i, r)
-                }, W.interrupt = function(n) {
-                    return this.each(null == n ? ba : wa(za(n)))
-                };
-                var ba = wa(za());
+    function fo(n) {
+        for (var t = 0, e = n.length, r = n[0], u = [r[0], ",", r[1]]; ++t < e;) u.push("V", (r = n[t])[1], "H", r[0]);
+        return u.join("")
+    }
 
-                function wa(n) {
-                    return function() {
-                        var t, e, r;
-                        (t = this[n]) && (r = t[e = t.active]) && (r.timer.c = null, r.timer.t = NaN, --t.count ? delete t[e] : delete this[n], t.active += .5, r.event && r.event.interrupt.call(this, this.__data__, r.index))
-                    }
-                }
+    function ho(n) {
+        for (var t = 0, e = n.length, r = n[0], u = [r[0], ",", r[1]]; ++t < e;) u.push("H", (r = n[t])[0], "V", r[1]);
+        return u.join("")
+    }
+
+    function go(n, t) {
+        return n.length < 4 ? co(n) : n[1] + mo(n.slice(1, n.length - 1), yo(n, t))
+    }
+
+    function po(n, t) {
+        return n.length < 3 ? co(n) : n[0] + mo((n.push(n[0]), n), yo([n[n.length - 2]].concat(n, [n[1]]), t))
+    }
+
+    function vo(n, t) {
+        return n.length < 3 ? co(n) : n[0] + mo(n, yo(n, t))
+    }
+
+    function mo(n, t) {
+        if (t.length < 1 || n.length != t.length && n.length != t.length + 2) return co(n);
+        var e = n.length != t.length,
+            r = "",
+            u = n[0],
+            i = n[1],
+            o = t[0],
+            a = o,
+            c = 1;
+        if (e && (r += "Q" + (i[0] - 2 * o[0] / 3) + "," + (i[1] - 2 * o[1] / 3) + "," + i[0] + "," + i[1], u = n[1], c = 2), t.length > 1) {
+            a = t[1], i = n[c], c++, r += "C" + (u[0] + o[0]) + "," + (u[1] + o[1]) + "," + (i[0] - a[0]) + "," + (i[1] - a[1]) + "," + i[0] + "," + i[1];
+            for (var l = 2; l < t.length; l++, c++) i = n[c], a = t[l], r += "S" + (i[0] - a[0]) + "," + (i[1] - a[1]) + "," + i[0] + "," + i[1]
+        }
+        if (e) {
+            var s = n[c];
+            r += "Q" + (i[0] + 2 * a[0] / 3) + "," + (i[1] + 2 * a[1] / 3) + "," + s[0] + "," + s[1]
+        }
+        return r
+    }
+
+    function yo(n, t) {
+        for (var e, r = [], u = (1 - t) / 2, i = n[0], o = n[1], a = 1, c = n.length; ++a < c;) e = i, i = o, o = n[a], r.push([u * (o[0] - e[0]), u * (o[1] - e[1])]);
+        return r
+    }
+
+    function xo(n) {
+        if (n.length < 3) return co(n);
+        var t = 1,
+            e = n.length,
+            r = n[0],
+            u = r[0],
+            i = r[1],
+            o = [u, u, u, (r = n[1])[0]],
+            a = [i, i, i, r[1]],
+            c = [u, ",", i, "L", wo(El, o), ",", wo(El, a)];
+        for (n.push(n[e - 1]); ++t <= e;) r = n[t], o.shift(), o.push(r[0]), a.shift(), a.push(r[1]), So(c, o, a);
+        return n.pop(), c.push("L", r), c.join("")
+    }
+
+    function Mo(n) {
+        if (n.length < 4) return co(n);
+        for (var t, e = [], r = -1, u = n.length, i = [0], o = [0]; ++r < 3;) t = n[r], i.push(t[0]), o.push(t[1]);
+        for (e.push(wo(El, i) + "," + wo(El, o)), --r; ++r < u;) t = n[r], i.shift(), i.push(t[0]), o.shift(), o.push(t[1]), So(e, i, o);
+        return e.join("")
+    }
+
+    function _o(n) {
+        for (var t, e, r = -1, u = n.length, i = u + 4, o = [], a = []; ++r < 4;) e = n[r % u], o.push(e[0]), a.push(e[1]);
+        for (t = [wo(El, o), ",", wo(El, a)], --r; ++r < i;) e = n[r % u], o.shift(), o.push(e[0]), a.shift(), a.push(e[1]), So(t, o, a);
+        return t.join("")
+    }
+
+    function bo(n, t) {
+        var e = n.length - 1;
+        if (e)
+            for (var r, u, i = n[0][0], o = n[0][1], a = n[e][0] - i, c = n[e][1] - o, l = -1; ++l <= e;) r = n[l], u = l / e, r[0] = t * r[0] + (1 - t) * (i + u * a), r[1] = t * r[1] + (1 - t) * (o + u * c);
+        return xo(n)
+    }
+
+    function wo(n, t) {
+        return n[0] * t[0] + n[1] * t[1] + n[2] * t[2] + n[3] * t[3]
+    }
+
+    function So(n, t, e) {
+        n.push("C", wo(Sl, t), ",", wo(Sl, e), ",", wo(kl, t), ",", wo(kl, e), ",", wo(El, t), ",", wo(El, e))
+    }
+
+    function ko(n, t) {
+        return (t[1] - n[1]) / (t[0] - n[0])
+    }
+
+    function Eo(n) {
+        for (var t = 0, e = n.length - 1, r = [], u = n[0], i = n[1], o = r[0] = ko(u, i); ++t < e;) r[t] = (o + (o = ko(u = i, i = n[t + 1]))) / 2;
+        return r[t] = o, r
+    }
+
+    function Ao(n) {
+        for (var t, e, r, u, i = [], o = Eo(n), a = -1, c = n.length - 1; ++a < c;) t = ko(n[a], n[a + 1]), ca(t) < Na ? o[a] = o[a + 1] = 0 : (e = o[a] / t, r = o[a + 1] / t, u = e * e + r * r, u > 9 && (u = 3 * t / Math.sqrt(u), o[a] = u * e, o[a + 1] = u * r));
+        for (a = -1; ++a <= c;) u = (n[Math.min(c, a + 1)][0] - n[Math.max(0, a - 1)][0]) / (6 * (1 + o[a] * o[a])), i.push([u || 0, o[a] * u || 0]);
+        return i
+    }
 
-                function _a(n, t, e) {
-                    return V(n, Na), n.namespace = t, n.id = e, n
+    function Co(n) {
+        return n.length < 3 ? co(n) : n[0] + mo(n, Ao(n))
+    }
+
+    function No(n) {
+        for (var t, e, r, u = -1, i = n.length; ++u < i;) t = n[u], e = t[0], r = t[1] + _l, t[0] = e * Math.cos(r), t[1] = e * Math.sin(r);
+        return n
+    }
+
+    function zo(n) {
+        function t(t) {
+            function c() {
+                v.push("M", a(n(m), f), s, l(n(d.reverse()), f), "Z")
+            }
+            for (var h, g, p, v = [], d = [], m = [], y = -1, x = t.length, M = kt(e), _ = kt(u), b = e === r ? function() {
+                    return g
+                } : kt(r), w = u === i ? function() {
+                    return p
+                } : kt(i); ++y < x;) o.call(this, h = t[y], y) ? (d.push([g = +M.call(this, h, y), p = +_.call(this, h, y)]), m.push([+b.call(this, h, y), +w.call(this, h, y)])) : d.length && (c(), d = [], m = []);
+            return d.length && c(), v.length ? v.join("") : null
+        }
+        var e = Ar,
+            r = Ar,
+            u = 0,
+            i = Cr,
+            o = Ae,
+            a = co,
+            c = a.key,
+            l = a,
+            s = "L",
+            f = .7;
+        return t.x = function(n) {
+            return arguments.length ? (e = r = n, t) : r
+        }, t.x0 = function(n) {
+            return arguments.length ? (e = n, t) : e
+        }, t.x1 = function(n) {
+            return arguments.length ? (r = n, t) : r
+        }, t.y = function(n) {
+            return arguments.length ? (u = i = n, t) : i
+        }, t.y0 = function(n) {
+            return arguments.length ? (u = n, t) : u
+        }, t.y1 = function(n) {
+            return arguments.length ? (i = n, t) : i
+        }, t.defined = function(n) {
+            return arguments.length ? (o = n, t) : o
+        }, t.interpolate = function(n) {
+            return arguments.length ? (c = "function" == typeof n ? a = n : (a = wl.get(n) || co).key, l = a.reverse || a, s = a.closed ? "M" : "L", t) : c
+        }, t.tension = function(n) {
+            return arguments.length ? (f = n, t) : f
+        }, t
+    }
+
+    function Lo(n) {
+        return n.radius
+    }
+
+    function To(n) {
+        return [n.x, n.y]
+    }
+
+    function qo(n) {
+        return function() {
+            var t = n.apply(this, arguments),
+                e = t[0],
+                r = t[1] + _l;
+            return [e * Math.cos(r), e * Math.sin(r)]
+        }
+    }
+
+    function Ro() {
+        return 64
+    }
+
+    function Do() {
+        return "circle"
+    }
+
+    function Po(n) {
+        var t = Math.sqrt(n / Ea);
+        return "M0," + t + "A" + t + "," + t + " 0 1,1 0," + -t + "A" + t + "," + t + " 0 1,1 0," + t + "Z"
+    }
+
+    function Uo(n, t) {
+        return ga(n, Tl), n.id = t, n
+    }
+
+    function jo(n, t, e, r) {
+        var u = n.id;
+        return F(n, "function" == typeof e ? function(n, i, o) {
+            n.__transition__[u].tween.set(t, r(e.call(n, n.__data__, i, o)))
+        } : (e = r(e), function(n) {
+            n.__transition__[u].tween.set(t, e)
+        }))
+    }
+
+    function Fo(n) {
+        return null == n && (n = ""),
+            function() {
+                this.textContent = n
+            }
+    }
+
+    function Ho(n, t, e, r) {
+        var u = n.__transition__ || (n.__transition__ = {
+                active: 0,
+                count: 0
+            }),
+            i = u[e];
+        if (!i) {
+            var o = r.time;
+            i = u[e] = {
+                tween: new a,
+                time: o,
+                ease: r.ease,
+                delay: r.delay,
+                duration: r.duration
+            }, ++u.count, Bo.timer(function(r) {
+                function a(r) {
+                    return u.active > e ? l() : (u.active = e, i.event && i.event.start.call(n, s, t), i.tween.forEach(function(e, r) {
+                        (r = r.call(n, s, t)) && v.push(r)
+                    }), Bo.timer(function() {
+                        return p.c = c(r || 1) ? Ae : c, 1
+                    }, 0, o), void 0)
+                }
+
+                function c(r) {
+                    if (u.active !== e) return l();
+                    for (var o = r / g, a = f(o), c = v.length; c > 0;) v[--c].call(n, a);
+                    return o >= 1 ? (i.event && i.event.end.call(n, s, t), l()) : void 0
+                }
+
+                function l() {
+                    return --u.count ? delete u[e] : delete n.__transition__, 1
+                }
+                var s = n.__data__,
+                    f = i.ease,
+                    h = i.delay,
+                    g = i.duration,
+                    p = Ka,
+                    v = [];
+                return p.t = h + o, r >= h ? a(r - h) : (p.c = a, void 0)
+            }, 0, o)
+        }
+    }
+
+    function Oo(n, t, e) {
+        n.attr("transform", function(n) {
+            var r = t(n);
+            return "translate(" + (isFinite(r) ? r : e(n)) + ",0)"
+        })
+    }
+
+    function Yo(n, t, e) {
+        n.attr("transform", function(n) {
+            var r = t(n);
+            return "translate(0," + (isFinite(r) ? r : e(n)) + ")"
+        })
+    }
+
+    function Io(n) {
+        return n.toISOString()
+    }
+
+    function Zo(n, t, e) {
+        function r(t) {
+            return n(t)
+        }
+
+        function u(n, e) {
+            var r = n[1] - n[0],
+                u = r / e,
+                i = Bo.bisect(Ol, u);
+            return i == Ol.length ? [t.year, Zi(n.map(function(n) {
+                return n / 31536e6
+            }), e)[2]] : i ? t[u / Ol[i - 1] < Ol[i] / u ? i - 1 : i] : [Zl, Zi(n, e)[2]]
+        }
+        return r.invert = function(t) {
+            return Vo(n.invert(t))
+        }, r.domain = function(t) {
+            return arguments.length ? (n.domain(t), r) : n.domain().map(Vo)
+        }, r.nice = function(n, t) {
+            function e(e) {
+                return !isNaN(e) && !n.range(e, Vo(+e + 1), t).length
+            }
+            var i = r.domain(),
+                o = Di(i),
+                a = null == n ? u(o, 10) : "number" == typeof n && u(o, n);
+            return a && (n = a[0], t = a[1]), r.domain(ji(i, t > 1 ? {
+                floor: function(t) {
+                    for (; e(t = n.floor(t));) t = Vo(t - 1);
+                    return t
+                },
+                ceil: function(t) {
+                    for (; e(t = n.ceil(t));) t = Vo(+t + 1);
+                    return t
                 }
-                var ka, Sa, Na = [],
-                    Ea = 0;
+            } : n))
+        }, r.ticks = function(n, t) {
+            var e = Di(r.domain()),
+                i = null == n ? u(e, 10) : "number" == typeof n ? u(e, n) : !n.range && [{
+                    range: n
+                }, t];
+            return i && (n = i[0], t = i[1]), n.range(e[0], Vo(+e[1] + 1), 1 > t ? 1 : t)
+        }, r.tickFormat = function() {
+            return e
+        }, r.copy = function() {
+            return Zo(n.copy(), t, e)
+        }, Yi(r, n)
+    }
 
-                function Aa(n, t, e, r) {
-                    var i = n.id,
-                        u = n.namespace;
-                    return vn(n, "function" == typeof e ? function(n, o, a) {
-                        n[u][i].tween.set(t, r(e.call(n, n.__data__, o, a)))
-                    } : (e = r(e), function(n) {
-                        n[u][i].tween.set(t, e)
+    function Vo(n) {
+        return new Date(n)
+    }
+
+    function Xo(n) {
+        return JSON.parse(n.responseText)
+    }
+
+    function $o(n) {
+        var t = Go.createRange();
+        return t.selectNode(Go.body), t.createContextualFragment(n.responseText)
+    }
+    var Bo = {
+        version: "3.4.13"
+    };
+    Date.now || (Date.now = function() {
+        return +new Date
+    });
+    var Wo = [].slice,
+        Jo = function(n) {
+            return Wo.call(n)
+        },
+        Go = document,
+        Ko = Go.documentElement,
+        Qo = window;
+    try {
+        Jo(Ko.childNodes)[0].nodeType
+    } catch (na) {
+        Jo = function(n) {
+            for (var t = n.length, e = new Array(t); t--;) e[t] = n[t];
+            return e
+        }
+    }
+    try {
+        Go.createElement("div").style.setProperty("opacity", 0, "")
+    } catch (ta) {
+        var ea = Qo.Element.prototype,
+            ra = ea.setAttribute,
+            ua = ea.setAttributeNS,
+            ia = Qo.CSSStyleDeclaration.prototype,
+            oa = ia.setProperty;
+        ea.setAttribute = function(n, t) {
+            ra.call(this, n, t + "")
+        }, ea.setAttributeNS = function(n, t, e) {
+            ua.call(this, n, t, e + "")
+        }, ia.setProperty = function(n, t, e) {
+            oa.call(this, n, t + "", e)
+        }
+    }
+    Bo.ascending = n, Bo.descending = function(n, t) {
+        return n > t ? -1 : t > n ? 1 : t >= n ? 0 : 0 / 0
+    }, Bo.min = function(n, t) {
+        var e, r, u = -1,
+            i = n.length;
+        if (1 === arguments.length) {
+            for (; ++u < i && !(null != (e = n[u]) && e >= e);) e = void 0;
+            for (; ++u < i;) null != (r = n[u]) && e > r && (e = r)
+        } else {
+            for (; ++u < i && !(null != (e = t.call(n, n[u], u)) && e >= e);) e = void 0;
+            for (; ++u < i;) null != (r = t.call(n, n[u], u)) && e > r && (e = r)
+        }
+        return e
+    }, Bo.max = function(n, t) {
+        var e, r, u = -1,
+            i = n.length;
+        if (1 === arguments.length) {
+            for (; ++u < i && !(null != (e = n[u]) && e >= e);) e = void 0;
+            for (; ++u < i;) null != (r = n[u]) && r > e && (e = r)
+        } else {
+            for (; ++u < i && !(null != (e = t.call(n, n[u], u)) && e >= e);) e = void 0;
+            for (; ++u < i;) null != (r = t.call(n, n[u], u)) && r > e && (e = r)
+        }
+        return e
+    }, Bo.extent = function(n, t) {
+        var e, r, u, i = -1,
+            o = n.length;
+        if (1 === arguments.length) {
+            for (; ++i < o && !(null != (e = u = n[i]) && e >= e);) e = u = void 0;
+            for (; ++i < o;) null != (r = n[i]) && (e > r && (e = r), r > u && (u = r))
+        } else {
+            for (; ++i < o && !(null != (e = u = t.call(n, n[i], i)) && e >= e);) e = void 0;
+            for (; ++i < o;) null != (r = t.call(n, n[i], i)) && (e > r && (e = r), r > u && (u = r))
+        }
+        return [e, u]
+    }, Bo.sum = function(n, t) {
+        var r, u = 0,
+            i = n.length,
+            o = -1;
+        if (1 === arguments.length)
+            for (; ++o < i;) e(r = +n[o]) && (u += r);
+        else
+            for (; ++o < i;) e(r = +t.call(n, n[o], o)) && (u += r);
+        return u
+    }, Bo.mean = function(n, r) {
+        var u, i = 0,
+            o = n.length,
+            a = -1,
+            c = o;
+        if (1 === arguments.length)
+            for (; ++a < o;) e(u = t(n[a])) ? i += u : --c;
+        else
+            for (; ++a < o;) e(u = t(r.call(n, n[a], a))) ? i += u : --c;
+        return c ? i / c : void 0
+    }, Bo.quantile = function(n, t) {
+        var e = (n.length - 1) * t + 1,
+            r = Math.floor(e),
+            u = +n[r - 1],
+            i = e - r;
+        return i ? u + i * (n[r] - u) : u
+    }, Bo.median = function(r, u) {
+        var i, o = [],
+            a = r.length,
+            c = -1;
+        if (1 === arguments.length)
+            for (; ++c < a;) e(i = t(r[c])) && o.push(i);
+        else
+            for (; ++c < a;) e(i = t(u.call(r, r[c], c))) && o.push(i);
+        return o.length ? Bo.quantile(o.sort(n), .5) : void 0
+    };
+    var aa = r(n);
+    Bo.bisectLeft = aa.left, Bo.bisect = Bo.bisectRight = aa.right, Bo.bisector = function(t) {
+        return r(1 === t.length ? function(e, r) {
+            return n(t(e), r)
+        } : t)
+    }, Bo.shuffle = function(n) {
+        for (var t, e, r = n.length; r;) e = 0 | Math.random() * r--, t = n[r], n[r] = n[e], n[e] = t;
+        return n
+    }, Bo.permute = function(n, t) {
+        for (var e = t.length, r = new Array(e); e--;) r[e] = n[t[e]];
+        return r
+    }, Bo.pairs = function(n) {
+        for (var t, e = 0, r = n.length - 1, u = n[0], i = new Array(0 > r ? 0 : r); r > e;) i[e] = [t = u, u = n[++e]];
+        return i
+    }, Bo.zip = function() {
+        if (!(r = arguments.length)) return [];
+        for (var n = -1, t = Bo.min(arguments, u), e = new Array(t); ++n < t;)
+            for (var r, i = -1, o = e[n] = new Array(r); ++i < r;) o[i] = arguments[i][n];
+        return e
+    }, Bo.transpose = function(n) {
+        return Bo.zip.apply(Bo, n)
+    }, Bo.keys = function(n) {
+        var t = [];
+        for (var e in n) t.push(e);
+        return t
+    }, Bo.values = function(n) {
+        var t = [];
+        for (var e in n) t.push(n[e]);
+        return t
+    }, Bo.entries = function(n) {
+        var t = [];
+        for (var e in n) t.push({
+            key: e,
+            value: n[e]
+        });
+        return t
+    }, Bo.merge = function(n) {
+        for (var t, e, r, u = n.length, i = -1, o = 0; ++i < u;) o += n[i].length;
+        for (e = new Array(o); --u >= 0;)
+            for (r = n[u], t = r.length; --t >= 0;) e[--o] = r[t];
+        return e
+    };
+    var ca = Math.abs;
+    Bo.range = function(n, t, e) {
+        if (arguments.length < 3 && (e = 1, arguments.length < 2 && (t = n, n = 0)), 1 / 0 === (t - n) / e) throw new Error("infinite range");
+        var r, u = [],
+            o = i(ca(e)),
+            a = -1;
+        if (n *= o, t *= o, e *= o, 0 > e)
+            for (;
+                (r = n + e * ++a) > t;) u.push(r / o);
+        else
+            for (;
+                (r = n + e * ++a) < t;) u.push(r / o);
+        return u
+    }, Bo.map = function(n) {
+        var t = new a;
+        if (n instanceof a) n.forEach(function(n, e) {
+            t.set(n, e)
+        });
+        else
+            for (var e in n) t.set(e, n[e]);
+        return t
+    };
+    var la = "__proto__",
+        sa = "\x00";
+    o(a, {
+        has: s,
+        get: function(n) {
+            return this._[c(n)]
+        },
+        set: function(n, t) {
+            return this._[c(n)] = t
+        },
+        remove: f,
+        keys: h,
+        values: function() {
+            var n = [];
+            for (var t in this._) n.push(this._[t]);
+            return n
+        },
+        entries: function() {
+            var n = [];
+            for (var t in this._) n.push({
+                key: l(t),
+                value: this._[t]
+            });
+            return n
+        },
+        size: g,
+        empty: p,
+        forEach: function(n) {
+            for (var t in this._) n.call(this, l(t), this._[t])
+        }
+    }), Bo.nest = function() {
+        function n(t, o, c) {
+            if (c >= i.length) return r ? r.call(u, o) : e ? o.sort(e) : o;
+            for (var l, s, f, h, g = -1, p = o.length, v = i[c++], d = new a; ++g < p;)(h = d.get(l = v(s = o[g]))) ? h.push(s) : d.set(l, [s]);
+            return t ? (s = t(), f = function(e, r) {
+                s.set(e, n(t, r, c))
+            }) : (s = {}, f = function(e, r) {
+                s[e] = n(t, r, c)
+            }), d.forEach(f), s
+        }
+
+        function t(n, e) {
+            if (e >= i.length) return n;
+            var r = [],
+                u = o[e++];
+            return n.forEach(function(n, u) {
+                r.push({
+                    key: n,
+                    values: t(u, e)
+                })
+            }), u ? r.sort(function(n, t) {
+                return u(n.key, t.key)
+            }) : r
+        }
+        var e, r, u = {},
+            i = [],
+            o = [];
+        return u.map = function(t, e) {
+            return n(e, t, 0)
+        }, u.entries = function(e) {
+            return t(n(Bo.map, e, 0), 0)
+        }, u.key = function(n) {
+            return i.push(n), u
+        }, u.sortKeys = function(n) {
+            return o[i.length - 1] = n, u
+        }, u.sortValues = function(n) {
+            return e = n, u
+        }, u.rollup = function(n) {
+            return r = n, u
+        }, u
+    }, Bo.set = function(n) {
+        var t = new v;
+        if (n)
+            for (var e = 0, r = n.length; r > e; ++e) t.add(n[e]);
+        return t
+    }, o(v, {
+        has: s,
+        add: function(n) {
+            return this._[c(n += "")] = !0, n
+        },
+        remove: f,
+        values: h,
+        size: g,
+        empty: p,
+        forEach: function(n) {
+            for (var t in this._) n.call(this, l(t))
+        }
+    }), Bo.behavior = {}, Bo.rebind = function(n, t) {
+        for (var e, r = 1, u = arguments.length; ++r < u;) n[e = arguments[r]] = d(n, t, t[e]);
+        return n
+    };
+    var fa = ["webkit", "ms", "moz", "Moz", "o", "O"];
+    Bo.dispatch = function() {
+        for (var n = new x, t = -1, e = arguments.length; ++t < e;) n[arguments[t]] = M(n);
+        return n
+    }, x.prototype.on = function(n, t) {
+        var e = n.indexOf("."),
+            r = "";
+        if (e >= 0 && (r = n.slice(e + 1), n = n.slice(0, e)), n) return arguments.length < 2 ? this[n].on(r) : this[n].on(r, t);
+        if (2 === arguments.length) {
+            if (null == t)
+                for (n in this) this.hasOwnProperty(n) && this[n].on(r, null);
+            return this
+        }
+    }, Bo.event = null, Bo.requote = function(n) {
+        return n.replace(ha, "\\$&")
+    };
+    var ha = /[\\\^\$\*\+\?\|\[\]\(\)\.\{\}]/g,
+        ga = {}.__proto__ ? function(n, t) {
+            n.__proto__ = t
+        } : function(n, t) {
+            for (var e in t) n[e] = t[e]
+        },
+        pa = function(n, t) {
+            return t.querySelector(n)
+        },
+        va = function(n, t) {
+            return t.querySelectorAll(n)
+        },
+        da = Ko.matches || Ko[m(Ko, "matchesSelector")],
+        ma = function(n, t) {
+            return da.call(n, t)
+        };
+    "function" == typeof Sizzle && (pa = function(n, t) {
+        return Sizzle(n, t)[0] || null
+    }, va = Sizzle, ma = Sizzle.matchesSelector), Bo.selection = function() {
+        return _a
+    };
+    var ya = Bo.selection.prototype = [];
+    ya.select = function(n) {
+        var t, e, r, u, i = [];
+        n = k(n);
+        for (var o = -1, a = this.length; ++o < a;) {
+            i.push(t = []), t.parentNode = (r = this[o]).parentNode;
+            for (var c = -1, l = r.length; ++c < l;)(u = r[c]) ? (t.push(e = n.call(u, u.__data__, c, o)), e && "__data__" in u && (e.__data__ = u.__data__)) : t.push(null)
+        }
+        return S(i)
+    }, ya.selectAll = function(n) {
+        var t, e, r = [];
+        n = E(n);
+        for (var u = -1, i = this.length; ++u < i;)
+            for (var o = this[u], a = -1, c = o.length; ++a < c;)(e = o[a]) && (r.push(t = Jo(n.call(e, e.__data__, a, u))), t.parentNode = e);
+        return S(r)
+    };
+    var xa = {
+        svg: "http://www.w3.org/2000/svg",
+        xhtml: "http://www.w3.org/1999/xhtml",
+        xlink: "http://www.w3.org/1999/xlink",
+        xml: "http://www.w3.org/XML/1998/namespace",
+        xmlns: "http://www.w3.org/2000/xmlns/"
+    };
+    Bo.ns = {
+        prefix: xa,
+        qualify: function(n) {
+            var t = n.indexOf(":"),
+                e = n;
+            return t >= 0 && (e = n.slice(0, t), n = n.slice(t + 1)), xa.hasOwnProperty(e) ? {
+                space: xa[e],
+                local: n
+            } : n
+        }
+    }, ya.attr = function(n, t) {
+        if (arguments.length < 2) {
+            if ("string" == typeof n) {
+                var e = this.node();
+                return n = Bo.ns.qualify(n), n.local ? e.getAttributeNS(n.space, n.local) : e.getAttribute(n)
+            }
+            for (t in n) this.each(A(t, n[t]));
+            return this
+        }
+        return this.each(A(n, t))
+    }, ya.classed = function(n, t) {
+        if (arguments.length < 2) {
+            if ("string" == typeof n) {
+                var e = this.node(),
+                    r = (n = z(n)).length,
+                    u = -1;
+                if (t = e.classList) {
+                    for (; ++u < r;)
+                        if (!t.contains(n[u])) return !1
+                } else
+                    for (t = e.getAttribute("class"); ++u < r;)
+                        if (!N(n[u]).test(t)) return !1;
+                return !0
+            }
+            for (t in n) this.each(L(t, n[t]));
+            return this
+        }
+        return this.each(L(n, t))
+    }, ya.style = function(n, t, e) {
+        var r = arguments.length;
+        if (3 > r) {
+            if ("string" != typeof n) {
+                2 > r && (t = "");
+                for (e in n) this.each(q(e, n[e], t));
+                return this
+            }
+            if (2 > r) return Qo.getComputedStyle(this.node(), null).getPropertyValue(n);
+            e = ""
+        }
+        return this.each(q(n, t, e))
+    }, ya.property = function(n, t) {
+        if (arguments.length < 2) {
+            if ("string" == typeof n) return this.node()[n];
+            for (t in n) this.each(R(t, n[t]));
+            return this
+        }
+        return this.each(R(n, t))
+    }, ya.text = function(n) {
+        return arguments.length ? this.each("function" == typeof n ? function() {
+            var t = n.apply(this, arguments);
+            this.textContent = null == t ? "" : t
+        } : null == n ? function() {
+            this.textContent = ""
+        } : function() {
+            this.textContent = n
+        }) : this.node().textContent
+    }, ya.html = function(n) {
+        return arguments.length ? this.each("function" == typeof n ? function() {
+            var t = n.apply(this, arguments);
+            this.innerHTML = null == t ? "" : t
+        } : null == n ? function() {
+            this.innerHTML = ""
+        } : function() {
+            this.innerHTML = n
+        }) : this.node().innerHTML
+    }, ya.append = function(n) {
+        return n = D(n), this.select(function() {
+            return this.appendChild(n.apply(this, arguments))
+        })
+    }, ya.insert = function(n, t) {
+        return n = D(n), t = k(t), this.select(function() {
+            return this.insertBefore(n.apply(this, arguments), t.apply(this, arguments) || null)
+        })
+    }, ya.remove = function() {
+        return this.each(function() {
+            var n = this.parentNode;
+            n && n.removeChild(this)
+        })
+    }, ya.data = function(n, t) {
+        function e(n, e) {
+            var r, u, i, o = n.length,
+                f = e.length,
+                h = Math.min(o, f),
+                g = new Array(f),
+                p = new Array(f),
+                v = new Array(o);
+            if (t) {
+                var d, m = new a,
+                    y = new Array(o);
+                for (r = -1; ++r < o;) m.has(d = t.call(u = n[r], u.__data__, r)) ? v[r] = u : m.set(d, u), y[r] = d;
+                for (r = -1; ++r < f;)(u = m.get(d = t.call(e, i = e[r], r))) ? u !== !0 && (g[r] = u, u.__data__ = i) : p[r] = P(i), m.set(d, !0);
+                for (r = -1; ++r < o;) m.get(y[r]) !== !0 && (v[r] = n[r])
+            } else {
+                for (r = -1; ++r < h;) u = n[r], i = e[r], u ? (u.__data__ = i, g[r] = u) : p[r] = P(i);
+                for (; f > r; ++r) p[r] = P(e[r]);
+                for (; o > r; ++r) v[r] = n[r]
+            }
+            p.update = g, p.parentNode = g.parentNode = v.parentNode = n.parentNode, c.push(p), l.push(g), s.push(v)
+        }
+        var r, u, i = -1,
+            o = this.length;
+        if (!arguments.length) {
+            for (n = new Array(o = (r = this[0]).length); ++i < o;)(u = r[i]) && (n[i] = u.__data__);
+            return n
+        }
+        var c = H([]),
+            l = S([]),
+            s = S([]);
+        if ("function" == typeof n)
+            for (; ++i < o;) e(r = this[i], n.call(r, r.parentNode.__data__, i));
+        else
+            for (; ++i < o;) e(r = this[i], n);
+        return l.enter = function() {
+            return c
+        }, l.exit = function() {
+            return s
+        }, l
+    }, ya.datum = function(n) {
+        return arguments.length ? this.property("__data__", n) : this.property("__data__")
+    }, ya.filter = function(n) {
+        var t, e, r, u = [];
+        "function" != typeof n && (n = U(n));
+        for (var i = 0, o = this.length; o > i; i++) {
+            u.push(t = []), t.parentNode = (e = this[i]).parentNode;
+            for (var a = 0, c = e.length; c > a; a++)(r = e[a]) && n.call(r, r.__data__, a, i) && t.push(r)
+        }
+        return S(u)
+    }, ya.order = function() {
+        for (var n = -1, t = this.length; ++n < t;)
+            for (var e, r = this[n], u = r.length - 1, i = r[u]; --u >= 0;)(e = r[u]) && (i && i !== e.nextSibling && i.parentNode.insertBefore(e, i), i = e);
+        return this
+    }, ya.sort = function(n) {
+        n = j.apply(this, arguments);
+        for (var t = -1, e = this.length; ++t < e;) this[t].sort(n);
+        return this.order()
+    }, ya.each = function(n) {
+        return F(this, function(t, e, r) {
+            n.call(t, t.__data__, e, r)
+        })
+    }, ya.call = function(n) {
+        var t = Jo(arguments);
+        return n.apply(t[0] = this, t), this
+    }, ya.empty = function() {
+        return !this.node()
+    }, ya.node = function() {
+        for (var n = 0, t = this.length; t > n; n++)
+            for (var e = this[n], r = 0, u = e.length; u > r; r++) {
+                var i = e[r];
+                if (i) return i
+            }
+        return null
+    }, ya.size = function() {
+        var n = 0;
+        return F(this, function() {
+            ++n
+        }), n
+    };
+    var Ma = [];
+    Bo.selection.enter = H, Bo.selection.enter.prototype = Ma, Ma.append = ya.append, Ma.empty = ya.empty, Ma.node = ya.node, Ma.call = ya.call, Ma.size = ya.size, Ma.select = function(n) {
+        for (var t, e, r, u, i, o = [], a = -1, c = this.length; ++a < c;) {
+            r = (u = this[a]).update, o.push(t = []), t.parentNode = u.parentNode;
+            for (var l = -1, s = u.length; ++l < s;)(i = u[l]) ? (t.push(r[l] = e = n.call(u.parentNode, i.__data__, l, a)), e.__data__ = i.__data__) : t.push(null)
+        }
+        return S(o)
+    }, Ma.insert = function(n, t) {
+        return arguments.length < 2 && (t = O(this)), ya.insert.call(this, n, t)
+    }, ya.transition = function() {
+        for (var n, t, e = Cl || ++ql, r = [], u = Nl || {
+                time: Date.now(),
+                ease: wu,
+                delay: 0,
+                duration: 250
+            }, i = -1, o = this.length; ++i < o;) {
+            r.push(n = []);
+            for (var a = this[i], c = -1, l = a.length; ++c < l;)(t = a[c]) && Ho(t, c, e, u), n.push(t)
+        }
+        return Uo(r, e)
+    }, ya.interrupt = function() {
+        return this.each(Y)
+    }, Bo.select = function(n) {
+        var t = ["string" == typeof n ? pa(n, Go) : n];
+        return t.parentNode = Ko, S([t])
+    }, Bo.selectAll = function(n) {
+        var t = Jo("string" == typeof n ? va(n, Go) : n);
+        return t.parentNode = Ko, S([t])
+    };
+    var _a = Bo.select(Ko);
+    ya.on = function(n, t, e) {
+        var r = arguments.length;
+        if (3 > r) {
+            if ("string" != typeof n) {
+                2 > r && (t = !1);
+                for (e in n) this.each(I(e, n[e], t));
+                return this
+            }
+            if (2 > r) return (r = this.node()["__on" + n]) && r._;
+            e = !1
+        }
+        return this.each(I(n, t, e))
+    };
+    var ba = Bo.map({
+        mouseenter: "mouseover",
+        mouseleave: "mouseout"
+    });
+    ba.forEach(function(n) {
+        "on" + n in Go && ba.remove(n)
+    });
+    var wa = "onselectstart" in Go ? null : m(Ko.style, "userSelect"),
+        Sa = 0;
+    Bo.mouse = function(n) {
+        return $(n, b())
+    };
+    var ka = /WebKit/.test(Qo.navigator.userAgent) ? -1 : 0;
+    Bo.touch = function(n, t, e) {
+        if (arguments.length < 3 && (e = t, t = b().changedTouches), t)
+            for (var r, u = 0, i = t.length; i > u; ++u)
+                if ((r = t[u]).identifier === e) return $(n, r)
+    }, Bo.behavior.drag = function() {
+        function n() {
+            this.on("mousedown.drag", u).on("touchstart.drag", i)
+        }
+
+        function t(n, t, u, i, o) {
+            return function() {
+                function a() {
+                    var n, e, r = t(h, v);
+                    r && (n = r[0] - x[0], e = r[1] - x[1], p |= n | e, x = r, g({
+                        type: "drag",
+                        x: r[0] + l[0],
+                        y: r[1] + l[1],
+                        dx: n,
+                        dy: e
                     }))
                 }
 
-                function Ca(n) {
-                    return null == n && (n = ""),
-                        function() {
-                            this.textContent = n
-                        }
+                function c() {
+                    t(h, v) && (m.on(i + d, null).on(o + d, null), y(p && Bo.event.target === f), g({
+                        type: "dragend"
+                    }))
                 }
+                var l, s = this,
+                    f = Bo.event.target,
+                    h = s.parentNode,
+                    g = e.of(s, arguments),
+                    p = 0,
+                    v = n(),
+                    d = ".drag" + (null == v ? "" : "-" + v),
+                    m = Bo.select(u()).on(i + d, a).on(o + d, c),
+                    y = X(),
+                    x = t(h, v);
+                r ? (l = r.apply(s, arguments), l = [l.x - x[0], l.y - x[1]]) : l = [0, 0], g({
+                    type: "dragstart"
+                })
+            }
+        }
+        var e = w(n, "drag", "dragstart", "dragend"),
+            r = null,
+            u = t(y, Bo.mouse, J, "mousemove", "mouseup"),
+            i = t(B, Bo.touch, W, "touchmove", "touchend");
+        return n.origin = function(t) {
+            return arguments.length ? (r = t, n) : r
+        }, Bo.rebind(n, e, "on")
+    }, Bo.touches = function(n, t) {
+        return arguments.length < 2 && (t = b().touches), t ? Jo(t).map(function(t) {
+            var e = $(n, t);
+            return e.identifier = t.identifier, e
+        }) : []
+    };
+    var Ea = Math.PI,
+        Aa = 2 * Ea,
+        Ca = Ea / 2,
+        Na = 1e-6,
+        za = Na * Na,
+        La = Ea / 180,
+        Ta = 180 / Ea,
+        qa = Math.SQRT2,
+        Ra = 2,
+        Da = 4;
+    Bo.interpolateZoom = function(n, t) {
+        function e(n) {
+            var t = n * y;
+            if (m) {
+                var e = et(v),
+                    o = i / (Ra * h) * (e * rt(qa * t + v) - tt(v));
+                return [r + o * l, u + o * s, i * e / et(qa * t + v)]
+            }
+            return [r + n * l, u + n * s, i * Math.exp(qa * t)]
+        }
+        var r = n[0],
+            u = n[1],
+            i = n[2],
+            o = t[0],
+            a = t[1],
+            c = t[2],
+            l = o - r,
+            s = a - u,
+            f = l * l + s * s,
+            h = Math.sqrt(f),
+            g = (c * c - i * i + Da * f) / (2 * i * Ra * h),
+            p = (c * c - i * i - Da * f) / (2 * c * Ra * h),
+            v = Math.log(Math.sqrt(g * g + 1) - g),
+            d = Math.log(Math.sqrt(p * p + 1) - p),
+            m = d - v,
+            y = (m || Math.log(c / i)) / qa;
+        return e.duration = 1e3 * y, e
+    }, Bo.behavior.zoom = function() {
+        function n(n) {
+            n.on(A, l).on(ja + ".zoom", f).on("dblclick.zoom", h).on(z, s)
+        }
 
-                function za(n) {
-                    return null == n ? "__transition__" : "__transition_" + n + "__"
-                }
+        function t(n) {
+            return [(n[0] - S.x) / S.k, (n[1] - S.y) / S.k]
+        }
 
-                function La(n, t, e, r, i) {
-                    var u, o, a, l, c, f = n[e] || (n[e] = {
-                            active: 0,
-                            count: 0
-                        }),
-                        s = f[r];
-
-                    function h(e) {
-                        var i = f.active,
-                            h = f[i];
-                        for (var g in h && (h.timer.c = null, h.timer.t = NaN, --f.count, delete f[i], h.event && h.event.interrupt.call(n, n.__data__, h.index)), f)
-                            if (+g < r) {
-                                var v = f[g];
-                                v.timer.c = null, v.timer.t = NaN, --f.count, delete f[g]
-                            } o.c = p, Et((function() {
-                            return o.c && p(e || 1) && (o.c = null, o.t = NaN), 1
-                        }), 0, u), f.active = r, s.event && s.event.start.call(n, n.__data__, t), c = [], s.tween.forEach((function(e, r) {
-                            (r = r.call(n, n.__data__, t)) && c.push(r)
-                        })), l = s.ease, a = s.duration
-                    }
+        function e(n) {
+            return [n[0] * S.k + S.x, n[1] * S.k + S.y]
+        }
 
-                    function p(i) {
-                        for (var u = i / a, o = l(u), h = c.length; h > 0;) c[--h].call(n, o);
-                        if (u >= 1) return s.event && s.event.end.call(n, n.__data__, t), --f.count ? delete f[r] : delete n[e], 1
-                    }
-                    s || (u = i.time, o = Et((function(n) {
-                        var t = s.delay;
-                        if (o.t = t + u, t <= n) return h(n - t);
-                        o.c = h
-                    }), 0, u), s = f[r] = {
-                        tween: new S,
-                        time: u,
-                        timer: o,
-                        delay: i.delay,
-                        duration: i.duration,
-                        ease: i.ease,
-                        index: t
-                    }, i = null, ++f.count)
-                }
-                Na.call = W.call, Na.empty = W.empty, Na.node = W.node, Na.size = W.size, u.transition = function(n, t) {
-                    return n && n.transition ? ka ? n.transition(t) : n : u.selection().transition(n)
-                }, u.transition.prototype = Na, Na.select = function(n) {
-                    var t, e, r, i = this.id,
-                        u = this.namespace,
-                        o = [];
-                    n = G(n);
-                    for (var a = -1, l = this.length; ++a < l;) {
-                        o.push(t = []);
-                        for (var c = this[a], f = -1, s = c.length; ++f < s;)(r = c[f]) && (e = n.call(r, r.__data__, f, a)) ? ("__data__" in r && (e.__data__ = r.__data__), La(e, f, u, i, r[u][i]), t.push(e)) : t.push(null)
-                    }
-                    return _a(o, u, i)
-                }, Na.selectAll = function(n) {
-                    var t, e, r, i, u, o = this.id,
-                        a = this.namespace,
-                        l = [];
-                    n = K(n);
-                    for (var c = -1, f = this.length; ++c < f;)
-                        for (var s = this[c], h = -1, p = s.length; ++h < p;)
-                            if (r = s[h]) {
-                                u = r[a][o], e = n.call(r, r.__data__, h, c), l.push(t = []);
-                                for (var g = -1, v = e.length; ++g < v;)(i = e[g]) && La(i, g, a, o, u), t.push(i)
-                            } return _a(l, a, o)
-                }, Na.filter = function(n) {
-                    var t, e, r = [];
-                    "function" != typeof n && (n = pn(n));
-                    for (var i = 0, u = this.length; i < u; i++) {
-                        r.push(t = []);
-                        for (var o, a = 0, l = (o = this[i]).length; a < l; a++)(e = o[a]) && n.call(e, e.__data__, a, i) && t.push(e)
-                    }
-                    return _a(r, this.namespace, this.id)
-                }, Na.tween = function(n, t) {
-                    var e = this.id,
-                        r = this.namespace;
-                    return arguments.length < 2 ? this.node()[r][e].tween.get(n) : vn(this, null == t ? function(t) {
-                        t[r][e].tween.remove(n)
-                    } : function(i) {
-                        i[r][e].tween.set(n, t)
-                    })
-                }, Na.attr = function(n, t) {
-                    if (arguments.length < 2) {
-                        for (t in n) this.attr(t, n[t]);
-                        return this
-                    }
-                    var e = "transform" == n ? ku : ru,
-                        r = u.ns.qualify(n);
+        function r(n) {
+            S.k = Math.max(E[0], Math.min(E[1], n))
+        }
 
-                    function i() {
-                        this.removeAttribute(r)
-                    }
+        function u(n, t) {
+            t = e(t), S.x += n[0] - t[0], S.y += n[1] - t[1]
+        }
 
-                    function o() {
-                        this.removeAttributeNS(r.space, r.local)
-                    }
+        function i() {
+            x && x.domain(y.range().map(function(n) {
+                return (n - S.x) / S.k
+            }).map(y.invert)), b && b.domain(M.range().map(function(n) {
+                return (n - S.y) / S.k
+            }).map(M.invert))
+        }
 
-                    function a(n) {
-                        return null == n ? i : (n += "", function() {
-                            var t, i = this.getAttribute(r);
-                            return i !== n && (t = e(i, n), function(n) {
-                                this.setAttribute(r, t(n))
-                            })
-                        })
-                    }
+        function o(n) {
+            n({
+                type: "zoomstart"
+            })
+        }
 
-                    function l(n) {
-                        return null == n ? o : (n += "", function() {
-                            var t, i = this.getAttributeNS(r.space, r.local);
-                            return i !== n && (t = e(i, n), function(n) {
-                                this.setAttributeNS(r.space, r.local, t(n))
-                            })
-                        })
-                    }
-                    return Aa(this, "attr." + n, t, r.local ? l : a)
-                }, Na.attrTween = function(n, t) {
-                    var e = u.ns.qualify(n);
-                    return this.tween("attr." + n, e.local ? function(n, r) {
-                        var i = t.call(this, n, r, this.getAttributeNS(e.space, e.local));
-                        return i && function(n) {
-                            this.setAttributeNS(e.space, e.local, i(n))
-                        }
-                    } : function(n, r) {
-                        var i = t.call(this, n, r, this.getAttribute(e));
-                        return i && function(n) {
-                            this.setAttribute(e, i(n))
-                        }
+        function a(n) {
+            i(), n({
+                type: "zoom",
+                scale: S.k,
+                translate: [S.x, S.y]
+            })
+        }
+
+        function c(n) {
+            n({
+                type: "zoomend"
+            })
+        }
+
+        function l() {
+            function n() {
+                s = 1, u(Bo.mouse(r), h), a(l)
+            }
+
+            function e() {
+                f.on(C, null).on(N, null), g(s && Bo.event.target === i), c(l)
+            }
+            var r = this,
+                i = Bo.event.target,
+                l = L.of(r, arguments),
+                s = 0,
+                f = Bo.select(Qo).on(C, n).on(N, e),
+                h = t(Bo.mouse(r)),
+                g = X();
+            Y.call(r), o(l)
+        }
+
+        function s() {
+            function n() {
+                var n = Bo.touches(g);
+                return h = S.k, n.forEach(function(n) {
+                    n.identifier in v && (v[n.identifier] = t(n))
+                }), n
+            }
+
+            function e() {
+                var t = Bo.event.target;
+                Bo.select(t).on(x, i).on(M, f), b.push(t);
+                for (var e = Bo.event.changedTouches, o = 0, c = e.length; c > o; ++o) v[e[o].identifier] = null;
+                var l = n(),
+                    s = Date.now();
+                if (1 === l.length) {
+                    if (500 > s - m) {
+                        var h = l[0],
+                            g = v[h.identifier];
+                        r(2 * S.k), u(h, g), _(), a(p)
+                    }
+                    m = s
+                } else if (l.length > 1) {
+                    var h = l[0],
+                        y = l[1],
+                        w = h[0] - y[0],
+                        k = h[1] - y[1];
+                    d = w * w + k * k
+                }
+            }
+
+            function i() {
+                for (var n, t, e, i, o = Bo.touches(g), c = 0, l = o.length; l > c; ++c, i = null)
+                    if (e = o[c], i = v[e.identifier]) {
+                        if (t) break;
+                        n = e, t = i
+                    } if (i) {
+                    var s = (s = e[0] - n[0]) * s + (s = e[1] - n[1]) * s,
+                        f = d && Math.sqrt(s / d);
+                    n = [(n[0] + e[0]) / 2, (n[1] + e[1]) / 2], t = [(t[0] + i[0]) / 2, (t[1] + i[1]) / 2], r(f * h)
+                }
+                m = null, u(n, t), a(p)
+            }
+
+            function f() {
+                if (Bo.event.touches.length) {
+                    for (var t = Bo.event.changedTouches, e = 0, r = t.length; r > e; ++e) delete v[t[e].identifier];
+                    for (var u in v) return void n()
+                }
+                Bo.selectAll(b).on(y, null), w.on(A, l).on(z, s), k(), c(p)
+            }
+            var h, g = this,
+                p = L.of(g, arguments),
+                v = {},
+                d = 0,
+                y = ".zoom-" + Bo.event.changedTouches[0].identifier,
+                x = "touchmove" + y,
+                M = "touchend" + y,
+                b = [],
+                w = Bo.select(g),
+                k = X();
+            Y.call(g), e(), o(p), w.on(A, null).on(z, e)
+        }
+
+        function f() {
+            var n = L.of(this, arguments);
+            d ? clearTimeout(d) : (g = t(p = v || Bo.mouse(this)), Y.call(this), o(n)), d = setTimeout(function() {
+                d = null, c(n)
+            }, 50), _(), r(Math.pow(2, .002 * Pa()) * S.k), u(p, g), a(n)
+        }
+
+        function h() {
+            var n = L.of(this, arguments),
+                e = Bo.mouse(this),
+                i = t(e),
+                l = Math.log(S.k) / Math.LN2;
+            o(n), r(Math.pow(2, Bo.event.shiftKey ? Math.ceil(l) - 1 : Math.floor(l) + 1)), u(e, i), a(n), c(n)
+        }
+        var g, p, v, d, m, y, x, M, b, S = {
+                x: 0,
+                y: 0,
+                k: 1
+            },
+            k = [960, 500],
+            E = Ua,
+            A = "mousedown.zoom",
+            C = "mousemove.zoom",
+            N = "mouseup.zoom",
+            z = "touchstart.zoom",
+            L = w(n, "zoomstart", "zoom", "zoomend");
+        return n.event = function(n) {
+            n.each(function() {
+                var n = L.of(this, arguments),
+                    t = S;
+                Cl ? Bo.select(this).transition().each("start.zoom", function() {
+                    S = this.__chart__ || {
+                        x: 0,
+                        y: 0,
+                        k: 1
+                    }, o(n)
+                }).tween("zoom:zoom", function() {
+                    var e = k[0],
+                        r = k[1],
+                        u = e / 2,
+                        i = r / 2,
+                        o = Bo.interpolateZoom([(u - S.x) / S.k, (i - S.y) / S.k, e / S.k], [(u - t.x) / t.k, (i - t.y) / t.k, e / t.k]);
+                    return function(t) {
+                        var r = o(t),
+                            c = e / r[2];
+                        this.__chart__ = S = {
+                            x: u - r[0] * c,
+                            y: i - r[1] * c,
+                            k: c
+                        }, a(n)
+                    }
+                }).each("end.zoom", function() {
+                    c(n)
+                }) : (this.__chart__ = S, o(n), a(n), c(n))
+            })
+        }, n.translate = function(t) {
+            return arguments.length ? (S = {
+                x: +t[0],
+                y: +t[1],
+                k: S.k
+            }, i(), n) : [S.x, S.y]
+        }, n.scale = function(t) {
+            return arguments.length ? (S = {
+                x: S.x,
+                y: S.y,
+                k: +t
+            }, i(), n) : S.k
+        }, n.scaleExtent = function(t) {
+            return arguments.length ? (E = null == t ? Ua : [+t[0], +t[1]], n) : E
+        }, n.center = function(t) {
+            return arguments.length ? (v = t && [+t[0], +t[1]], n) : v
+        }, n.size = function(t) {
+            return arguments.length ? (k = t && [+t[0], +t[1]], n) : k
+        }, n.x = function(t) {
+            return arguments.length ? (x = t, y = t.copy(), S = {
+                x: 0,
+                y: 0,
+                k: 1
+            }, n) : x
+        }, n.y = function(t) {
+            return arguments.length ? (b = t, M = t.copy(), S = {
+                x: 0,
+                y: 0,
+                k: 1
+            }, n) : b
+        }, Bo.rebind(n, L, "on")
+    };
+    var Pa, Ua = [0, 1 / 0],
+        ja = "onwheel" in Go ? (Pa = function() {
+            return -Bo.event.deltaY * (Bo.event.deltaMode ? 120 : 1)
+        }, "wheel") : "onmousewheel" in Go ? (Pa = function() {
+            return Bo.event.wheelDelta
+        }, "mousewheel") : (Pa = function() {
+            return -Bo.event.detail
+        }, "MozMousePixelScroll");
+    Bo.color = it, it.prototype.toString = function() {
+        return this.rgb() + ""
+    }, Bo.hsl = ot;
+    var Fa = ot.prototype = new it;
+    Fa.brighter = function(n) {
+        return n = Math.pow(.7, arguments.length ? n : 1), new ot(this.h, this.s, this.l / n)
+    }, Fa.darker = function(n) {
+        return n = Math.pow(.7, arguments.length ? n : 1), new ot(this.h, this.s, n * this.l)
+    }, Fa.rgb = function() {
+        return at(this.h, this.s, this.l)
+    }, Bo.hcl = ct;
+    var Ha = ct.prototype = new it;
+    Ha.brighter = function(n) {
+        return new ct(this.h, this.c, Math.min(100, this.l + Oa * (arguments.length ? n : 1)))
+    }, Ha.darker = function(n) {
+        return new ct(this.h, this.c, Math.max(0, this.l - Oa * (arguments.length ? n : 1)))
+    }, Ha.rgb = function() {
+        return lt(this.h, this.c, this.l).rgb()
+    }, Bo.lab = st;
+    var Oa = 18,
+        Ya = .95047,
+        Ia = 1,
+        Za = 1.08883,
+        Va = st.prototype = new it;
+    Va.brighter = function(n) {
+        return new st(Math.min(100, this.l + Oa * (arguments.length ? n : 1)), this.a, this.b)
+    }, Va.darker = function(n) {
+        return new st(Math.max(0, this.l - Oa * (arguments.length ? n : 1)), this.a, this.b)
+    }, Va.rgb = function() {
+        return ft(this.l, this.a, this.b)
+    }, Bo.rgb = dt;
+    var Xa = dt.prototype = new it;
+    Xa.brighter = function(n) {
+        n = Math.pow(.7, arguments.length ? n : 1);
+        var t = this.r,
+            e = this.g,
+            r = this.b,
+            u = 30;
+        return t || e || r ? (t && u > t && (t = u), e && u > e && (e = u), r && u > r && (r = u), new dt(Math.min(255, t / n), Math.min(255, e / n), Math.min(255, r / n))) : new dt(u, u, u)
+    }, Xa.darker = function(n) {
+        return n = Math.pow(.7, arguments.length ? n : 1), new dt(n * this.r, n * this.g, n * this.b)
+    }, Xa.hsl = function() {
+        return _t(this.r, this.g, this.b)
+    }, Xa.toString = function() {
+        return "#" + xt(this.r) + xt(this.g) + xt(this.b)
+    };
+    var $a = Bo.map({
+        aliceblue: 15792383,
+        antiquewhite: 16444375,
+        aqua: 65535,
+        aquamarine: 8388564,
+        azure: 15794175,
+        beige: 16119260,
+        bisque: 16770244,
+        black: 0,
+        blanchedalmond: 16772045,
+        blue: 255,
+        blueviolet: 9055202,
+        brown: 10824234,
+        burlywood: 14596231,
+        cadetblue: 6266528,
+        chartreuse: 8388352,
+        chocolate: 13789470,
+        coral: 16744272,
+        cornflowerblue: 6591981,
+        cornsilk: 16775388,
+        crimson: 14423100,
+        cyan: 65535,
+        darkblue: 139,
+        darkcyan: 35723,
+        darkgoldenrod: 12092939,
+        darkgray: 11119017,
+        darkgreen: 25600,
+        darkgrey: 11119017,
+        darkkhaki: 12433259,
+        darkmagenta: 9109643,
+        darkolivegreen: 5597999,
+        darkorange: 16747520,
+        darkorchid: 10040012,
+        darkred: 9109504,
+        darksalmon: 15308410,
+        darkseagreen: 9419919,
+        darkslateblue: 4734347,
+        darkslategray: 3100495,
+        darkslategrey: 3100495,
+        darkturquoise: 52945,
+        darkviolet: 9699539,
+        deeppink: 16716947,
+        deepskyblue: 49151,
+        dimgray: 6908265,
+        dimgrey: 6908265,
+        dodgerblue: 2003199,
+        firebrick: 11674146,
+        floralwhite: 16775920,
+        forestgreen: 2263842,
+        fuchsia: 16711935,
+        gainsboro: 14474460,
+        ghostwhite: 16316671,
+        gold: 16766720,
+        goldenrod: 14329120,
+        gray: 8421504,
+        green: 32768,
+        greenyellow: 11403055,
+        grey: 8421504,
+        honeydew: 15794160,
+        hotpink: 16738740,
+        indianred: 13458524,
+        indigo: 4915330,
+        ivory: 16777200,
+        khaki: 15787660,
+        lavender: 15132410,
+        lavenderblush: 16773365,
+        lawngreen: 8190976,
+        lemonchiffon: 16775885,
+        lightblue: 11393254,
+        lightcoral: 15761536,
+        lightcyan: 14745599,
+        lightgoldenrodyellow: 16448210,
+        lightgray: 13882323,
+        lightgreen: 9498256,
+        lightgrey: 13882323,
+        lightpink: 16758465,
+        lightsalmon: 16752762,
+        lightseagreen: 2142890,
+        lightskyblue: 8900346,
+        lightslategray: 7833753,
+        lightslategrey: 7833753,
+        lightsteelblue: 11584734,
+        lightyellow: 16777184,
+        lime: 65280,
+        limegreen: 3329330,
+        linen: 16445670,
+        magenta: 16711935,
+        maroon: 8388608,
+        mediumaquamarine: 6737322,
+        mediumblue: 205,
+        mediumorchid: 12211667,
+        mediumpurple: 9662683,
+        mediumseagreen: 3978097,
+        mediumslateblue: 8087790,
+        mediumspringgreen: 64154,
+        mediumturquoise: 4772300,
+        mediumvioletred: 13047173,
+        midnightblue: 1644912,
+        mintcream: 16121850,
+        mistyrose: 16770273,
+        moccasin: 16770229,
+        navajowhite: 16768685,
+        navy: 128,
+        oldlace: 16643558,
+        olive: 8421376,
+        olivedrab: 7048739,
+        orange: 16753920,
+        orangered: 16729344,
+        orchid: 14315734,
+        palegoldenrod: 15657130,
+        palegreen: 10025880,
+        paleturquoise: 11529966,
+        palevioletred: 14381203,
+        papayawhip: 16773077,
+        peachpuff: 16767673,
+        peru: 13468991,
+        pink: 16761035,
+        plum: 14524637,
+        powderblue: 11591910,
+        purple: 8388736,
+        red: 16711680,
+        rosybrown: 12357519,
+        royalblue: 4286945,
+        saddlebrown: 9127187,
+        salmon: 16416882,
+        sandybrown: 16032864,
+        seagreen: 3050327,
+        seashell: 16774638,
+        sienna: 10506797,
+        silver: 12632256,
+        skyblue: 8900331,
+        slateblue: 6970061,
+        slategray: 7372944,
+        slategrey: 7372944,
+        snow: 16775930,
+        springgreen: 65407,
+        steelblue: 4620980,
+        tan: 13808780,
+        teal: 32896,
+        thistle: 14204888,
+        tomato: 16737095,
+        turquoise: 4251856,
+        violet: 15631086,
+        wheat: 16113331,
+        white: 16777215,
+        whitesmoke: 16119285,
+        yellow: 16776960,
+        yellowgreen: 10145074
+    });
+    $a.forEach(function(n, t) {
+        $a.set(n, mt(t))
+    }), Bo.functor = kt, Bo.xhr = At(Et), Bo.dsv = function(n, t) {
+        function e(n, e, i) {
+            arguments.length < 3 && (i = e, e = null);
+            var o = Ct(n, t, null == e ? r : u(e), i);
+            return o.row = function(n) {
+                return arguments.length ? o.response(null == (e = n) ? r : u(n)) : e
+            }, o
+        }
+
+        function r(n) {
+            return e.parse(n.responseText)
+        }
+
+        function u(n) {
+            return function(t) {
+                return e.parse(t.responseText, n)
+            }
+        }
+
+        function i(t) {
+            return t.map(o).join(n)
+        }
+
+        function o(n) {
+            return a.test(n) ? '"' + n.replace(/\"/g, '""') + '"' : n
+        }
+        var a = new RegExp('["' + n + "\n]"),
+            c = n.charCodeAt(0);
+        return e.parse = function(n, t) {
+            var r;
+            return e.parseRows(n, function(n, e) {
+                if (r) return r(n, e - 1);
+                var u = new Function("d", "return {" + n.map(function(n, t) {
+                    return JSON.stringify(n) + ": d[" + t + "]"
+                }).join(",") + "}");
+                r = t ? function(n, e) {
+                    return t(u(n), e)
+                } : u
+            })
+        }, e.parseRows = function(n, t) {
+            function e() {
+                if (s >= l) return o;
+                if (u) return u = !1, i;
+                var t = s;
+                if (34 === n.charCodeAt(t)) {
+                    for (var e = t; e++ < l;)
+                        if (34 === n.charCodeAt(e)) {
+                            if (34 !== n.charCodeAt(e + 1)) break;
+                            ++e
+                        } s = e + 2;
+                    var r = n.charCodeAt(e + 1);
+                    return 13 === r ? (u = !0, 10 === n.charCodeAt(e + 2) && ++s) : 10 === r && (u = !0), n.slice(t + 1, e).replace(/""/g, '"')
+                }
+                for (; l > s;) {
+                    var r = n.charCodeAt(s++),
+                        a = 1;
+                    if (10 === r) u = !0;
+                    else if (13 === r) u = !0, 10 === n.charCodeAt(s) && (++s, ++a);
+                    else if (r !== c) continue;
+                    return n.slice(t, s - a)
+                }
+                return n.slice(t)
+            }
+            for (var r, u, i = {}, o = {}, a = [], l = n.length, s = 0, f = 0;
+                (r = e()) !== o;) {
+                for (var h = []; r !== i && r !== o;) h.push(r), r = e();
+                t && null == (h = t(h, f++)) || a.push(h)
+            }
+            return a
+        }, e.format = function(t) {
+            if (Array.isArray(t[0])) return e.formatRows(t);
+            var r = new v,
+                u = [];
+            return t.forEach(function(n) {
+                for (var t in n) r.has(t) || u.push(r.add(t))
+            }), [u.map(o).join(n)].concat(t.map(function(t) {
+                return u.map(function(n) {
+                    return o(t[n])
+                }).join(n)
+            })).join("\n")
+        }, e.formatRows = function(n) {
+            return n.map(i).join("\n")
+        }, e
+    }, Bo.csv = Bo.dsv(",", "text/csv"), Bo.tsv = Bo.dsv("	", "text/tab-separated-values");
+    var Ba, Wa, Ja, Ga, Ka, Qa = Qo[m(Qo, "requestAnimationFrame")] || function(n) {
+        setTimeout(n, 17)
+    };
+    Bo.timer = function(n, t, e) {
+        var r = arguments.length;
+        2 > r && (t = 0), 3 > r && (e = Date.now());
+        var u = e + t,
+            i = {
+                c: n,
+                t: u,
+                f: !1,
+                n: null
+            };
+        Wa ? Wa.n = i : Ba = i, Wa = i, Ja || (Ga = clearTimeout(Ga), Ja = 1, Qa(Lt))
+    }, Bo.timer.flush = function() {
+        Tt(), qt()
+    }, Bo.round = function(n, t) {
+        return t ? Math.round(n * (t = Math.pow(10, t))) / t : Math.round(n)
+    };
+    var nc = ["y", "z", "a", "f", "p", "n", "\xb5", "m", "", "k", "M", "G", "T", "P", "E", "Z", "Y"].map(Dt);
+    Bo.formatPrefix = function(n, t) {
+        var e = 0;
+        return n && (0 > n && (n *= -1), t && (n = Bo.round(n, Rt(n, t))), e = 1 + Math.floor(1e-12 + Math.log(n) / Math.LN10), e = Math.max(-24, Math.min(24, 3 * Math.floor((e - 1) / 3)))), nc[8 + e / 3]
+    };
+    var tc = /(?:([^{])?([<>=^]))?([+\- ])?([$#])?(0)?(\d+)?(,)?(\.-?\d+)?([a-z%])?/i,
+        ec = Bo.map({
+            b: function(n) {
+                return n.toString(2)
+            },
+            c: function(n) {
+                return String.fromCharCode(n)
+            },
+            o: function(n) {
+                return n.toString(8)
+            },
+            x: function(n) {
+                return n.toString(16)
+            },
+            X: function(n) {
+                return n.toString(16).toUpperCase()
+            },
+            g: function(n, t) {
+                return n.toPrecision(t)
+            },
+            e: function(n, t) {
+                return n.toExponential(t)
+            },
+            f: function(n, t) {
+                return n.toFixed(t)
+            },
+            r: function(n, t) {
+                return (n = Bo.round(n, Rt(n, t))).toFixed(Math.max(0, Math.min(20, Rt(n * (1 + 1e-15), t))))
+            }
+        }),
+        rc = Bo.time = {},
+        uc = Date;
+    jt.prototype = {
+        getDate: function() {
+            return this._.getUTCDate()
+        },
+        getDay: function() {
+            return this._.getUTCDay()
+        },
+        getFullYear: function() {
+            return this._.getUTCFullYear()
+        },
+        getHours: function() {
+            return this._.getUTCHours()
+        },
+        getMilliseconds: function() {
+            return this._.getUTCMilliseconds()
+        },
+        getMinutes: function() {
+            return this._.getUTCMinutes()
+        },
+        getMonth: function() {
+            return this._.getUTCMonth()
+        },
+        getSeconds: function() {
+            return this._.getUTCSeconds()
+        },
+        getTime: function() {
+            return this._.getTime()
+        },
+        getTimezoneOffset: function() {
+            return 0
+        },
+        valueOf: function() {
+            return this._.valueOf()
+        },
+        setDate: function() {
+            ic.setUTCDate.apply(this._, arguments)
+        },
+        setDay: function() {
+            ic.setUTCDay.apply(this._, arguments)
+        },
+        setFullYear: function() {
+            ic.setUTCFullYear.apply(this._, arguments)
+        },
+        setHours: function() {
+            ic.setUTCHours.apply(this._, arguments)
+        },
+        setMilliseconds: function() {
+            ic.setUTCMilliseconds.apply(this._, arguments)
+        },
+        setMinutes: function() {
+            ic.setUTCMinutes.apply(this._, arguments)
+        },
+        setMonth: function() {
+            ic.setUTCMonth.apply(this._, arguments)
+        },
+        setSeconds: function() {
+            ic.setUTCSeconds.apply(this._, arguments)
+        },
+        setTime: function() {
+            ic.setTime.apply(this._, arguments)
+        }
+    };
+    var ic = Date.prototype;
+    rc.year = Ft(function(n) {
+        return n = rc.day(n), n.setMonth(0, 1), n
+    }, function(n, t) {
+        n.setFullYear(n.getFullYear() + t)
+    }, function(n) {
+        return n.getFullYear()
+    }), rc.years = rc.year.range, rc.years.utc = rc.year.utc.range, rc.day = Ft(function(n) {
+        var t = new uc(2e3, 0);
+        return t.setFullYear(n.getFullYear(), n.getMonth(), n.getDate()), t
+    }, function(n, t) {
+        n.setDate(n.getDate() + t)
+    }, function(n) {
+        return n.getDate() - 1
+    }), rc.days = rc.day.range, rc.days.utc = rc.day.utc.range, rc.dayOfYear = function(n) {
+        var t = rc.year(n);
+        return Math.floor((n - t - 6e4 * (n.getTimezoneOffset() - t.getTimezoneOffset())) / 864e5)
+    }, ["sunday", "monday", "tuesday", "wednesday", "thursday", "friday", "saturday"].forEach(function(n, t) {
+        t = 7 - t;
+        var e = rc[n] = Ft(function(n) {
+            return (n = rc.day(n)).setDate(n.getDate() - (n.getDay() + t) % 7), n
+        }, function(n, t) {
+            n.setDate(n.getDate() + 7 * Math.floor(t))
+        }, function(n) {
+            var e = rc.year(n).getDay();
+            return Math.floor((rc.dayOfYear(n) + (e + t) % 7) / 7) - (e !== t)
+        });
+        rc[n + "s"] = e.range, rc[n + "s"].utc = e.utc.range, rc[n + "OfYear"] = function(n) {
+            var e = rc.year(n).getDay();
+            return Math.floor((rc.dayOfYear(n) + (e + t) % 7) / 7)
+        }
+    }), rc.week = rc.sunday, rc.weeks = rc.sunday.range, rc.weeks.utc = rc.sunday.utc.range, rc.weekOfYear = rc.sundayOfYear;
+    var oc = {
+            "-": "",
+            _: " ",
+            0: "0"
+        },
+        ac = /^\s*\d+/,
+        cc = /^%/;
+    Bo.locale = function(n) {
+        return {
+            numberFormat: Pt(n),
+            timeFormat: Ot(n)
+        }
+    };
+    var lc = Bo.locale({
+        decimal: ".",
+        thousands: ",",
+        grouping: [3],
+        currency: ["$", ""],
+        dateTime: "%a %b %e %X %Y",
+        date: "%m/%d/%Y",
+        time: "%H:%M:%S",
+        periods: ["AM", "PM"],
+        days: ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"],
+        shortDays: ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
+        months: ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"],
+        shortMonths: ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"]
+    });
+    Bo.format = lc.numberFormat, Bo.geo = {}, ce.prototype = {
+        s: 0,
+        t: 0,
+        add: function(n) {
+            le(n, this.t, sc), le(sc.s, this.s, this), this.s ? this.t += sc.t : this.s = sc.t
+        },
+        reset: function() {
+            this.s = this.t = 0
+        },
+        valueOf: function() {
+            return this.s
+        }
+    };
+    var sc = new ce;
+    Bo.geo.stream = function(n, t) {
+        n && fc.hasOwnProperty(n.type) ? fc[n.type](n, t) : se(n, t)
+    };
+    var fc = {
+            Feature: function(n, t) {
+                se(n.geometry, t)
+            },
+            FeatureCollection: function(n, t) {
+                for (var e = n.features, r = -1, u = e.length; ++r < u;) se(e[r].geometry, t)
+            }
+        },
+        hc = {
+            Sphere: function(n, t) {
+                t.sphere()
+            },
+            Point: function(n, t) {
+                n = n.coordinates, t.point(n[0], n[1], n[2])
+            },
+            MultiPoint: function(n, t) {
+                for (var e = n.coordinates, r = -1, u = e.length; ++r < u;) n = e[r], t.point(n[0], n[1], n[2])
+            },
+            LineString: function(n, t) {
+                fe(n.coordinates, t, 0)
+            },
+            MultiLineString: function(n, t) {
+                for (var e = n.coordinates, r = -1, u = e.length; ++r < u;) fe(e[r], t, 0)
+            },
+            Polygon: function(n, t) {
+                he(n.coordinates, t)
+            },
+            MultiPolygon: function(n, t) {
+                for (var e = n.coordinates, r = -1, u = e.length; ++r < u;) he(e[r], t)
+            },
+            GeometryCollection: function(n, t) {
+                for (var e = n.geometries, r = -1, u = e.length; ++r < u;) se(e[r], t)
+            }
+        };
+    Bo.geo.area = function(n) {
+        return gc = 0, Bo.geo.stream(n, vc), gc
+    };
+    var gc, pc = new ce,
+        vc = {
+            sphere: function() {
+                gc += 4 * Ea
+            },
+            point: y,
+            lineStart: y,
+            lineEnd: y,
+            polygonStart: function() {
+                pc.reset(), vc.lineStart = ge
+            },
+            polygonEnd: function() {
+                var n = 2 * pc;
+                gc += 0 > n ? 4 * Ea + n : n, vc.lineStart = vc.lineEnd = vc.point = y
+            }
+        };
+    Bo.geo.bounds = function() {
+        function n(n, t) {
+            x.push(M = [s = n, h = n]), f > t && (f = t), t > g && (g = t)
+        }
+
+        function t(t, e) {
+            var r = pe([t * La, e * La]);
+            if (m) {
+                var u = de(m, r),
+                    i = [u[1], -u[0], 0],
+                    o = de(i, u);
+                xe(o), o = Me(o);
+                var c = t - p,
+                    l = c > 0 ? 1 : -1,
+                    v = o[0] * Ta * l,
+                    d = ca(c) > 180;
+                if (d ^ (v > l * p && l * t > v)) {
+                    var y = o[1] * Ta;
+                    y > g && (g = y)
+                } else if (v = (v + 360) % 360 - 180, d ^ (v > l * p && l * t > v)) {
+                    var y = -o[1] * Ta;
+                    f > y && (f = y)
+                } else f > e && (f = e), e > g && (g = e);
+                d ? p > t ? a(s, t) > a(s, h) && (h = t) : a(t, h) > a(s, h) && (s = t) : h >= s ? (s > t && (s = t), t > h && (h = t)) : t > p ? a(s, t) > a(s, h) && (h = t) : a(t, h) > a(s, h) && (s = t)
+            } else n(t, e);
+            m = r, p = t
+        }
+
+        function e() {
+            _.point = t
+        }
+
+        function r() {
+            M[0] = s, M[1] = h, _.point = n, m = null
+        }
+
+        function u(n, e) {
+            if (m) {
+                var r = n - p;
+                y += ca(r) > 180 ? r + (r > 0 ? 360 : -360) : r
+            } else v = n, d = e;
+            vc.point(n, e), t(n, e)
+        }
+
+        function i() {
+            vc.lineStart()
+        }
+
+        function o() {
+            u(v, d), vc.lineEnd(), ca(y) > Na && (s = -(h = 180)), M[0] = s, M[1] = h, m = null
+        }
+
+        function a(n, t) {
+            return (t -= n) < 0 ? t + 360 : t
+        }
+
+        function c(n, t) {
+            return n[0] - t[0]
+        }
+
+        function l(n, t) {
+            return t[0] <= t[1] ? t[0] <= n && n <= t[1] : n < t[0] || t[1] < n
+        }
+        var s, f, h, g, p, v, d, m, y, x, M, _ = {
+            point: n,
+            lineStart: e,
+            lineEnd: r,
+            polygonStart: function() {
+                _.point = u, _.lineStart = i, _.lineEnd = o, y = 0, vc.polygonStart()
+            },
+            polygonEnd: function() {
+                vc.polygonEnd(), _.point = n, _.lineStart = e, _.lineEnd = r, 0 > pc ? (s = -(h = 180), f = -(g = 90)) : y > Na ? g = 90 : -Na > y && (f = -90), M[0] = s, M[1] = h
+            }
+        };
+        return function(n) {
+            g = h = -(s = f = 1 / 0), x = [], Bo.geo.stream(n, _);
+            var t = x.length;
+            if (t) {
+                x.sort(c);
+                for (var e, r = 1, u = x[0], i = [u]; t > r; ++r) e = x[r], l(e[0], u) || l(e[1], u) ? (a(u[0], e[1]) > a(u[0], u[1]) && (u[1] = e[1]), a(e[0], u[1]) > a(u[0], u[1]) && (u[0] = e[0])) : i.push(u = e);
+                for (var o, e, p = -1 / 0, t = i.length - 1, r = 0, u = i[t]; t >= r; u = e, ++r) e = i[r], (o = a(u[1], e[0])) > p && (p = o, s = e[0], h = u[1])
+            }
+            return x = M = null, 1 / 0 === s || 1 / 0 === f ? [
+                [0 / 0, 0 / 0],
+                [0 / 0, 0 / 0]
+            ] : [
+                [s, f],
+                [h, g]
+            ]
+        }
+    }(), Bo.geo.centroid = function(n) {
+        dc = mc = yc = xc = Mc = _c = bc = wc = Sc = kc = Ec = 0, Bo.geo.stream(n, Ac);
+        var t = Sc,
+            e = kc,
+            r = Ec,
+            u = t * t + e * e + r * r;
+        return za > u && (t = _c, e = bc, r = wc, Na > mc && (t = yc, e = xc, r = Mc), u = t * t + e * e + r * r, za > u) ? [0 / 0, 0 / 0] : [Math.atan2(e, t) * Ta, nt(r / Math.sqrt(u)) * Ta]
+    };
+    var dc, mc, yc, xc, Mc, _c, bc, wc, Sc, kc, Ec, Ac = {
+            sphere: y,
+            point: be,
+            lineStart: Se,
+            lineEnd: ke,
+            polygonStart: function() {
+                Ac.lineStart = Ee
+            },
+            polygonEnd: function() {
+                Ac.lineStart = Se
+            }
+        },
+        Cc = Le(Ae, De, Ue, [-Ea, -Ea / 2]),
+        Nc = 1e9;
+    Bo.geo.clipExtent = function() {
+        var n, t, e, r, u, i, o = {
+            stream: function(n) {
+                return u && (u.valid = !1), u = i(n), u.valid = !0, u
+            },
+            extent: function(a) {
+                return arguments.length ? (i = Oe(n = +a[0][0], t = +a[0][1], e = +a[1][0], r = +a[1][1]), u && (u.valid = !1, u = null), o) : [
+                    [n, t],
+                    [e, r]
+                ]
+            }
+        };
+        return o.extent([
+            [0, 0],
+            [960, 500]
+        ])
+    }, (Bo.geo.conicEqualArea = function() {
+        return Ie(Ze)
+    }).raw = Ze, Bo.geo.albers = function() {
+        return Bo.geo.conicEqualArea().rotate([96, 0]).center([-.6, 38.7]).parallels([29.5, 45.5]).scale(1070)
+    }, Bo.geo.albersUsa = function() {
+        function n(n) {
+            var i = n[0],
+                o = n[1];
+            return t = null, e(i, o), t || (r(i, o), t) || u(i, o), t
+        }
+        var t, e, r, u, i = Bo.geo.albers(),
+            o = Bo.geo.conicEqualArea().rotate([154, 0]).center([-2, 58.5]).parallels([55, 65]),
+            a = Bo.geo.conicEqualArea().rotate([157, 0]).center([-3, 19.9]).parallels([8, 18]),
+            c = {
+                point: function(n, e) {
+                    t = [n, e]
+                }
+            };
+        return n.invert = function(n) {
+            var t = i.scale(),
+                e = i.translate(),
+                r = (n[0] - e[0]) / t,
+                u = (n[1] - e[1]) / t;
+            return (u >= .12 && .234 > u && r >= -.425 && -.214 > r ? o : u >= .166 && .234 > u && r >= -.214 && -.115 > r ? a : i).invert(n)
+        }, n.stream = function(n) {
+            var t = i.stream(n),
+                e = o.stream(n),
+                r = a.stream(n);
+            return {
+                point: function(n, u) {
+                    t.point(n, u), e.point(n, u), r.point(n, u)
+                },
+                sphere: function() {
+                    t.sphere(), e.sphere(), r.sphere()
+                },
+                lineStart: function() {
+                    t.lineStart(), e.lineStart(), r.lineStart()
+                },
+                lineEnd: function() {
+                    t.lineEnd(), e.lineEnd(), r.lineEnd()
+                },
+                polygonStart: function() {
+                    t.polygonStart(), e.polygonStart(), r.polygonStart()
+                },
+                polygonEnd: function() {
+                    t.polygonEnd(), e.polygonEnd(), r.polygonEnd()
+                }
+            }
+        }, n.precision = function(t) {
+            return arguments.length ? (i.precision(t), o.precision(t), a.precision(t), n) : i.precision()
+        }, n.scale = function(t) {
+            return arguments.length ? (i.scale(t), o.scale(.35 * t), a.scale(t), n.translate(i.translate())) : i.scale()
+        }, n.translate = function(t) {
+            if (!arguments.length) return i.translate();
+            var l = i.scale(),
+                s = +t[0],
+                f = +t[1];
+            return e = i.translate(t).clipExtent([
+                [s - .455 * l, f - .238 * l],
+                [s + .455 * l, f + .238 * l]
+            ]).stream(c).point, r = o.translate([s - .307 * l, f + .201 * l]).clipExtent([
+                [s - .425 * l + Na, f + .12 * l + Na],
+                [s - .214 * l - Na, f + .234 * l - Na]
+            ]).stream(c).point, u = a.translate([s - .205 * l, f + .212 * l]).clipExtent([
+                [s - .214 * l + Na, f + .166 * l + Na],
+                [s - .115 * l - Na, f + .234 * l - Na]
+            ]).stream(c).point, n
+        }, n.scale(1070)
+    };
+    var zc, Lc, Tc, qc, Rc, Dc, Pc = {
+            point: y,
+            lineStart: y,
+            lineEnd: y,
+            polygonStart: function() {
+                Lc = 0, Pc.lineStart = Ve
+            },
+            polygonEnd: function() {
+                Pc.lineStart = Pc.lineEnd = Pc.point = y, zc += ca(Lc / 2)
+            }
+        },
+        Uc = {
+            point: Xe,
+            lineStart: y,
+            lineEnd: y,
+            polygonStart: y,
+            polygonEnd: y
+        },
+        jc = {
+            point: We,
+            lineStart: Je,
+            lineEnd: Ge,
+            polygonStart: function() {
+                jc.lineStart = Ke
+            },
+            polygonEnd: function() {
+                jc.point = We, jc.lineStart = Je, jc.lineEnd = Ge
+            }
+        };
+    Bo.geo.path = function() {
+        function n(n) {
+            return n && ("function" == typeof a && i.pointRadius(+a.apply(this, arguments)), o && o.valid || (o = u(i)), Bo.geo.stream(n, o)), i.result()
+        }
+
+        function t() {
+            return o = null, n
+        }
+        var e, r, u, i, o, a = 4.5;
+        return n.area = function(n) {
+            return zc = 0, Bo.geo.stream(n, u(Pc)), zc
+        }, n.centroid = function(n) {
+            return yc = xc = Mc = _c = bc = wc = Sc = kc = Ec = 0, Bo.geo.stream(n, u(jc)), Ec ? [Sc / Ec, kc / Ec] : wc ? [_c / wc, bc / wc] : Mc ? [yc / Mc, xc / Mc] : [0 / 0, 0 / 0]
+        }, n.bounds = function(n) {
+            return Rc = Dc = -(Tc = qc = 1 / 0), Bo.geo.stream(n, u(Uc)), [
+                [Tc, qc],
+                [Rc, Dc]
+            ]
+        }, n.projection = function(n) {
+            return arguments.length ? (u = (e = n) ? n.stream || tr(n) : Et, t()) : e
+        }, n.context = function(n) {
+            return arguments.length ? (i = null == (r = n) ? new $e : new Qe(n), "function" != typeof a && i.pointRadius(a), t()) : r
+        }, n.pointRadius = function(t) {
+            return arguments.length ? (a = "function" == typeof t ? t : (i.pointRadius(+t), +t), n) : a
+        }, n.projection(Bo.geo.albersUsa()).context(null)
+    }, Bo.geo.transform = function(n) {
+        return {
+            stream: function(t) {
+                var e = new er(t);
+                for (var r in n) e[r] = n[r];
+                return e
+            }
+        }
+    }, er.prototype = {
+        point: function(n, t) {
+            this.stream.point(n, t)
+        },
+        sphere: function() {
+            this.stream.sphere()
+        },
+        lineStart: function() {
+            this.stream.lineStart()
+        },
+        lineEnd: function() {
+            this.stream.lineEnd()
+        },
+        polygonStart: function() {
+            this.stream.polygonStart()
+        },
+        polygonEnd: function() {
+            this.stream.polygonEnd()
+        }
+    }, Bo.geo.projection = ur, Bo.geo.projectionMutator = ir, (Bo.geo.equirectangular = function() {
+        return ur(ar)
+    }).raw = ar.invert = ar, Bo.geo.rotation = function(n) {
+        function t(t) {
+            return t = n(t[0] * La, t[1] * La), t[0] *= Ta, t[1] *= Ta, t
+        }
+        return n = lr(n[0] % 360 * La, n[1] * La, n.length > 2 ? n[2] * La : 0), t.invert = function(t) {
+            return t = n.invert(t[0] * La, t[1] * La), t[0] *= Ta, t[1] *= Ta, t
+        }, t
+    }, cr.invert = ar, Bo.geo.circle = function() {
+        function n() {
+            var n = "function" == typeof r ? r.apply(this, arguments) : r,
+                t = lr(-n[0] * La, -n[1] * La, 0).invert,
+                u = [];
+            return e(null, null, 1, {
+                point: function(n, e) {
+                    u.push(n = t(n, e)), n[0] *= Ta, n[1] *= Ta
+                }
+            }), {
+                type: "Polygon",
+                coordinates: [u]
+            }
+        }
+        var t, e, r = [0, 0],
+            u = 6;
+        return n.origin = function(t) {
+            return arguments.length ? (r = t, n) : r
+        }, n.angle = function(r) {
+            return arguments.length ? (e = gr((t = +r) * La, u * La), n) : t
+        }, n.precision = function(r) {
+            return arguments.length ? (e = gr(t * La, (u = +r) * La), n) : u
+        }, n.angle(90)
+    }, Bo.geo.distance = function(n, t) {
+        var e, r = (t[0] - n[0]) * La,
+            u = n[1] * La,
+            i = t[1] * La,
+            o = Math.sin(r),
+            a = Math.cos(r),
+            c = Math.sin(u),
+            l = Math.cos(u),
+            s = Math.sin(i),
+            f = Math.cos(i);
+        return Math.atan2(Math.sqrt((e = f * o) * e + (e = l * s - c * f * a) * e), c * s + l * f * a)
+    }, Bo.geo.graticule = function() {
+        function n() {
+            return {
+                type: "MultiLineString",
+                coordinates: t()
+            }
+        }
+
+        function t() {
+            return Bo.range(Math.ceil(i / d) * d, u, d).map(h).concat(Bo.range(Math.ceil(l / m) * m, c, m).map(g)).concat(Bo.range(Math.ceil(r / p) * p, e, p).filter(function(n) {
+                return ca(n % d) > Na
+            }).map(s)).concat(Bo.range(Math.ceil(a / v) * v, o, v).filter(function(n) {
+                return ca(n % m) > Na
+            }).map(f))
+        }
+        var e, r, u, i, o, a, c, l, s, f, h, g, p = 10,
+            v = p,
+            d = 90,
+            m = 360,
+            y = 2.5;
+        return n.lines = function() {
+            return t().map(function(n) {
+                return {
+                    type: "LineString",
+                    coordinates: n
+                }
+            })
+        }, n.outline = function() {
+            return {
+                type: "Polygon",
+                coordinates: [h(i).concat(g(c).slice(1), h(u).reverse().slice(1), g(l).reverse().slice(1))]
+            }
+        }, n.extent = function(t) {
+            return arguments.length ? n.majorExtent(t).minorExtent(t) : n.minorExtent()
+        }, n.majorExtent = function(t) {
+            return arguments.length ? (i = +t[0][0], u = +t[1][0], l = +t[0][1], c = +t[1][1], i > u && (t = i, i = u, u = t), l > c && (t = l, l = c, c = t), n.precision(y)) : [
+                [i, l],
+                [u, c]
+            ]
+        }, n.minorExtent = function(t) {
+            return arguments.length ? (r = +t[0][0], e = +t[1][0], a = +t[0][1], o = +t[1][1], r > e && (t = r, r = e, e = t), a > o && (t = a, a = o, o = t), n.precision(y)) : [
+                [r, a],
+                [e, o]
+            ]
+        }, n.step = function(t) {
+            return arguments.length ? n.majorStep(t).minorStep(t) : n.minorStep()
+        }, n.majorStep = function(t) {
+            return arguments.length ? (d = +t[0], m = +t[1], n) : [d, m]
+        }, n.minorStep = function(t) {
+            return arguments.length ? (p = +t[0], v = +t[1], n) : [p, v]
+        }, n.precision = function(t) {
+            return arguments.length ? (y = +t, s = vr(a, o, 90), f = dr(r, e, y), h = vr(l, c, 90), g = dr(i, u, y), n) : y
+        }, n.majorExtent([
+            [-180, -90 + Na],
+            [180, 90 - Na]
+        ]).minorExtent([
+            [-180, -80 - Na],
+            [180, 80 + Na]
+        ])
+    }, Bo.geo.greatArc = function() {
+        function n() {
+            return {
+                type: "LineString",
+                coordinates: [t || r.apply(this, arguments), e || u.apply(this, arguments)]
+            }
+        }
+        var t, e, r = mr,
+            u = yr;
+        return n.distance = function() {
+            return Bo.geo.distance(t || r.apply(this, arguments), e || u.apply(this, arguments))
+        }, n.source = function(e) {
+            return arguments.length ? (r = e, t = "function" == typeof e ? null : e, n) : r
+        }, n.target = function(t) {
+            return arguments.length ? (u = t, e = "function" == typeof t ? null : t, n) : u
+        }, n.precision = function() {
+            return arguments.length ? n : 0
+        }, n
+    }, Bo.geo.interpolate = function(n, t) {
+        return xr(n[0] * La, n[1] * La, t[0] * La, t[1] * La)
+    }, Bo.geo.length = function(n) {
+        return Fc = 0, Bo.geo.stream(n, Hc), Fc
+    };
+    var Fc, Hc = {
+            sphere: y,
+            point: y,
+            lineStart: Mr,
+            lineEnd: y,
+            polygonStart: y,
+            polygonEnd: y
+        },
+        Oc = _r(function(n) {
+            return Math.sqrt(2 / (1 + n))
+        }, function(n) {
+            return 2 * Math.asin(n / 2)
+        });
+    (Bo.geo.azimuthalEqualArea = function() {
+        return ur(Oc)
+    }).raw = Oc;
+    var Yc = _r(function(n) {
+        var t = Math.acos(n);
+        return t && t / Math.sin(t)
+    }, Et);
+    (Bo.geo.azimuthalEquidistant = function() {
+        return ur(Yc)
+    }).raw = Yc, (Bo.geo.conicConformal = function() {
+        return Ie(br)
+    }).raw = br, (Bo.geo.conicEquidistant = function() {
+        return Ie(wr)
+    }).raw = wr;
+    var Ic = _r(function(n) {
+        return 1 / n
+    }, Math.atan);
+    (Bo.geo.gnomonic = function() {
+        return ur(Ic)
+    }).raw = Ic, Sr.invert = function(n, t) {
+        return [n, 2 * Math.atan(Math.exp(t)) - Ca]
+    }, (Bo.geo.mercator = function() {
+        return kr(Sr)
+    }).raw = Sr;
+    var Zc = _r(function() {
+        return 1
+    }, Math.asin);
+    (Bo.geo.orthographic = function() {
+        return ur(Zc)
+    }).raw = Zc;
+    var Vc = _r(function(n) {
+        return 1 / (1 + n)
+    }, function(n) {
+        return 2 * Math.atan(n)
+    });
+    (Bo.geo.stereographic = function() {
+        return ur(Vc)
+    }).raw = Vc, Er.invert = function(n, t) {
+        return [-t, 2 * Math.atan(Math.exp(n)) - Ca]
+    }, (Bo.geo.transverseMercator = function() {
+        var n = kr(Er),
+            t = n.center,
+            e = n.rotate;
+        return n.center = function(n) {
+            return n ? t([-n[1], n[0]]) : (n = t(), [n[1], -n[0]])
+        }, n.rotate = function(n) {
+            return n ? e([n[0], n[1], n.length > 2 ? n[2] + 90 : 90]) : (n = e(), [n[0], n[1], n[2] - 90])
+        }, e([0, 0, 90])
+    }).raw = Er, Bo.geom = {}, Bo.geom.hull = function(n) {
+        function t(n) {
+            if (n.length < 3) return [];
+            var t, u = kt(e),
+                i = kt(r),
+                o = n.length,
+                a = [],
+                c = [];
+            for (t = 0; o > t; t++) a.push([+u.call(this, n[t], t), +i.call(this, n[t], t), t]);
+            for (a.sort(zr), t = 0; o > t; t++) c.push([a[t][0], -a[t][1]]);
+            var l = Nr(a),
+                s = Nr(c),
+                f = s[0] === l[0],
+                h = s[s.length - 1] === l[l.length - 1],
+                g = [];
+            for (t = l.length - 1; t >= 0; --t) g.push(n[a[l[t]][2]]);
+            for (t = +f; t < s.length - h; ++t) g.push(n[a[s[t]][2]]);
+            return g
+        }
+        var e = Ar,
+            r = Cr;
+        return arguments.length ? t(n) : (t.x = function(n) {
+            return arguments.length ? (e = n, t) : e
+        }, t.y = function(n) {
+            return arguments.length ? (r = n, t) : r
+        }, t)
+    }, Bo.geom.polygon = function(n) {
+        return ga(n, Xc), n
+    };
+    var Xc = Bo.geom.polygon.prototype = [];
+    Xc.area = function() {
+        for (var n, t = -1, e = this.length, r = this[e - 1], u = 0; ++t < e;) n = r, r = this[t], u += n[1] * r[0] - n[0] * r[1];
+        return .5 * u
+    }, Xc.centroid = function(n) {
+        var t, e, r = -1,
+            u = this.length,
+            i = 0,
+            o = 0,
+            a = this[u - 1];
+        for (arguments.length || (n = -1 / (6 * this.area())); ++r < u;) t = a, a = this[r], e = t[0] * a[1] - a[0] * t[1], i += (t[0] + a[0]) * e, o += (t[1] + a[1]) * e;
+        return [i * n, o * n]
+    }, Xc.clip = function(n) {
+        for (var t, e, r, u, i, o, a = qr(n), c = -1, l = this.length - qr(this), s = this[l - 1]; ++c < l;) {
+            for (t = n.slice(), n.length = 0, u = this[c], i = t[(r = t.length - a) - 1], e = -1; ++e < r;) o = t[e], Lr(o, s, u) ? (Lr(i, s, u) || n.push(Tr(i, o, s, u)), n.push(o)) : Lr(i, s, u) && n.push(Tr(i, o, s, u)), i = o;
+            a && n.push(n[0]), s = u
+        }
+        return n
+    };
+    var $c, Bc, Wc, Jc, Gc, Kc = [],
+        Qc = [];
+    Or.prototype.prepare = function() {
+        for (var n, t = this.edges, e = t.length; e--;) n = t[e].edge, n.b && n.a || t.splice(e, 1);
+        return t.sort(Ir), t.length
+    }, Qr.prototype = {
+        start: function() {
+            return this.edge.l === this.site ? this.edge.a : this.edge.b
+        },
+        end: function() {
+            return this.edge.l === this.site ? this.edge.b : this.edge.a
+        }
+    }, nu.prototype = {
+        insert: function(n, t) {
+            var e, r, u;
+            if (n) {
+                if (t.P = n, t.N = n.N, n.N && (n.N.P = t), n.N = t, n.R) {
+                    for (n = n.R; n.L;) n = n.L;
+                    n.L = t
+                } else n.R = t;
+                e = n
+            } else this._ ? (n = uu(this._), t.P = null, t.N = n, n.P = n.L = t, e = n) : (t.P = t.N = null, this._ = t, e = null);
+            for (t.L = t.R = null, t.U = e, t.C = !0, n = t; e && e.C;) r = e.U, e === r.L ? (u = r.R, u && u.C ? (e.C = u.C = !1, r.C = !0, n = r) : (n === e.R && (eu(this, e), n = e, e = n.U), e.C = !1, r.C = !0, ru(this, r))) : (u = r.L, u && u.C ? (e.C = u.C = !1, r.C = !0, n = r) : (n === e.L && (ru(this, e), n = e, e = n.U), e.C = !1, r.C = !0, eu(this, r))), e = n.U;
+            this._.C = !1
+        },
+        remove: function(n) {
+            n.N && (n.N.P = n.P), n.P && (n.P.N = n.N), n.N = n.P = null;
+            var t, e, r, u = n.U,
+                i = n.L,
+                o = n.R;
+            if (e = i ? o ? uu(o) : i : o, u ? u.L === n ? u.L = e : u.R = e : this._ = e, i && o ? (r = e.C, e.C = n.C, e.L = i, i.U = e, e !== o ? (u = e.U, e.U = n.U, n = e.R, u.L = n, e.R = o, o.U = e) : (e.U = u, u = e, n = e.R)) : (r = n.C, n = e), n && (n.U = u), !r) {
+                if (n && n.C) return n.C = !1, void 0;
+                do {
+                    if (n === this._) break;
+                    if (n === u.L) {
+                        if (t = u.R, t.C && (t.C = !1, u.C = !0, eu(this, u), t = u.R), t.L && t.L.C || t.R && t.R.C) {
+                            t.R && t.R.C || (t.L.C = !1, t.C = !0, ru(this, t), t = u.R), t.C = u.C, u.C = t.R.C = !1, eu(this, u), n = this._;
+                            break
+                        }
+                    } else if (t = u.L, t.C && (t.C = !1, u.C = !0, ru(this, u), t = u.L), t.L && t.L.C || t.R && t.R.C) {
+                        t.L && t.L.C || (t.R.C = !1, t.C = !0, eu(this, t), t = u.L), t.C = u.C, u.C = t.L.C = !1, ru(this, u), n = this._;
+                        break
+                    }
+                    t.C = !0, n = u, u = u.U
+                } while (!n.C);
+                n && (n.C = !1)
+            }
+        }
+    }, Bo.geom.voronoi = function(n) {
+        function t(n) {
+            var t = new Array(n.length),
+                r = a[0][0],
+                u = a[0][1],
+                i = a[1][0],
+                o = a[1][1];
+            return iu(e(n), a).cells.forEach(function(e, a) {
+                var c = e.edges,
+                    l = e.site,
+                    s = t[a] = c.length ? c.map(function(n) {
+                        var t = n.start();
+                        return [t.x, t.y]
+                    }) : l.x >= r && l.x <= i && l.y >= u && l.y <= o ? [
+                        [r, o],
+                        [i, o],
+                        [i, u],
+                        [r, u]
+                    ] : [];
+                s.point = n[a]
+            }), t
+        }
+
+        function e(n) {
+            return n.map(function(n, t) {
+                return {
+                    x: Math.round(i(n, t) / Na) * Na,
+                    y: Math.round(o(n, t) / Na) * Na,
+                    i: t
+                }
+            })
+        }
+        var r = Ar,
+            u = Cr,
+            i = r,
+            o = u,
+            a = nl;
+        return n ? t(n) : (t.links = function(n) {
+            return iu(e(n)).edges.filter(function(n) {
+                return n.l && n.r
+            }).map(function(t) {
+                return {
+                    source: n[t.l.i],
+                    target: n[t.r.i]
+                }
+            })
+        }, t.triangles = function(n) {
+            var t = [];
+            return iu(e(n)).cells.forEach(function(e, r) {
+                for (var u, i, o = e.site, a = e.edges.sort(Ir), c = -1, l = a.length, s = a[l - 1].edge, f = s.l === o ? s.r : s.l; ++c < l;) u = s, i = f, s = a[c].edge, f = s.l === o ? s.r : s.l, r < i.i && r < f.i && au(o, i, f) < 0 && t.push([n[r], n[i.i], n[f.i]])
+            }), t
+        }, t.x = function(n) {
+            return arguments.length ? (i = kt(r = n), t) : r
+        }, t.y = function(n) {
+            return arguments.length ? (o = kt(u = n), t) : u
+        }, t.clipExtent = function(n) {
+            return arguments.length ? (a = null == n ? nl : n, t) : a === nl ? null : a
+        }, t.size = function(n) {
+            return arguments.length ? t.clipExtent(n && [
+                [0, 0], n
+            ]) : a === nl ? null : a && a[1]
+        }, t)
+    };
+    var nl = [
+        [-1e6, -1e6],
+        [1e6, 1e6]
+    ];
+    Bo.geom.delaunay = function(n) {
+        return Bo.geom.voronoi().triangles(n)
+    }, Bo.geom.quadtree = function(n, t, e, r, u) {
+        function i(n) {
+            function i(n, t, e, r, u, i, o, a) {
+                if (!isNaN(e) && !isNaN(r))
+                    if (n.leaf) {
+                        var c = n.x,
+                            s = n.y;
+                        if (null != c)
+                            if (ca(c - e) + ca(s - r) < .01) l(n, t, e, r, u, i, o, a);
+                            else {
+                                var f = n.point;
+                                n.x = n.y = n.point = null, l(n, f, c, s, u, i, o, a), l(n, t, e, r, u, i, o, a)
+                            }
+                        else n.x = e, n.y = r, n.point = t
+                    } else l(n, t, e, r, u, i, o, a)
+            }
+
+            function l(n, t, e, r, u, o, a, c) {
+                var l = .5 * (u + a),
+                    s = .5 * (o + c),
+                    f = e >= l,
+                    h = r >= s,
+                    g = (h << 1) + f;
+                n.leaf = !1, n = n.nodes[g] || (n.nodes[g] = su()), f ? u = l : a = l, h ? o = s : c = s, i(n, t, e, r, u, o, a, c)
+            }
+            var s, f, h, g, p, v, d, m, y, x = kt(a),
+                M = kt(c);
+            if (null != t) v = t, d = e, m = r, y = u;
+            else if (m = y = -(v = d = 1 / 0), f = [], h = [], p = n.length, o)
+                for (g = 0; p > g; ++g) s = n[g], s.x < v && (v = s.x), s.y < d && (d = s.y), s.x > m && (m = s.x), s.y > y && (y = s.y), f.push(s.x), h.push(s.y);
+            else
+                for (g = 0; p > g; ++g) {
+                    var _ = +x(s = n[g], g),
+                        b = +M(s, g);
+                    v > _ && (v = _), d > b && (d = b), _ > m && (m = _), b > y && (y = b), f.push(_), h.push(b)
+                }
+            var w = m - v,
+                S = y - d;
+            w > S ? y = d + w : m = v + S;
+            var k = su();
+            if (k.add = function(n) {
+                    i(k, n, +x(n, ++g), +M(n, g), v, d, m, y)
+                }, k.visit = function(n) {
+                    fu(n, k, v, d, m, y)
+                }, g = -1, null == t) {
+                for (; ++g < p;) i(k, n[g], f[g], h[g], v, d, m, y);
+                --g
+            } else n.forEach(k.add);
+            return f = h = n = s = null, k
+        }
+        var o, a = Ar,
+            c = Cr;
+        return (o = arguments.length) ? (a = cu, c = lu, 3 === o && (u = e, r = t, e = t = 0), i(n)) : (i.x = function(n) {
+            return arguments.length ? (a = n, i) : a
+        }, i.y = function(n) {
+            return arguments.length ? (c = n, i) : c
+        }, i.extent = function(n) {
+            return arguments.length ? (null == n ? t = e = r = u = null : (t = +n[0][0], e = +n[0][1], r = +n[1][0], u = +n[1][1]), i) : null == t ? null : [
+                [t, e],
+                [r, u]
+            ]
+        }, i.size = function(n) {
+            return arguments.length ? (null == n ? t = e = r = u = null : (t = e = 0, r = +n[0], u = +n[1]), i) : null == t ? null : [r - t, u - e]
+        }, i)
+    }, Bo.interpolateRgb = hu, Bo.interpolateObject = gu, Bo.interpolateNumber = pu, Bo.interpolateString = vu;
+    var tl = /[-+]?(?:\d+\.?\d*|\.?\d+)(?:[eE][-+]?\d+)?/g,
+        el = new RegExp(tl.source, "g");
+    Bo.interpolate = du, Bo.interpolators = [function(n, t) {
+        var e = typeof t;
+        return ("string" === e ? $a.has(t) || /^(#|rgb\(|hsl\()/.test(t) ? hu : vu : t instanceof it ? hu : Array.isArray(t) ? mu : "object" === e && isNaN(t) ? gu : pu)(n, t)
+    }], Bo.interpolateArray = mu;
+    var rl = function() {
+            return Et
+        },
+        ul = Bo.map({
+            linear: rl,
+            poly: Su,
+            quad: function() {
+                return _u
+            },
+            cubic: function() {
+                return bu
+            },
+            sin: function() {
+                return ku
+            },
+            exp: function() {
+                return Eu
+            },
+            circle: function() {
+                return Au
+            },
+            elastic: Cu,
+            back: Nu,
+            bounce: function() {
+                return zu
+            }
+        }),
+        il = Bo.map({
+            "in": Et,
+            out: xu,
+            "in-out": Mu,
+            "out-in": function(n) {
+                return Mu(xu(n))
+            }
+        });
+    Bo.ease = function(n) {
+        var t = n.indexOf("-"),
+            e = t >= 0 ? n.slice(0, t) : n,
+            r = t >= 0 ? n.slice(t + 1) : "in";
+        return e = ul.get(e) || rl, r = il.get(r) || Et, yu(r(e.apply(null, Wo.call(arguments, 1))))
+    }, Bo.interpolateHcl = Lu, Bo.interpolateHsl = Tu, Bo.interpolateLab = qu, Bo.interpolateRound = Ru, Bo.transform = function(n) {
+        var t = Go.createElementNS(Bo.ns.prefix.svg, "g");
+        return (Bo.transform = function(n) {
+            if (null != n) {
+                t.setAttribute("transform", n);
+                var e = t.transform.baseVal.consolidate()
+            }
+            return new Du(e ? e.matrix : ol)
+        })(n)
+    }, Du.prototype.toString = function() {
+        return "translate(" + this.translate + ")rotate(" + this.rotate + ")skewX(" + this.skew + ")scale(" + this.scale + ")"
+    };
+    var ol = {
+        a: 1,
+        b: 0,
+        c: 0,
+        d: 1,
+        e: 0,
+        f: 0
+    };
+    Bo.interpolateTransform = Fu, Bo.layout = {}, Bo.layout.bundle = function() {
+        return function(n) {
+            for (var t = [], e = -1, r = n.length; ++e < r;) t.push(Yu(n[e]));
+            return t
+        }
+    }, Bo.layout.chord = function() {
+        function n() {
+            var n, l, f, h, g, p = {},
+                v = [],
+                d = Bo.range(i),
+                m = [];
+            for (e = [], r = [], n = 0, h = -1; ++h < i;) {
+                for (l = 0, g = -1; ++g < i;) l += u[h][g];
+                v.push(l), m.push(Bo.range(i)), n += l
+            }
+            for (o && d.sort(function(n, t) {
+                    return o(v[n], v[t])
+                }), a && m.forEach(function(n, t) {
+                    n.sort(function(n, e) {
+                        return a(u[t][n], u[t][e])
                     })
-                }, Na.style = function(n, t, e) {
-                    var r = arguments.length;
-                    if (r < 3) {
-                        if ("string" != typeof n) {
-                            for (e in r < 2 && (t = ""), n) this.style(e, n[e], t);
-                            return this
-                        }
-                        e = ""
-                    }
+                }), n = (Aa - s * i) / n, l = 0, h = -1; ++h < i;) {
+                for (f = l, g = -1; ++g < i;) {
+                    var y = d[h],
+                        x = m[y][g],
+                        M = u[y][x],
+                        _ = l,
+                        b = l += M * n;
+                    p[y + "-" + x] = {
+                        index: y,
+                        subindex: x,
+                        startAngle: _,
+                        endAngle: b,
+                        value: M
+                    }
+                }
+                r[y] = {
+                    index: y,
+                    startAngle: f,
+                    endAngle: l,
+                    value: (l - f) / n
+                }, l += s
+            }
+            for (h = -1; ++h < i;)
+                for (g = h - 1; ++g < i;) {
+                    var w = p[h + "-" + g],
+                        S = p[g + "-" + h];
+                    (w.value || S.value) && e.push(w.value < S.value ? {
+                        source: S,
+                        target: w
+                    } : {
+                        source: w,
+                        target: S
+                    })
+                }
+            c && t()
+        }
 
-                    function i() {
-                        this.style.removeProperty(n)
+        function t() {
+            e.sort(function(n, t) {
+                return c((n.source.value + n.target.value) / 2, (t.source.value + t.target.value) / 2)
+            })
+        }
+        var e, r, u, i, o, a, c, l = {},
+            s = 0;
+        return l.matrix = function(n) {
+            return arguments.length ? (i = (u = n) && u.length, e = r = null, l) : u
+        }, l.padding = function(n) {
+            return arguments.length ? (s = n, e = r = null, l) : s
+        }, l.sortGroups = function(n) {
+            return arguments.length ? (o = n, e = r = null, l) : o
+        }, l.sortSubgroups = function(n) {
+            return arguments.length ? (a = n, e = null, l) : a
+        }, l.sortChords = function(n) {
+            return arguments.length ? (c = n, e && t(), l) : c
+        }, l.chords = function() {
+            return e || n(), e
+        }, l.groups = function() {
+            return r || n(), r
+        }, l
+    }, Bo.layout.force = function() {
+        function n(n) {
+            return function(t, e, r, u) {
+                if (t.point !== n) {
+                    var i = t.cx - n.x,
+                        o = t.cy - n.y,
+                        a = u - e,
+                        c = i * i + o * o;
+                    if (c > a * a / d) {
+                        if (p > c) {
+                            var l = t.charge / c;
+                            n.px -= i * l, n.py -= o * l
+                        }
+                        return !0
+                    }
+                    if (t.point && c && p > c) {
+                        var l = t.pointCharge / c;
+                        n.px -= i * l, n.py -= o * l
                     }
+                }
+                return !t.charge
+            }
+        }
 
-                    function u(t) {
-                        return null == t ? i : (t += "", function() {
-                            var r, i = f(this).getComputedStyle(this, null).getPropertyValue(n);
-                            return i !== t && (r = ru(i, t), function(t) {
-                                this.style.setProperty(n, r(t), e)
-                            })
-                        })
-                    }
-                    return Aa(this, "style." + n, t, u)
-                }, Na.styleTween = function(n, t, e) {
-                    function r(r, i) {
-                        var u = t.call(this, r, i, f(this).getComputedStyle(this, null).getPropertyValue(n));
-                        return u && function(t) {
-                            this.style.setProperty(n, u(t), e)
-                        }
-                    }
-                    return arguments.length < 3 && (e = ""), this.tween("style." + n, r)
-                }, Na.text = function(n) {
-                    return Aa(this, "text", n, Ca)
-                }, Na.remove = function() {
-                    var n = this.namespace;
-                    return this.each("end.transition", (function() {
-                        var t;
-                        this[n].count < 2 && (t = this.parentNode) && t.removeChild(this)
-                    }))
-                }, Na.ease = function(n) {
-                    var t = this.id,
-                        e = this.namespace;
-                    return arguments.length < 1 ? this.node()[e][t].ease : ("function" != typeof n && (n = u.ease.apply(u, arguments)), vn(this, (function(r) {
-                        r[e][t].ease = n
-                    })))
-                }, Na.delay = function(n) {
-                    var t = this.id,
-                        e = this.namespace;
-                    return arguments.length < 1 ? this.node()[e][t].delay : vn(this, "function" == typeof n ? function(r, i, u) {
-                        r[e][t].delay = +n.call(r, r.__data__, i, u)
-                    } : (n = +n, function(r) {
-                        r[e][t].delay = n
-                    }))
-                }, Na.duration = function(n) {
-                    var t = this.id,
-                        e = this.namespace;
-                    return arguments.length < 1 ? this.node()[e][t].duration : vn(this, "function" == typeof n ? function(r, i, u) {
-                        r[e][t].duration = Math.max(1, n.call(r, r.__data__, i, u))
-                    } : (n = Math.max(1, n), function(r) {
-                        r[e][t].duration = n
-                    }))
-                }, Na.each = function(n, t) {
-                    var e = this.id,
-                        r = this.namespace;
-                    if (arguments.length < 2) {
-                        var i = Sa,
-                            o = ka;
-                        try {
-                            ka = e, vn(this, (function(t, i, u) {
-                                Sa = t[r][e], n.call(t, t.__data__, i, u)
-                            }))
-                        } finally {
-                            Sa = i, ka = o
-                        }
-                    } else vn(this, (function(i) {
-                        var o = i[r][e];
-                        (o.event || (o.event = u.dispatch("start", "end", "interrupt"))).on(n, t)
-                    }));
-                    return this
-                }, Na.transition = function() {
-                    for (var n, t, e, r = this.id, i = ++Ea, u = this.namespace, o = [], a = 0, l = this.length; a < l; a++) {
-                        o.push(n = []);
-                        for (var c, f = 0, s = (c = this[a]).length; f < s; f++)(t = c[f]) && La(t, f, u, i, {
-                            time: (e = t[u][r]).time,
-                            ease: e.ease,
-                            delay: e.delay + e.duration,
-                            duration: e.duration
-                        }), n.push(t)
-                    }
-                    return _a(o, u, i)
-                }, u.svg.axis = function() {
-                    var n, t = u.scale.linear(),
-                        e = qa,
-                        r = 6,
-                        i = 6,
-                        o = 3,
-                        l = [10],
-                        c = null;
-
-                    function f(a) {
-                        a.each((function() {
-                            var a, f = u.select(this),
-                                s = this.__chart__ || t,
-                                h = this.__chart__ = t.copy(),
-                                p = null == c ? h.ticks ? h.ticks.apply(h, l) : h.domain() : c,
-                                g = null == n ? h.tickFormat ? h.tickFormat.apply(h, l) : R : n,
-                                v = f.selectAll(".tick").data(p, h),
-                                d = v.enter().insert("g", ".domain").attr("class", "tick").style("opacity", Cn),
-                                y = u.transition(v.exit()).style("opacity", Cn).remove(),
-                                m = u.transition(v.order()).style("opacity", 1),
-                                M = Math.max(r, 0) + o,
-                                x = xo(h),
-                                b = f.selectAll(".domain").data([0]),
-                                w = (b.enter().append("path").attr("class", "domain"), u.transition(b));
-                            d.append("line"), d.append("text");
-                            var _, k, S, N, E = d.select("line"),
-                                A = m.select("line"),
-                                C = v.select("text").text(g),
-                                z = d.select("text"),
-                                L = m.select("text"),
-                                q = "top" === e || "left" === e ? -1 : 1;
-                            if ("bottom" === e || "top" === e ? (a = Ra, _ = "x", S = "y", k = "x2", N = "y2", C.attr("dy", q < 0 ? "0em" : ".71em").style("text-anchor", "middle"), w.attr("d", "M" + x[0] + "," + q * i + "V0H" + x[1] + "V" + q * i)) : (a = Da, _ = "y", S = "x", k = "y2", N = "x2", C.attr("dy", ".32em").style("text-anchor", q < 0 ? "end" : "start"), w.attr("d", "M" + q * i + "," + x[0] + "H0V" + x[1] + "H" + q * i)), E.attr(N, q * r), z.attr(S, q * M), A.attr(k, 0).attr(N, q * r), L.attr(_, 0).attr(S, q * M), h.rangeBand) {
-                                var T = h,
-                                    D = T.rangeBand() / 2;
-                                s = h = function(n) {
-                                    return T(n) + D
-                                }
-                            } else s.rangeBand ? s = h : y.call(a, h, s);
-                            d.call(a, s, h), m.call(a, h, h)
-                        }))
-                    }
-                    return f.scale = function(n) {
-                        return arguments.length ? (t = n, f) : t
-                    }, f.orient = function(n) {
-                        return arguments.length ? (e = n in Ta ? n + "" : qa, f) : e
-                    }, f.ticks = function() {
-                        return arguments.length ? (l = a(arguments), f) : l
-                    }, f.tickValues = function(n) {
-                        return arguments.length ? (c = n, f) : c
-                    }, f.tickFormat = function(t) {
-                        return arguments.length ? (n = t, f) : n
-                    }, f.tickSize = function(n) {
-                        var t = arguments.length;
-                        return t ? (r = +n, i = +arguments[t - 1], f) : r
-                    }, f.innerTickSize = function(n) {
-                        return arguments.length ? (r = +n, f) : r
-                    }, f.outerTickSize = function(n) {
-                        return arguments.length ? (i = +n, f) : i
-                    }, f.tickPadding = function(n) {
-                        return arguments.length ? (o = +n, f) : o
-                    }, f.tickSubdivide = function() {
-                        return arguments.length && f
-                    }, f
-                };
-                var qa = "bottom",
-                    Ta = {
-                        top: 1,
-                        right: 1,
-                        bottom: 1,
-                        left: 1
-                    };
+        function t(n) {
+            n.px = Bo.event.x, n.py = Bo.event.y, a.resume()
+        }
+        var e, r, u, i, o, a = {},
+            c = Bo.dispatch("start", "tick", "end"),
+            l = [1, 1],
+            s = .9,
+            f = al,
+            h = cl,
+            g = -30,
+            p = ll,
+            v = .1,
+            d = .64,
+            m = [],
+            y = [];
+        return a.tick = function() {
+            if ((r *= .99) < .005) return c.end({
+                type: "end",
+                alpha: r = 0
+            }), !0;
+            var t, e, a, f, h, p, d, x, M, _ = m.length,
+                b = y.length;
+            for (e = 0; b > e; ++e) a = y[e], f = a.source, h = a.target, x = h.x - f.x, M = h.y - f.y, (p = x * x + M * M) && (p = r * i[e] * ((p = Math.sqrt(p)) - u[e]) / p, x *= p, M *= p, h.x -= x * (d = f.weight / (h.weight + f.weight)), h.y -= M * d, f.x += x * (d = 1 - d), f.y += M * d);
+            if ((d = r * v) && (x = l[0] / 2, M = l[1] / 2, e = -1, d))
+                for (; ++e < _;) a = m[e], a.x += (x - a.x) * d, a.y += (M - a.y) * d;
+            if (g)
+                for (Wu(t = Bo.geom.quadtree(m), r, o), e = -1; ++e < _;)(a = m[e]).fixed || t.visit(n(a));
+            for (e = -1; ++e < _;) a = m[e], a.fixed ? (a.x = a.px, a.y = a.py) : (a.x -= (a.px - (a.px = a.x)) * s, a.y -= (a.py - (a.py = a.y)) * s);
+            c.tick({
+                type: "tick",
+                alpha: r
+            })
+        }, a.nodes = function(n) {
+            return arguments.length ? (m = n, a) : m
+        }, a.links = function(n) {
+            return arguments.length ? (y = n, a) : y
+        }, a.size = function(n) {
+            return arguments.length ? (l = n, a) : l
+        }, a.linkDistance = function(n) {
+            return arguments.length ? (f = "function" == typeof n ? n : +n, a) : f
+        }, a.distance = a.linkDistance, a.linkStrength = function(n) {
+            return arguments.length ? (h = "function" == typeof n ? n : +n, a) : h
+        }, a.friction = function(n) {
+            return arguments.length ? (s = +n, a) : s
+        }, a.charge = function(n) {
+            return arguments.length ? (g = "function" == typeof n ? n : +n, a) : g
+        }, a.chargeDistance = function(n) {
+            return arguments.length ? (p = n * n, a) : Math.sqrt(p)
+        }, a.gravity = function(n) {
+            return arguments.length ? (v = +n, a) : v
+        }, a.theta = function(n) {
+            return arguments.length ? (d = n * n, a) : Math.sqrt(d)
+        }, a.alpha = function(n) {
+            return arguments.length ? (n = +n, r ? r = n > 0 ? n : 0 : n > 0 && (c.start({
+                type: "start",
+                alpha: r = n
+            }), Bo.timer(a.tick)), a) : r
+        }, a.start = function() {
+            function n(n, r) {
+                if (!e) {
+                    for (e = new Array(c), a = 0; c > a; ++a) e[a] = [];
+                    for (a = 0; l > a; ++a) {
+                        var u = y[a];
+                        e[u.source.index].push(u.target), e[u.target.index].push(u.source)
+                    }
+                }
+                for (var i, o = e[t], a = -1, l = o.length; ++a < l;)
+                    if (!isNaN(i = o[a][n])) return i;
+                return Math.random() * r
+            }
+            var t, e, r, c = m.length,
+                s = y.length,
+                p = l[0],
+                v = l[1];
+            for (t = 0; c > t; ++t)(r = m[t]).index = t, r.weight = 0;
+            for (t = 0; s > t; ++t) r = y[t], "number" == typeof r.source && (r.source = m[r.source]), "number" == typeof r.target && (r.target = m[r.target]), ++r.source.weight, ++r.target.weight;
+            for (t = 0; c > t; ++t) r = m[t], isNaN(r.x) && (r.x = n("x", p)), isNaN(r.y) && (r.y = n("y", v)), isNaN(r.px) && (r.px = r.x), isNaN(r.py) && (r.py = r.y);
+            if (u = [], "function" == typeof f)
+                for (t = 0; s > t; ++t) u[t] = +f.call(this, y[t], t);
+            else
+                for (t = 0; s > t; ++t) u[t] = f;
+            if (i = [], "function" == typeof h)
+                for (t = 0; s > t; ++t) i[t] = +h.call(this, y[t], t);
+            else
+                for (t = 0; s > t; ++t) i[t] = h;
+            if (o = [], "function" == typeof g)
+                for (t = 0; c > t; ++t) o[t] = +g.call(this, m[t], t);
+            else
+                for (t = 0; c > t; ++t) o[t] = g;
+            return a.resume()
+        }, a.resume = function() {
+            return a.alpha(.1)
+        }, a.stop = function() {
+            return a.alpha(0)
+        }, a.drag = function() {
+            return e || (e = Bo.behavior.drag().origin(Et).on("dragstart.force", Vu).on("drag.force", t).on("dragend.force", Xu)), arguments.length ? (this.on("mouseover.force", $u).on("mouseout.force", Bu).call(e), void 0) : e
+        }, Bo.rebind(a, c, "on")
+    };
+    var al = 20,
+        cl = 1,
+        ll = 1 / 0;
+    Bo.layout.hierarchy = function() {
+        function n(u) {
+            var i, o = [u],
+                a = [];
+            for (u.depth = 0; null != (i = o.pop());)
+                if (a.push(i), (l = e.call(n, i, i.depth)) && (c = l.length)) {
+                    for (var c, l, s; --c >= 0;) o.push(s = l[c]), s.parent = i, s.depth = i.depth + 1;
+                    r && (i.value = 0), i.children = l
+                } else r && (i.value = +r.call(n, i, i.depth) || 0), delete i.children;
+            return Ku(u, function(n) {
+                var e, u;
+                t && (e = n.children) && e.sort(t), r && (u = n.parent) && (u.value += n.value)
+            }), a
+        }
+        var t = ti,
+            e = Qu,
+            r = ni;
+        return n.sort = function(e) {
+            return arguments.length ? (t = e, n) : t
+        }, n.children = function(t) {
+            return arguments.length ? (e = t, n) : e
+        }, n.value = function(t) {
+            return arguments.length ? (r = t, n) : r
+        }, n.revalue = function(t) {
+            return r && (Gu(t, function(n) {
+                n.children && (n.value = 0)
+            }), Ku(t, function(t) {
+                var e;
+                t.children || (t.value = +r.call(n, t, t.depth) || 0), (e = t.parent) && (e.value += t.value)
+            })), t
+        }, n
+    }, Bo.layout.partition = function() {
+        function n(t, e, r, u) {
+            var i = t.children;
+            if (t.x = e, t.y = t.depth * u, t.dx = r, t.dy = u, i && (o = i.length)) {
+                var o, a, c, l = -1;
+                for (r = t.value ? r / t.value : 0; ++l < o;) n(a = i[l], e, c = a.value * r, u), e += c
+            }
+        }
 
-                function Ra(n, t, e) {
-                    n.attr("transform", (function(n) {
-                        var r = t(n);
-                        return "translate(" + (isFinite(r) ? r : e(n)) + ",0)"
-                    }))
-                }
+        function t(n) {
+            var e = n.children,
+                r = 0;
+            if (e && (u = e.length))
+                for (var u, i = -1; ++i < u;) r = Math.max(r, t(e[i]));
+            return 1 + r
+        }
 
-                function Da(n, t, e) {
-                    n.attr("transform", (function(n) {
-                        var r = t(n);
-                        return "translate(0," + (isFinite(r) ? r : e(n)) + ")"
-                    }))
+        function e(e, i) {
+            var o = r.call(this, e, i);
+            return n(o[0], 0, u[0], u[1] / t(o[0])), o
+        }
+        var r = Bo.layout.hierarchy(),
+            u = [1, 1];
+        return e.size = function(n) {
+            return arguments.length ? (u = n, e) : u
+        }, Ju(e, r)
+    }, Bo.layout.pie = function() {
+        function n(i) {
+            var o = i.map(function(e, r) {
+                    return +t.call(n, e, r)
+                }),
+                a = +("function" == typeof r ? r.apply(this, arguments) : r),
+                c = (("function" == typeof u ? u.apply(this, arguments) : u) - a) / Bo.sum(o),
+                l = Bo.range(i.length);
+            null != e && l.sort(e === sl ? function(n, t) {
+                return o[t] - o[n]
+            } : function(n, t) {
+                return e(i[n], i[t])
+            });
+            var s = [];
+            return l.forEach(function(n) {
+                var t;
+                s[n] = {
+                    data: i[n],
+                    value: t = o[n],
+                    startAngle: a,
+                    endAngle: a += t * c
                 }
-                u.svg.brush = function() {
-                    var n, t, e = Y(h, "brushstart", "brush", "brushend"),
-                        r = null,
-                        i = null,
-                        o = [0, 0],
-                        a = [0, 0],
-                        l = !0,
-                        c = !0,
-                        s = Ua[0];
-
-                    function h(n) {
-                        n.each((function() {
-                            var n = u.select(this).style("pointer-events", "all").style("-webkit-tap-highlight-color", "rgba(0,0,0,0)").on("mousedown.brush", d).on("touchstart.brush", d),
-                                t = n.selectAll(".background").data([0]);
-                            t.enter().append("rect").attr("class", "background").style("visibility", "hidden").style("cursor", "crosshair"), n.selectAll(".extent").data([0]).enter().append("rect").attr("class", "extent").style("cursor", "move");
-                            var e = n.selectAll(".resize").data(s, R);
-                            e.exit().remove(), e.enter().append("g").attr("class", (function(n) {
-                                return "resize " + n
-                            })).style("cursor", (function(n) {
-                                return Pa[n]
-                            })).append("rect").attr("x", (function(n) {
-                                return /[ew]$/.test(n) ? -3 : null
-                            })).attr("y", (function(n) {
-                                return /^[ns]/.test(n) ? -3 : null
-                            })).attr("width", 6).attr("height", 6).style("visibility", "hidden"), e.style("display", h.empty() ? "none" : null);
-                            var o, a = u.transition(n),
-                                l = u.transition(t);
-                            r && (o = xo(r), l.attr("x", o[0]).attr("width", o[1] - o[0]), g(a)), i && (o = xo(i), l.attr("y", o[0]).attr("height", o[1] - o[0]), v(a)), p(a)
-                        }))
-                    }
+            }), s
+        }
+        var t = Number,
+            e = sl,
+            r = 0,
+            u = Aa;
+        return n.value = function(e) {
+            return arguments.length ? (t = e, n) : t
+        }, n.sort = function(t) {
+            return arguments.length ? (e = t, n) : e
+        }, n.startAngle = function(t) {
+            return arguments.length ? (r = t, n) : r
+        }, n.endAngle = function(t) {
+            return arguments.length ? (u = t, n) : u
+        }, n
+    };
+    var sl = {};
+    Bo.layout.stack = function() {
+        function n(a, c) {
+            if (!(h = a.length)) return a;
+            var l = a.map(function(e, r) {
+                    return t.call(n, e, r)
+                }),
+                s = l.map(function(t) {
+                    return t.map(function(t, e) {
+                        return [i.call(n, t, e), o.call(n, t, e)]
+                    })
+                }),
+                f = e.call(n, s, c);
+            l = Bo.permute(l, f), s = Bo.permute(s, f);
+            var h, g, p, v, d = r.call(n, s, c),
+                m = l[0].length;
+            for (p = 0; m > p; ++p)
+                for (u.call(n, l[0][p], v = d[p], s[0][p][1]), g = 1; h > g; ++g) u.call(n, l[g][p], v += s[g - 1][p][1], s[g][p][1]);
+            return a
+        }
+        var t = Et,
+            e = oi,
+            r = ai,
+            u = ii,
+            i = ri,
+            o = ui;
+        return n.values = function(e) {
+            return arguments.length ? (t = e, n) : t
+        }, n.order = function(t) {
+            return arguments.length ? (e = "function" == typeof t ? t : fl.get(t) || oi, n) : e
+        }, n.offset = function(t) {
+            return arguments.length ? (r = "function" == typeof t ? t : hl.get(t) || ai, n) : r
+        }, n.x = function(t) {
+            return arguments.length ? (i = t, n) : i
+        }, n.y = function(t) {
+            return arguments.length ? (o = t, n) : o
+        }, n.out = function(t) {
+            return arguments.length ? (u = t, n) : u
+        }, n
+    };
+    var fl = Bo.map({
+            "inside-out": function(n) {
+                var t, e, r = n.length,
+                    u = n.map(ci),
+                    i = n.map(li),
+                    o = Bo.range(r).sort(function(n, t) {
+                        return u[n] - u[t]
+                    }),
+                    a = 0,
+                    c = 0,
+                    l = [],
+                    s = [];
+                for (t = 0; r > t; ++t) e = o[t], c > a ? (a += i[e], l.push(e)) : (c += i[e], s.push(e));
+                return s.reverse().concat(l)
+            },
+            reverse: function(n) {
+                return Bo.range(n.length).reverse()
+            },
+            "default": oi
+        }),
+        hl = Bo.map({
+            silhouette: function(n) {
+                var t, e, r, u = n.length,
+                    i = n[0].length,
+                    o = [],
+                    a = 0,
+                    c = [];
+                for (e = 0; i > e; ++e) {
+                    for (t = 0, r = 0; u > t; t++) r += n[t][e][1];
+                    r > a && (a = r), o.push(r)
+                }
+                for (e = 0; i > e; ++e) c[e] = (a - o[e]) / 2;
+                return c
+            },
+            wiggle: function(n) {
+                var t, e, r, u, i, o, a, c, l, s = n.length,
+                    f = n[0],
+                    h = f.length,
+                    g = [];
+                for (g[0] = c = l = 0, e = 1; h > e; ++e) {
+                    for (t = 0, u = 0; s > t; ++t) u += n[t][e][1];
+                    for (t = 0, i = 0, a = f[e][0] - f[e - 1][0]; s > t; ++t) {
+                        for (r = 0, o = (n[t][e][1] - n[t][e - 1][1]) / (2 * a); t > r; ++r) o += (n[r][e][1] - n[r][e - 1][1]) / a;
+                        i += o * n[t][e][1]
+                    }
+                    g[e] = c -= u ? i / u * a : 0, l > c && (l = c)
+                }
+                for (e = 0; h > e; ++e) g[e] -= l;
+                return g
+            },
+            expand: function(n) {
+                var t, e, r, u = n.length,
+                    i = n[0].length,
+                    o = 1 / u,
+                    a = [];
+                for (e = 0; i > e; ++e) {
+                    for (t = 0, r = 0; u > t; t++) r += n[t][e][1];
+                    if (r)
+                        for (t = 0; u > t; t++) n[t][e][1] /= r;
+                    else
+                        for (t = 0; u > t; t++) n[t][e][1] = o
+                }
+                for (e = 0; i > e; ++e) a[e] = 0;
+                return a
+            },
+            zero: ai
+        });
+    Bo.layout.histogram = function() {
+        function n(n, i) {
+            for (var o, a, c = [], l = n.map(e, this), s = r.call(this, l, i), f = u.call(this, s, l, i), i = -1, h = l.length, g = f.length - 1, p = t ? 1 : 1 / h; ++i < g;) o = c[i] = [], o.dx = f[i + 1] - (o.x = f[i]), o.y = 0;
+            if (g > 0)
+                for (i = -1; ++i < h;) a = l[i], a >= s[0] && a <= s[1] && (o = c[Bo.bisect(f, a, 1, g) - 1], o.y += p, o.push(n[i]));
+            return c
+        }
+        var t = !0,
+            e = Number,
+            r = gi,
+            u = fi;
+        return n.value = function(t) {
+            return arguments.length ? (e = t, n) : e
+        }, n.range = function(t) {
+            return arguments.length ? (r = kt(t), n) : r
+        }, n.bins = function(t) {
+            return arguments.length ? (u = "number" == typeof t ? function(n) {
+                return hi(n, t)
+            } : kt(t), n) : u
+        }, n.frequency = function(e) {
+            return arguments.length ? (t = !!e, n) : t
+        }, n
+    }, Bo.layout.pack = function() {
+        function n(n, i) {
+            var o = e.call(this, n, i),
+                a = o[0],
+                c = u[0],
+                l = u[1],
+                s = null == t ? Math.sqrt : "function" == typeof t ? t : function() {
+                    return t
+                };
+            if (a.x = a.y = 0, Ku(a, function(n) {
+                    n.r = +s(n.value)
+                }), Ku(a, yi), r) {
+                var f = r * (t ? 1 : Math.max(2 * a.r / c, 2 * a.r / l)) / 2;
+                Ku(a, function(n) {
+                    n.r += f
+                }), Ku(a, yi), Ku(a, function(n) {
+                    n.r -= f
+                })
+            }
+            return _i(a, c / 2, l / 2, t ? 1 : 1 / Math.max(2 * a.r / c, 2 * a.r / l)), o
+        }
+        var t, e = Bo.layout.hierarchy().sort(pi),
+            r = 0,
+            u = [1, 1];
+        return n.size = function(t) {
+            return arguments.length ? (u = t, n) : u
+        }, n.radius = function(e) {
+            return arguments.length ? (t = null == e || "function" == typeof e ? e : +e, n) : t
+        }, n.padding = function(t) {
+            return arguments.length ? (r = +t, n) : r
+        }, Ju(n, e)
+    }, Bo.layout.tree = function() {
+        function n(n, u) {
+            var s = o.call(this, n, u),
+                f = s[0],
+                h = t(f);
+            if (Ku(h, e), h.parent.m = -h.z, Gu(h, r), l) Gu(f, i);
+            else {
+                var g = f,
+                    p = f,
+                    v = f;
+                Gu(f, function(n) {
+                    n.x < g.x && (g = n), n.x > p.x && (p = n), n.depth > v.depth && (v = n)
+                });
+                var d = a(g, p) / 2 - g.x,
+                    m = c[0] / (p.x + a(p, g) / 2 + d),
+                    y = c[1] / (v.depth || 1);
+                Gu(f, function(n) {
+                    n.x = (n.x + d) * m, n.y = n.depth * y
+                })
+            }
+            return s
+        }
 
-                    function p(n) {
-                        n.selectAll(".resize").attr("transform", (function(n) {
-                            return "translate(" + o[+/e$/.test(n)] + "," + a[+/^s/.test(n)] + ")"
-                        }))
-                    }
+        function t(n) {
+            for (var t, e = {
+                    A: null,
+                    children: [n]
+                }, r = [e]; null != (t = r.pop());)
+                for (var u, i = t.children, o = 0, a = i.length; a > o; ++o) r.push((i[o] = u = {
+                    _: i[o],
+                    parent: t,
+                    children: (u = i[o].children) && u.slice() || [],
+                    A: null,
+                    a: null,
+                    z: 0,
+                    m: 0,
+                    c: 0,
+                    s: 0,
+                    t: null,
+                    i: o
+                }).a = u);
+            return e.children[0]
+        }
 
-                    function g(n) {
-                        n.select(".extent").attr("x", o[0]), n.selectAll(".extent,.n>rect,.s>rect").attr("width", o[1] - o[0])
-                    }
+        function e(n) {
+            var t = n.children,
+                e = n.parent.children,
+                r = n.i ? e[n.i - 1] : null;
+            if (t.length) {
+                Ai(n);
+                var i = (t[0].z + t[t.length - 1].z) / 2;
+                r ? (n.z = r.z + a(n._, r._), n.m = n.z - i) : n.z = i
+            } else r && (n.z = r.z + a(n._, r._));
+            n.parent.A = u(n, r, n.parent.A || e[0])
+        }
 
-                    function v(n) {
-                        n.select(".extent").attr("y", a[0]), n.selectAll(".extent,.e>rect,.w>rect").attr("height", a[1] - a[0])
-                    }
+        function r(n) {
+            n._.x = n.z + n.parent.m, n.m += n.parent.m
+        }
 
-                    function d() {
-                        var s, d, y = this,
-                            m = u.select(u.event.target),
-                            M = e.of(y, arguments),
-                            x = u.select(y),
-                            b = m.datum(),
-                            w = !/^(n|s)$/.test(b) && r,
-                            _ = !/^(e|w)$/.test(b) && i,
-                            k = m.classed("extent"),
-                            S = Sn(y),
-                            N = u.mouse(y),
-                            E = u.select(f(y)).on("keydown.brush", z).on("keyup.brush", L);
-                        if (u.event.changedTouches ? E.on("touchmove.brush", q).on("touchend.brush", R) : E.on("mousemove.brush", q).on("mouseup.brush", R), x.interrupt().selectAll("*").interrupt(), k) N[0] = o[0] - N[0], N[1] = a[0] - N[1];
-                        else if (b) {
-                            var A = +/w$/.test(b),
-                                C = +/^n/.test(b);
-                            d = [o[1 - A] - N[0], a[1 - C] - N[1]], N[0] = o[A], N[1] = a[C]
-                        } else u.event.altKey && (s = N.slice());
+        function u(n, t, e) {
+            if (t) {
+                for (var r, u = n, i = n, o = t, c = u.parent.children[0], l = u.m, s = i.m, f = o.m, h = c.m; o = ki(o), u = Si(u), o && u;) c = Si(c), i = ki(i), i.a = n, r = o.z + f - u.z - l + a(o._, u._), r > 0 && (Ei(Ci(o, n, e), n, r), l += r, s += r), f += o.m, l += u.m, h += c.m, s += i.m;
+                o && !ki(i) && (i.t = o, i.m += f - s), u && !Si(c) && (c.t = u, c.m += l - h, e = n)
+            }
+            return e
+        }
 
-                        function z() {
-                            32 == u.event.keyCode && (k || (s = null, N[0] -= o[1], N[1] -= a[1], k = 2), O())
-                        }
+        function i(n) {
+            n.x *= c[0], n.y = n.depth * c[1]
+        }
+        var o = Bo.layout.hierarchy().sort(null).value(null),
+            a = wi,
+            c = [1, 1],
+            l = null;
+        return n.separation = function(t) {
+            return arguments.length ? (a = t, n) : a
+        }, n.size = function(t) {
+            return arguments.length ? (l = null == (c = t) ? i : null, n) : l ? null : c
+        }, n.nodeSize = function(t) {
+            return arguments.length ? (l = null == (c = t) ? null : i, n) : l ? c : null
+        }, Ju(n, o)
+    }, Bo.layout.cluster = function() {
+        function n(n, i) {
+            var o, a = t.call(this, n, i),
+                c = a[0],
+                l = 0;
+            Ku(c, function(n) {
+                var t = n.children;
+                t && t.length ? (n.x = zi(t), n.y = Ni(t)) : (n.x = o ? l += e(n, o) : 0, n.y = 0, o = n)
+            });
+            var s = Li(c),
+                f = Ti(c),
+                h = s.x - e(s, f) / 2,
+                g = f.x + e(f, s) / 2;
+            return Ku(c, u ? function(n) {
+                n.x = (n.x - c.x) * r[0], n.y = (c.y - n.y) * r[1]
+            } : function(n) {
+                n.x = (n.x - h) / (g - h) * r[0], n.y = (1 - (c.y ? n.y / c.y : 1)) * r[1]
+            }), a
+        }
+        var t = Bo.layout.hierarchy().sort(null).value(null),
+            e = wi,
+            r = [1, 1],
+            u = !1;
+        return n.separation = function(t) {
+            return arguments.length ? (e = t, n) : e
+        }, n.size = function(t) {
+            return arguments.length ? (u = null == (r = t), n) : u ? null : r
+        }, n.nodeSize = function(t) {
+            return arguments.length ? (u = null != (r = t), n) : u ? r : null
+        }, Ju(n, t)
+    }, Bo.layout.treemap = function() {
+        function n(n, t) {
+            for (var e, r, u = -1, i = n.length; ++u < i;) r = (e = n[u]).value * (0 > t ? 0 : t), e.area = isNaN(r) || 0 >= r ? 0 : r
+        }
 
-                        function L() {
-                            32 == u.event.keyCode && 2 == k && (N[0] += o[1], N[1] += a[1], k = 0, O())
-                        }
+        function t(e) {
+            var i = e.children;
+            if (i && i.length) {
+                var o, a, c, l = f(e),
+                    s = [],
+                    h = i.slice(),
+                    p = 1 / 0,
+                    v = "slice" === g ? l.dx : "dice" === g ? l.dy : "slice-dice" === g ? 1 & e.depth ? l.dy : l.dx : Math.min(l.dx, l.dy);
+                for (n(h, l.dx * l.dy / e.value), s.area = 0;
+                    (c = h.length) > 0;) s.push(o = h[c - 1]), s.area += o.area, "squarify" !== g || (a = r(s, v)) <= p ? (h.pop(), p = a) : (s.area -= s.pop().area, u(s, v, l, !1), v = Math.min(l.dx, l.dy), s.length = s.area = 0, p = 1 / 0);
+                s.length && (u(s, v, l, !0), s.length = s.area = 0), i.forEach(t)
+            }
+        }
 
-                        function q() {
-                            var n = u.mouse(y),
-                                t = !1;
-                            d && (n[0] += d[0], n[1] += d[1]), k || (u.event.altKey ? (s || (s = [(o[0] + o[1]) / 2, (a[0] + a[1]) / 2]), N[0] = o[+(n[0] < s[0])], N[1] = a[+(n[1] < s[1])]) : s = null), w && T(n, r, 0) && (g(x), t = !0), _ && T(n, i, 1) && (v(x), t = !0), t && (p(x), M({
-                                type: "brush",
-                                mode: k ? "move" : "resize"
-                            }))
-                        }
+        function e(t) {
+            var r = t.children;
+            if (r && r.length) {
+                var i, o = f(t),
+                    a = r.slice(),
+                    c = [];
+                for (n(a, o.dx * o.dy / t.value), c.area = 0; i = a.pop();) c.push(i), c.area += i.area, null != i.z && (u(c, i.z ? o.dx : o.dy, o, !a.length), c.length = c.area = 0);
+                r.forEach(e)
+            }
+        }
 
-                        function T(e, r, i) {
-                            var u, f, h = xo(r),
-                                p = h[0],
-                                g = h[1],
-                                v = N[i],
-                                d = i ? a : o,
-                                y = d[1] - d[0];
-                            if (k && (p -= v, g -= y + v), u = (i ? c : l) ? Math.max(p, Math.min(g, e[i])) : e[i], k ? f = (u += v) + y : (s && (v = Math.max(p, Math.min(g, 2 * s[i] - u))), v < u ? (f = u, u = v) : f = v), d[0] != u || d[1] != f) return i ? t = null : n = null, d[0] = u, d[1] = f, !0
-                        }
+        function r(n, t) {
+            for (var e, r = n.area, u = 0, i = 1 / 0, o = -1, a = n.length; ++o < a;)(e = n[o].area) && (i > e && (i = e), e > u && (u = e));
+            return r *= r, t *= t, r ? Math.max(t * u * p / r, r / (t * i * p)) : 1 / 0
+        }
 
-                        function R() {
-                            q(), x.style("pointer-events", "all").selectAll(".resize").style("display", h.empty() ? "none" : null), u.select("body").style("cursor", null), E.on("mousemove.brush", null).on("mouseup.brush", null).on("touchmove.brush", null).on("touchend.brush", null).on("keydown.brush", null).on("keyup.brush", null), S(), M({
-                                type: "brushend"
-                            })
-                        }
-                        x.style("pointer-events", "none").selectAll(".resize").style("display", null), u.select("body").style("cursor", m.style("cursor")), M({
-                            type: "brushstart"
-                        }), q()
-                    }
-                    return h.event = function(r) {
-                        r.each((function() {
-                            var r = e.of(this, arguments),
-                                i = {
-                                    x: o,
-                                    y: a,
-                                    i: n,
-                                    j: t
-                                },
-                                l = this.__chart__ || i;
-                            this.__chart__ = i, ka ? u.select(this).transition().each("start.brush", (function() {
-                                n = l.i, t = l.j, o = l.x, a = l.y, r({
-                                    type: "brushstart"
-                                })
-                            })).tween("brush:brush", (function() {
-                                var e = iu(o, i.x),
-                                    u = iu(a, i.y);
-                                return n = t = null,
-                                    function(n) {
-                                        o = i.x = e(n), a = i.y = u(n), r({
-                                            type: "brush",
-                                            mode: "resize"
-                                        })
-                                    }
-                            })).each("end.brush", (function() {
-                                n = i.i, t = i.j, r({
-                                    type: "brush",
-                                    mode: "resize"
-                                }), r({
-                                    type: "brushend"
-                                })
-                            })) : (r({
-                                type: "brushstart"
-                            }), r({
-                                type: "brush",
-                                mode: "resize"
-                            }), r({
-                                type: "brushend"
-                            }))
-                        }))
-                    }, h.x = function(n) {
-                        return arguments.length ? (s = Ua[!(r = n) << 1 | !i], h) : r
-                    }, h.y = function(n) {
-                        return arguments.length ? (s = Ua[!r << 1 | !(i = n)], h) : i
-                    }, h.clamp = function(n) {
-                        return arguments.length ? (r && i ? (l = !!n[0], c = !!n[1]) : r ? l = !!n : i && (c = !!n), h) : r && i ? [l, c] : r ? l : i ? c : null
-                    }, h.extent = function(e) {
-                        var u, l, c, f, s;
-                        return arguments.length ? (r && (u = e[0], l = e[1], i && (u = u[0], l = l[0]), n = [u, l], r.invert && (u = r(u), l = r(l)), l < u && (s = u, u = l, l = s), u == o[0] && l == o[1] || (o = [u, l])), i && (c = e[0], f = e[1], r && (c = c[1], f = f[1]), t = [c, f], i.invert && (c = i(c), f = i(f)), f < c && (s = c, c = f, f = s), c == a[0] && f == a[1] || (a = [c, f])), h) : (r && (n ? (u = n[0], l = n[1]) : (u = o[0], l = o[1], r.invert && (u = r.invert(u), l = r.invert(l)), l < u && (s = u, u = l, l = s))), i && (t ? (c = t[0], f = t[1]) : (c = a[0], f = a[1], i.invert && (c = i.invert(c), f = i.invert(f)), f < c && (s = c, c = f, f = s))), r && i ? [
-                            [u, c],
-                            [l, f]
-                        ] : r ? [u, l] : i && [c, f])
-                    }, h.clear = function() {
-                        return h.empty() || (o = [0, 0], a = [0, 0], n = t = null), h
-                    }, h.empty = function() {
-                        return !!r && o[0] == o[1] || !!i && a[0] == a[1]
-                    }, u.rebind(h, e, "on")
-                };
-                var Pa = {
-                        n: "ns-resize",
-                        e: "ew-resize",
-                        s: "ns-resize",
-                        w: "ew-resize",
-                        nw: "nwse-resize",
-                        ne: "nesw-resize",
-                        se: "nwse-resize",
-                        sw: "nesw-resize"
-                    },
-                    Ua = [
-                        ["n", "e", "s", "w", "nw", "ne", "se", "sw"],
-                        ["e", "w"],
-                        ["n", "s"],
-                        []
-                    ],
-                    ja = Ut.format = he.timeFormat,
-                    Fa = ja.utc,
-                    Ha = Fa("%Y-%m-%dT%H:%M:%S.%LZ");
-
-                function Oa(n) {
-                    return n.toISOString()
-                }
-
-                function Ia(n, t, e) {
-                    function r(t) {
-                        return n(t)
-                    }
+        function u(n, t, e, r) {
+            var u, i = -1,
+                o = n.length,
+                a = e.x,
+                l = e.y,
+                s = t ? c(n.area / t) : 0;
+            if (t == e.dx) {
+                for ((r || s > e.dy) && (s = e.dy); ++i < o;) u = n[i], u.x = a, u.y = l, u.dy = s, a += u.dx = Math.min(e.x + e.dx - a, s ? c(u.area / s) : 0);
+                u.z = !0, u.dx += e.x + e.dx - a, e.y += s, e.dy -= s
+            } else {
+                for ((r || s > e.dx) && (s = e.dx); ++i < o;) u = n[i], u.x = a, u.y = l, u.dx = s, l += u.dy = Math.min(e.y + e.dy - l, s ? c(u.area / s) : 0);
+                u.z = !1, u.dy += e.y + e.dy - l, e.x += s, e.dx -= s
+            }
+        }
 
-                    function i(n, e) {
-                        var r = (n[1] - n[0]) / e,
-                            i = u.bisect(Za, r);
-                        return i == Za.length ? [t.year, Ao(n.map((function(n) {
-                            return n / 31536e6
-                        })), e)[2]] : i ? t[r / Za[i - 1] < Za[i] / r ? i - 1 : i] : [$a, Ao(n, e)[2]]
-                    }
-                    return r.invert = function(t) {
-                        return Ya(n.invert(t))
-                    }, r.domain = function(t) {
-                        return arguments.length ? (n.domain(t), r) : n.domain().map(Ya)
-                    }, r.nice = function(n, t) {
-                        var e = r.domain(),
-                            u = Mo(e),
-                            o = null == n ? i(u, 10) : "number" == typeof n && i(u, n);
+        function i(r) {
+            var u = o || a(r),
+                i = u[0];
+            return i.x = 0, i.y = 0, i.dx = l[0], i.dy = l[1], o && a.revalue(i), n([i], i.dx * i.dy / i.value), (o ? e : t)(i), h && (o = u), u
+        }
+        var o, a = Bo.layout.hierarchy(),
+            c = Math.round,
+            l = [1, 1],
+            s = null,
+            f = qi,
+            h = !1,
+            g = "squarify",
+            p = .5 * (1 + Math.sqrt(5));
+        return i.size = function(n) {
+            return arguments.length ? (l = n, i) : l
+        }, i.padding = function(n) {
+            function t(t) {
+                var e = n.call(i, t, t.depth);
+                return null == e ? qi(t) : Ri(t, "number" == typeof e ? [e, e, e, e] : e)
+            }
+
+            function e(t) {
+                return Ri(t, n)
+            }
+            if (!arguments.length) return s;
+            var r;
+            return f = null == (s = n) ? qi : "function" == (r = typeof n) ? t : "number" === r ? (n = [n, n, n, n], e) : e, i
+        }, i.round = function(n) {
+            return arguments.length ? (c = n ? Math.round : Number, i) : c != Number
+        }, i.sticky = function(n) {
+            return arguments.length ? (h = n, o = null, i) : h
+        }, i.ratio = function(n) {
+            return arguments.length ? (p = n, i) : p
+        }, i.mode = function(n) {
+            return arguments.length ? (g = n + "", i) : g
+        }, Ju(i, a)
+    }, Bo.random = {
+        normal: function(n, t) {
+            var e = arguments.length;
+            return 2 > e && (t = 1), 1 > e && (n = 0),
+                function() {
+                    var e, r, u;
+                    do e = 2 * Math.random() - 1, r = 2 * Math.random() - 1, u = e * e + r * r; while (!u || u > 1);
+                    return n + t * e * Math.sqrt(-2 * Math.log(u) / u)
+                }
+        },
+        logNormal: function() {
+            var n = Bo.random.normal.apply(Bo, arguments);
+            return function() {
+                return Math.exp(n())
+            }
+        },
+        bates: function(n) {
+            var t = Bo.random.irwinHall(n);
+            return function() {
+                return t() / n
+            }
+        },
+        irwinHall: function(n) {
+            return function() {
+                for (var t = 0, e = 0; n > e; e++) t += Math.random();
+                return t
+            }
+        }
+    }, Bo.scale = {};
+    var gl = {
+        floor: Et,
+        ceil: Et
+    };
+    Bo.scale.linear = function() {
+        return Oi([0, 1], [0, 1], du, !1)
+    };
+    var pl = {
+        s: 1,
+        g: 1,
+        p: 1,
+        r: 1,
+        e: 1
+    };
+    Bo.scale.log = function() {
+        return Wi(Bo.scale.linear().domain([0, 1]), 10, !0, [1, 10])
+    };
+    var vl = Bo.format(".0e"),
+        dl = {
+            floor: function(n) {
+                return -Math.ceil(-n)
+            },
+            ceil: function(n) {
+                return -Math.floor(-n)
+            }
+        };
+    Bo.scale.pow = function() {
+        return Ji(Bo.scale.linear(), 1, [0, 1])
+    }, Bo.scale.sqrt = function() {
+        return Bo.scale.pow().exponent(.5)
+    }, Bo.scale.ordinal = function() {
+        return Ki([], {
+            t: "range",
+            a: [
+                []
+            ]
+        })
+    }, Bo.scale.category10 = function() {
+        return Bo.scale.ordinal().range(ml)
+    }, Bo.scale.category20 = function() {
+        return Bo.scale.ordinal().range(yl)
+    }, Bo.scale.category20b = function() {
+        return Bo.scale.ordinal().range(xl)
+    }, Bo.scale.category20c = function() {
+        return Bo.scale.ordinal().range(Ml)
+    };
+    var ml = [2062260, 16744206, 2924588, 14034728, 9725885, 9197131, 14907330, 8355711, 12369186, 1556175].map(yt),
+        yl = [2062260, 11454440, 16744206, 16759672, 2924588, 10018698, 14034728, 16750742, 9725885, 12955861, 9197131, 12885140, 14907330, 16234194, 8355711, 13092807, 12369186, 14408589, 1556175, 10410725].map(yt),
+        xl = [3750777, 5395619, 7040719, 10264286, 6519097, 9216594, 11915115, 13556636, 9202993, 12426809, 15186514, 15190932, 8666169, 11356490, 14049643, 15177372, 8077683, 10834324, 13528509, 14589654].map(yt),
+        Ml = [3244733, 7057110, 10406625, 13032431, 15095053, 16616764, 16625259, 16634018, 3253076, 7652470, 10607003, 13101504, 7695281, 10394312, 12369372, 14342891, 6513507, 9868950, 12434877, 14277081].map(yt);
+    Bo.scale.quantile = function() {
+        return Qi([], [])
+    }, Bo.scale.quantize = function() {
+        return no(0, 1, [0, 1])
+    }, Bo.scale.threshold = function() {
+        return to([.5], [0, 1])
+    }, Bo.scale.identity = function() {
+        return eo([0, 1])
+    }, Bo.svg = {}, Bo.svg.arc = function() {
+        function n() {
+            var n = t.apply(this, arguments),
+                i = e.apply(this, arguments),
+                o = r.apply(this, arguments) + _l,
+                a = u.apply(this, arguments) + _l,
+                c = (o > a && (c = o, o = a, a = c), a - o),
+                l = Ea > c ? "0" : "1",
+                s = Math.cos(o),
+                f = Math.sin(o),
+                h = Math.cos(a),
+                g = Math.sin(a);
+            return c >= bl ? n ? "M0," + i + "A" + i + "," + i + " 0 1,1 0," + -i + "A" + i + "," + i + " 0 1,1 0," + i + "M0," + n + "A" + n + "," + n + " 0 1,0 0," + -n + "A" + n + "," + n + " 0 1,0 0," + n + "Z" : "M0," + i + "A" + i + "," + i + " 0 1,1 0," + -i + "A" + i + "," + i + " 0 1,1 0," + i + "Z" : n ? "M" + i * s + "," + i * f + "A" + i + "," + i + " 0 " + l + ",1 " + i * h + "," + i * g + "L" + n * h + "," + n * g + "A" + n + "," + n + " 0 " + l + ",0 " + n * s + "," + n * f + "Z" : "M" + i * s + "," + i * f + "A" + i + "," + i + " 0 " + l + ",1 " + i * h + "," + i * g + "L0,0" + "Z"
+        }
+        var t = ro,
+            e = uo,
+            r = io,
+            u = oo;
+        return n.innerRadius = function(e) {
+            return arguments.length ? (t = kt(e), n) : t
+        }, n.outerRadius = function(t) {
+            return arguments.length ? (e = kt(t), n) : e
+        }, n.startAngle = function(t) {
+            return arguments.length ? (r = kt(t), n) : r
+        }, n.endAngle = function(t) {
+            return arguments.length ? (u = kt(t), n) : u
+        }, n.centroid = function() {
+            var n = (t.apply(this, arguments) + e.apply(this, arguments)) / 2,
+                i = (r.apply(this, arguments) + u.apply(this, arguments)) / 2 + _l;
+            return [Math.cos(i) * n, Math.sin(i) * n]
+        }, n
+    };
+    var _l = -Ca,
+        bl = Aa - Na;
+    Bo.svg.line = function() {
+        return ao(Et)
+    };
+    var wl = Bo.map({
+        linear: co,
+        "linear-closed": lo,
+        step: so,
+        "step-before": fo,
+        "step-after": ho,
+        basis: xo,
+        "basis-open": Mo,
+        "basis-closed": _o,
+        bundle: bo,
+        cardinal: vo,
+        "cardinal-open": go,
+        "cardinal-closed": po,
+        monotone: Co
+    });
+    wl.forEach(function(n, t) {
+        t.key = n, t.closed = /-closed$/.test(n)
+    });
+    var Sl = [0, 2 / 3, 1 / 3, 0],
+        kl = [0, 1 / 3, 2 / 3, 0],
+        El = [0, 1 / 6, 2 / 3, 1 / 6];
+    Bo.svg.line.radial = function() {
+        var n = ao(No);
+        return n.radius = n.x, delete n.x, n.angle = n.y, delete n.y, n
+    }, fo.reverse = ho, ho.reverse = fo, Bo.svg.area = function() {
+        return zo(Et)
+    }, Bo.svg.area.radial = function() {
+        var n = zo(No);
+        return n.radius = n.x, delete n.x, n.innerRadius = n.x0, delete n.x0, n.outerRadius = n.x1, delete n.x1, n.angle = n.y, delete n.y, n.startAngle = n.y0, delete n.y0, n.endAngle = n.y1, delete n.y1, n
+    }, Bo.svg.chord = function() {
+        function n(n, a) {
+            var c = t(this, i, n, a),
+                l = t(this, o, n, a);
+            return "M" + c.p0 + r(c.r, c.p1, c.a1 - c.a0) + (e(c, l) ? u(c.r, c.p1, c.r, c.p0) : u(c.r, c.p1, l.r, l.p0) + r(l.r, l.p1, l.a1 - l.a0) + u(l.r, l.p1, c.r, c.p0)) + "Z"
+        }
 
-                        function a(e) {
-                            return !isNaN(e) && !n.range(e, Ya(+e + 1), t).length
-                        }
-                        return o && (n = o[0], t = o[1]), r.domain(wo(e, t > 1 ? {
-                            floor: function(t) {
-                                for (; a(t = n.floor(t));) t = Ya(t - 1);
-                                return t
-                            },
-                            ceil: function(t) {
-                                for (; a(t = n.ceil(t));) t = Ya(+t + 1);
-                                return t
-                            }
-                        } : n))
-                    }, r.ticks = function(n, t) {
-                        var e = Mo(r.domain()),
-                            u = null == n ? i(e, 10) : "number" == typeof n ? i(e, n) : !n.range && [{
-                                range: n
-                            }, t];
-                        return u && (n = u[0], t = u[1]), n.range(e[0], Ya(+e[1] + 1), t < 1 ? 1 : t)
-                    }, r.tickFormat = function() {
-                        return e
-                    }, r.copy = function() {
-                        return Ia(n.copy(), t, e)
-                    }, No(r, n)
-                }
-
-                function Ya(n) {
-                    return new Date(n)
-                }
-                ja.iso = Date.prototype.toISOString && +new Date("2000-01-01T00:00:00.000Z") ? Oa : Ha, Oa.parse = function(n) {
-                    var t = new Date(n);
-                    return isNaN(t) ? null : t
-                }, Oa.toString = Ha.toString, Ut.second = Ot((function(n) {
-                    return new jt(1e3 * Math.floor(n / 1e3))
-                }), (function(n, t) {
-                    n.setTime(n.getTime() + 1e3 * Math.floor(t))
-                }), (function(n) {
-                    return n.getSeconds()
-                })), Ut.seconds = Ut.second.range, Ut.seconds.utc = Ut.second.utc.range, Ut.minute = Ot((function(n) {
-                    return new jt(6e4 * Math.floor(n / 6e4))
-                }), (function(n, t) {
-                    n.setTime(n.getTime() + 6e4 * Math.floor(t))
-                }), (function(n) {
-                    return n.getMinutes()
-                })), Ut.minutes = Ut.minute.range, Ut.minutes.utc = Ut.minute.utc.range, Ut.hour = Ot((function(n) {
-                    var t = n.getTimezoneOffset() / 60;
-                    return new jt(36e5 * (Math.floor(n / 36e5 - t) + t))
-                }), (function(n, t) {
-                    n.setTime(n.getTime() + 36e5 * Math.floor(t))
-                }), (function(n) {
-                    return n.getHours()
-                })), Ut.hours = Ut.hour.range, Ut.hours.utc = Ut.hour.utc.range, Ut.month = Ot((function(n) {
-                    return (n = Ut.day(n)).setDate(1), n
-                }), (function(n, t) {
-                    n.setMonth(n.getMonth() + t)
-                }), (function(n) {
-                    return n.getMonth()
-                })), Ut.months = Ut.month.range, Ut.months.utc = Ut.month.utc.range;
-                var Za = [1e3, 5e3, 15e3, 3e4, 6e4, 3e5, 9e5, 18e5, 36e5, 108e5, 216e5, 432e5, 864e5, 1728e5, 6048e5, 2592e6, 7776e6, 31536e6],
-                    Va = [
-                        [Ut.second, 1],
-                        [Ut.second, 5],
-                        [Ut.second, 15],
-                        [Ut.second, 30],
-                        [Ut.minute, 1],
-                        [Ut.minute, 5],
-                        [Ut.minute, 15],
-                        [Ut.minute, 30],
-                        [Ut.hour, 1],
-                        [Ut.hour, 3],
-                        [Ut.hour, 6],
-                        [Ut.hour, 12],
-                        [Ut.day, 1],
-                        [Ut.day, 2],
-                        [Ut.week, 1],
-                        [Ut.month, 1],
-                        [Ut.month, 3],
-                        [Ut.year, 1]
-                    ],
-                    Xa = ja.multi([
-                        [".%L", function(n) {
-                            return n.getMilliseconds()
-                        }],
-                        [":%S", function(n) {
-                            return n.getSeconds()
-                        }],
-                        ["%I:%M", function(n) {
-                            return n.getMinutes()
-                        }],
-                        ["%I %p", function(n) {
-                            return n.getHours()
-                        }],
-                        ["%a %d", function(n) {
-                            return n.getDay() && 1 != n.getDate()
-                        }],
-                        ["%b %d", function(n) {
-                            return 1 != n.getDate()
-                        }],
-                        ["%B", function(n) {
-                            return n.getMonth()
-                        }],
-                        ["%Y", Ge]
-                    ]),
-                    $a = {
-                        range: function(n, t, e) {
-                            return u.range(Math.ceil(n / e) * e, +t, e).map(Ya)
-                        },
-                        floor: R,
-                        ceil: R
-                    };
-                Va.year = Ut.year, Ut.scale = function() {
-                    return Ia(u.scale.linear(), Va, Xa)
-                };
-                var Ba = Va.map((function(n) {
-                        return [n[0].utc, n[1]]
-                    })),
-                    Ja = Fa.multi([
-                        [".%L", function(n) {
-                            return n.getUTCMilliseconds()
-                        }],
-                        [":%S", function(n) {
-                            return n.getUTCSeconds()
-                        }],
-                        ["%I:%M", function(n) {
-                            return n.getUTCMinutes()
-                        }],
-                        ["%I %p", function(n) {
-                            return n.getUTCHours()
-                        }],
-                        ["%a %d", function(n) {
-                            return n.getUTCDay() && 1 != n.getUTCDate()
-                        }],
-                        ["%b %d", function(n) {
-                            return 1 != n.getUTCDate()
-                        }],
-                        ["%B", function(n) {
-                            return n.getUTCMonth()
-                        }],
-                        ["%Y", Ge]
-                    ]);
-
-                function Wa(n) {
-                    return JSON.parse(n.responseText)
-                }
-
-                function Ga(n) {
-                    var t = l.createRange();
-                    return t.selectNode(l.body), t.createContextualFragment(n.responseText)
-                }
-                Ba.year = Ut.year.utc, Ut.scale.utc = function() {
-                    return Ia(u.scale.linear(), Ba, Ja)
-                }, u.text = xt((function(n) {
-                    return n.responseText
-                })), u.json = function(n, t) {
-                    return bt(n, "application/json", Wa, t)
-                }, u.html = function(n, t) {
-                    return bt(n, "text/html", Ga, t)
-                }, u.xml = xt((function(n) {
-                    return n.responseXML
-                })), this.d3 = u, void 0 === (i = "function" == typeof(r = u) ? r.call(t, e, t, n) : r) || (n.exports = i)
-            }()
+        function t(n, t, e, r) {
+            var u = t.call(n, e, r),
+                i = a.call(n, u, r),
+                o = c.call(n, u, r) + _l,
+                s = l.call(n, u, r) + _l;
+            return {
+                r: i,
+                a0: o,
+                a1: s,
+                p0: [i * Math.cos(o), i * Math.sin(o)],
+                p1: [i * Math.cos(s), i * Math.sin(s)]
+            }
         }
-    }
-]);
-//# sourceMappingURL=2.js.map
+
+        function e(n, t) {
+            return n.a0 == t.a0 && n.a1 == t.a1
+        }
+
+        function r(n, t, e) {
+            return "A" + n + "," + n + " 0 " + +(e > Ea) + ",1 " + t
+        }
+
+        function u(n, t, e, r) {
+            return "Q 0,0 " + r
+        }
+        var i = mr,
+            o = yr,
+            a = Lo,
+            c = io,
+            l = oo;
+        return n.radius = function(t) {
+            return arguments.length ? (a = kt(t), n) : a
+        }, n.source = function(t) {
+            return arguments.length ? (i = kt(t), n) : i
+        }, n.target = function(t) {
+            return arguments.length ? (o = kt(t), n) : o
+        }, n.startAngle = function(t) {
+            return arguments.length ? (c = kt(t), n) : c
+        }, n.endAngle = function(t) {
+            return arguments.length ? (l = kt(t), n) : l
+        }, n
+    }, Bo.svg.diagonal = function() {
+        function n(n, u) {
+            var i = t.call(this, n, u),
+                o = e.call(this, n, u),
+                a = (i.y + o.y) / 2,
+                c = [i, {
+                    x: i.x,
+                    y: a
+                }, {
+                    x: o.x,
+                    y: a
+                }, o];
+            return c = c.map(r), "M" + c[0] + "C" + c[1] + " " + c[2] + " " + c[3]
+        }
+        var t = mr,
+            e = yr,
+            r = To;
+        return n.source = function(e) {
+            return arguments.length ? (t = kt(e), n) : t
+        }, n.target = function(t) {
+            return arguments.length ? (e = kt(t), n) : e
+        }, n.projection = function(t) {
+            return arguments.length ? (r = t, n) : r
+        }, n
+    }, Bo.svg.diagonal.radial = function() {
+        var n = Bo.svg.diagonal(),
+            t = To,
+            e = n.projection;
+        return n.projection = function(n) {
+            return arguments.length ? e(qo(t = n)) : t
+        }, n
+    }, Bo.svg.symbol = function() {
+        function n(n, r) {
+            return (Al.get(t.call(this, n, r)) || Po)(e.call(this, n, r))
+        }
+        var t = Do,
+            e = Ro;
+        return n.type = function(e) {
+            return arguments.length ? (t = kt(e), n) : t
+        }, n.size = function(t) {
+            return arguments.length ? (e = kt(t), n) : e
+        }, n
+    };
+    var Al = Bo.map({
+        circle: Po,
+        cross: function(n) {
+            var t = Math.sqrt(n / 5) / 2;
+            return "M" + -3 * t + "," + -t + "H" + -t + "V" + -3 * t + "H" + t + "V" + -t + "H" + 3 * t + "V" + t + "H" + t + "V" + 3 * t + "H" + -t + "V" + t + "H" + -3 * t + "Z"
+        },
+        diamond: function(n) {
+            var t = Math.sqrt(n / (2 * Ll)),
+                e = t * Ll;
+            return "M0," + -t + "L" + e + ",0" + " 0," + t + " " + -e + ",0" + "Z"
+        },
+        square: function(n) {
+            var t = Math.sqrt(n) / 2;
+            return "M" + -t + "," + -t + "L" + t + "," + -t + " " + t + "," + t + " " + -t + "," + t + "Z"
+        },
+        "triangle-down": function(n) {
+            var t = Math.sqrt(n / zl),
+                e = t * zl / 2;
+            return "M0," + e + "L" + t + "," + -e + " " + -t + "," + -e + "Z"
+        },
+        "triangle-up": function(n) {
+            var t = Math.sqrt(n / zl),
+                e = t * zl / 2;
+            return "M0," + -e + "L" + t + "," + e + " " + -t + "," + e + "Z"
+        }
+    });
+    Bo.svg.symbolTypes = Al.keys();
+    var Cl, Nl, zl = Math.sqrt(3),
+        Ll = Math.tan(30 * La),
+        Tl = [],
+        ql = 0;
+    Tl.call = ya.call, Tl.empty = ya.empty, Tl.node = ya.node, Tl.size = ya.size, Bo.transition = function(n) {
+        return arguments.length ? Cl ? n.transition() : n : _a.transition()
+    }, Bo.transition.prototype = Tl, Tl.select = function(n) {
+        var t, e, r, u = this.id,
+            i = [];
+        n = k(n);
+        for (var o = -1, a = this.length; ++o < a;) {
+            i.push(t = []);
+            for (var c = this[o], l = -1, s = c.length; ++l < s;)(r = c[l]) && (e = n.call(r, r.__data__, l, o)) ? ("__data__" in r && (e.__data__ = r.__data__), Ho(e, l, u, r.__transition__[u]), t.push(e)) : t.push(null)
+        }
+        return Uo(i, u)
+    }, Tl.selectAll = function(n) {
+        var t, e, r, u, i, o = this.id,
+            a = [];
+        n = E(n);
+        for (var c = -1, l = this.length; ++c < l;)
+            for (var s = this[c], f = -1, h = s.length; ++f < h;)
+                if (r = s[f]) {
+                    i = r.__transition__[o], e = n.call(r, r.__data__, f, c), a.push(t = []);
+                    for (var g = -1, p = e.length; ++g < p;)(u = e[g]) && Ho(u, g, o, i), t.push(u)
+                } return Uo(a, o)
+    }, Tl.filter = function(n) {
+        var t, e, r, u = [];
+        "function" != typeof n && (n = U(n));
+        for (var i = 0, o = this.length; o > i; i++) {
+            u.push(t = []);
+            for (var e = this[i], a = 0, c = e.length; c > a; a++)(r = e[a]) && n.call(r, r.__data__, a, i) && t.push(r)
+        }
+        return Uo(u, this.id)
+    }, Tl.tween = function(n, t) {
+        var e = this.id;
+        return arguments.length < 2 ? this.node().__transition__[e].tween.get(n) : F(this, null == t ? function(t) {
+            t.__transition__[e].tween.remove(n)
+        } : function(r) {
+            r.__transition__[e].tween.set(n, t)
+        })
+    }, Tl.attr = function(n, t) {
+        function e() {
+            this.removeAttribute(a)
+        }
+
+        function r() {
+            this.removeAttributeNS(a.space, a.local)
+        }
+
+        function u(n) {
+            return null == n ? e : (n += "", function() {
+                var t, e = this.getAttribute(a);
+                return e !== n && (t = o(e, n), function(n) {
+                    this.setAttribute(a, t(n))
+                })
+            })
+        }
+
+        function i(n) {
+            return null == n ? r : (n += "", function() {
+                var t, e = this.getAttributeNS(a.space, a.local);
+                return e !== n && (t = o(e, n), function(n) {
+                    this.setAttributeNS(a.space, a.local, t(n))
+                })
+            })
+        }
+        if (arguments.length < 2) {
+            for (t in n) this.attr(t, n[t]);
+            return this
+        }
+        var o = "transform" == n ? Fu : du,
+            a = Bo.ns.qualify(n);
+        return jo(this, "attr." + n, t, a.local ? i : u)
+    }, Tl.attrTween = function(n, t) {
+        function e(n, e) {
+            var r = t.call(this, n, e, this.getAttribute(u));
+            return r && function(n) {
+                this.setAttribute(u, r(n))
+            }
+        }
+
+        function r(n, e) {
+            var r = t.call(this, n, e, this.getAttributeNS(u.space, u.local));
+            return r && function(n) {
+                this.setAttributeNS(u.space, u.local, r(n))
+            }
+        }
+        var u = Bo.ns.qualify(n);
+        return this.tween("attr." + n, u.local ? r : e)
+    }, Tl.style = function(n, t, e) {
+        function r() {
+            this.style.removeProperty(n)
+        }
+
+        function u(t) {
+            return null == t ? r : (t += "", function() {
+                var r, u = Qo.getComputedStyle(this, null).getPropertyValue(n);
+                return u !== t && (r = du(u, t), function(t) {
+                    this.style.setProperty(n, r(t), e)
+                })
+            })
+        }
+        var i = arguments.length;
+        if (3 > i) {
+            if ("string" != typeof n) {
+                2 > i && (t = "");
+                for (e in n) this.style(e, n[e], t);
+                return this
+            }
+            e = ""
+        }
+        return jo(this, "style." + n, t, u)
+    }, Tl.styleTween = function(n, t, e) {
+        function r(r, u) {
+            var i = t.call(this, r, u, Qo.getComputedStyle(this, null).getPropertyValue(n));
+            return i && function(t) {
+                this.style.setProperty(n, i(t), e)
+            }
+        }
+        return arguments.length < 3 && (e = ""), this.tween("style." + n, r)
+    }, Tl.text = function(n) {
+        return jo(this, "text", n, Fo)
+    }, Tl.remove = function() {
+        return this.each("end.transition", function() {
+            var n;
+            this.__transition__.count < 2 && (n = this.parentNode) && n.removeChild(this)
+        })
+    }, Tl.ease = function(n) {
+        var t = this.id;
+        return arguments.length < 1 ? this.node().__transition__[t].ease : ("function" != typeof n && (n = Bo.ease.apply(Bo, arguments)), F(this, function(e) {
+            e.__transition__[t].ease = n
+        }))
+    }, Tl.delay = function(n) {
+        var t = this.id;
+        return arguments.length < 1 ? this.node().__transition__[t].delay : F(this, "function" == typeof n ? function(e, r, u) {
+            e.__transition__[t].delay = +n.call(e, e.__data__, r, u)
+        } : (n = +n, function(e) {
+            e.__transition__[t].delay = n
+        }))
+    }, Tl.duration = function(n) {
+        var t = this.id;
+        return arguments.length < 1 ? this.node().__transition__[t].duration : F(this, "function" == typeof n ? function(e, r, u) {
+            e.__transition__[t].duration = Math.max(1, n.call(e, e.__data__, r, u))
+        } : (n = Math.max(1, n), function(e) {
+            e.__transition__[t].duration = n
+        }))
+    }, Tl.each = function(n, t) {
+        var e = this.id;
+        if (arguments.length < 2) {
+            var r = Nl,
+                u = Cl;
+            Cl = e, F(this, function(t, r, u) {
+                Nl = t.__transition__[e], n.call(t, t.__data__, r, u)
+            }), Nl = r, Cl = u
+        } else F(this, function(r) {
+            var u = r.__transition__[e];
+            (u.event || (u.event = Bo.dispatch("start", "end"))).on(n, t)
+        });
+        return this
+    }, Tl.transition = function() {
+        for (var n, t, e, r, u = this.id, i = ++ql, o = [], a = 0, c = this.length; c > a; a++) {
+            o.push(n = []);
+            for (var t = this[a], l = 0, s = t.length; s > l; l++)(e = t[l]) && (r = Object.create(e.__transition__[u]), r.delay += r.duration, Ho(e, l, i, r)), n.push(e)
+        }
+        return Uo(o, i)
+    }, Bo.svg.axis = function() {
+        function n(n) {
+            n.each(function() {
+                var n, l = Bo.select(this),
+                    s = this.__chart__ || e,
+                    f = this.__chart__ = e.copy(),
+                    h = null == c ? f.ticks ? f.ticks.apply(f, a) : f.domain() : c,
+                    g = null == t ? f.tickFormat ? f.tickFormat.apply(f, a) : Et : t,
+                    p = l.selectAll(".tick").data(h, f),
+                    v = p.enter().insert("g", ".domain").attr("class", "tick").style("opacity", Na),
+                    d = Bo.transition(p.exit()).style("opacity", Na).remove(),
+                    m = Bo.transition(p.order()).style("opacity", 1),
+                    y = Math.max(u, 0) + o,
+                    x = Pi(f),
+                    M = l.selectAll(".domain").data([0]),
+                    _ = (M.enter().append("path").attr("class", "domain"), Bo.transition(M));
+                v.append("line"), v.append("text");
+                var b, w, S, k, E = v.select("line"),
+                    A = m.select("line"),
+                    C = p.select("text").text(g),
+                    N = v.select("text"),
+                    z = m.select("text"),
+                    L = "top" === r || "left" === r ? -1 : 1;
+                if ("bottom" === r || "top" === r ? (n = Oo, b = "x", S = "y", w = "x2", k = "y2", C.attr("dy", 0 > L ? "0em" : ".71em").style("text-anchor", "middle"), _.attr("d", "M" + x[0] + "," + L * i + "V0H" + x[1] + "V" + L * i)) : (n = Yo, b = "y", S = "x", w = "y2", k = "x2", C.attr("dy", ".32em").style("text-anchor", 0 > L ? "end" : "start"), _.attr("d", "M" + L * i + "," + x[0] + "H0V" + x[1] + "H" + L * i)), E.attr(k, L * u), N.attr(S, L * y), A.attr(w, 0).attr(k, L * u), z.attr(b, 0).attr(S, L * y), f.rangeBand) {
+                    var T = f,
+                        q = T.rangeBand() / 2;
+                    s = f = function(n) {
+                        return T(n) + q
+                    }
+                } else s.rangeBand ? s = f : d.call(n, f, s);
+                v.call(n, s, f), m.call(n, f, f)
+            })
+        }
+        var t, e = Bo.scale.linear(),
+            r = Rl,
+            u = 6,
+            i = 6,
+            o = 3,
+            a = [10],
+            c = null;
+        return n.scale = function(t) {
+            return arguments.length ? (e = t, n) : e
+        }, n.orient = function(t) {
+            return arguments.length ? (r = t in Dl ? t + "" : Rl, n) : r
+        }, n.ticks = function() {
+            return arguments.length ? (a = arguments, n) : a
+        }, n.tickValues = function(t) {
+            return arguments.length ? (c = t, n) : c
+        }, n.tickFormat = function(e) {
+            return arguments.length ? (t = e, n) : t
+        }, n.tickSize = function(t) {
+            var e = arguments.length;
+            return e ? (u = +t, i = +arguments[e - 1], n) : u
+        }, n.innerTickSize = function(t) {
+            return arguments.length ? (u = +t, n) : u
+        }, n.outerTickSize = function(t) {
+            return arguments.length ? (i = +t, n) : i
+        }, n.tickPadding = function(t) {
+            return arguments.length ? (o = +t, n) : o
+        }, n.tickSubdivide = function() {
+            return arguments.length && n
+        }, n
+    };
+    var Rl = "bottom",
+        Dl = {
+            top: 1,
+            right: 1,
+            bottom: 1,
+            left: 1
+        };
+    Bo.svg.brush = function() {
+        function n(i) {
+            i.each(function() {
+                var i = Bo.select(this).style("pointer-events", "all").style("-webkit-tap-highlight-color", "rgba(0,0,0,0)").on("mousedown.brush", u).on("touchstart.brush", u),
+                    o = i.selectAll(".background").data([0]);
+                o.enter().append("rect").attr("class", "background").style("visibility", "hidden").style("cursor", "crosshair"), i.selectAll(".extent").data([0]).enter().append("rect").attr("class", "extent").style("cursor", "move");
+                var a = i.selectAll(".resize").data(p, Et);
+                a.exit().remove(), a.enter().append("g").attr("class", function(n) {
+                    return "resize " + n
+                }).style("cursor", function(n) {
+                    return Pl[n]
+                }).append("rect").attr("x", function(n) {
+                    return /[ew]$/.test(n) ? -3 : null
+                }).attr("y", function(n) {
+                    return /^[ns]/.test(n) ? -3 : null
+                }).attr("width", 6).attr("height", 6).style("visibility", "hidden"), a.style("display", n.empty() ? "none" : null);
+                var s, f = Bo.transition(i),
+                    h = Bo.transition(o);
+                c && (s = Pi(c), h.attr("x", s[0]).attr("width", s[1] - s[0]), e(f)), l && (s = Pi(l), h.attr("y", s[0]).attr("height", s[1] - s[0]), r(f)), t(f)
+            })
+        }
+
+        function t(n) {
+            n.selectAll(".resize").attr("transform", function(n) {
+                return "translate(" + s[+/e$/.test(n)] + "," + f[+/^s/.test(n)] + ")"
+            })
+        }
+
+        function e(n) {
+            n.select(".extent").attr("x", s[0]), n.selectAll(".extent,.n>rect,.s>rect").attr("width", s[1] - s[0])
+        }
+
+        function r(n) {
+            n.select(".extent").attr("y", f[0]), n.selectAll(".extent,.e>rect,.w>rect").attr("height", f[1] - f[0])
+        }
+
+        function u() {
+            function u() {
+                32 == Bo.event.keyCode && (C || (y = null, z[0] -= s[1], z[1] -= f[1], C = 2), _())
+            }
+
+            function p() {
+                32 == Bo.event.keyCode && 2 == C && (z[0] += s[1], z[1] += f[1], C = 0, _())
+            }
+
+            function v() {
+                var n = Bo.mouse(M),
+                    u = !1;
+                x && (n[0] += x[0], n[1] += x[1]), C || (Bo.event.altKey ? (y || (y = [(s[0] + s[1]) / 2, (f[0] + f[1]) / 2]), z[0] = s[+(n[0] < y[0])], z[1] = f[+(n[1] < y[1])]) : y = null), E && d(n, c, 0) && (e(S), u = !0), A && d(n, l, 1) && (r(S), u = !0), u && (t(S), w({
+                    type: "brush",
+                    mode: C ? "move" : "resize"
+                }))
+            }
+
+            function d(n, t, e) {
+                var r, u, a = Pi(t),
+                    c = a[0],
+                    l = a[1],
+                    p = z[e],
+                    v = e ? f : s,
+                    d = v[1] - v[0];
+                return C && (c -= p, l -= d + p), r = (e ? g : h) ? Math.max(c, Math.min(l, n[e])) : n[e], C ? u = (r += p) + d : (y && (p = Math.max(c, Math.min(l, 2 * y[e] - r))), r > p ? (u = r, r = p) : u = p), v[0] != r || v[1] != u ? (e ? o = null : i = null, v[0] = r, v[1] = u, !0) : void 0
+            }
+
+            function m() {
+                v(), S.style("pointer-events", "all").selectAll(".resize").style("display", n.empty() ? "none" : null), Bo.select("body").style("cursor", null), L.on("mousemove.brush", null).on("mouseup.brush", null).on("touchmove.brush", null).on("touchend.brush", null).on("keydown.brush", null).on("keyup.brush", null), N(), w({
+                    type: "brushend"
+                })
+            }
+            var y, x, M = this,
+                b = Bo.select(Bo.event.target),
+                w = a.of(M, arguments),
+                S = Bo.select(M),
+                k = b.datum(),
+                E = !/^(n|s)$/.test(k) && c,
+                A = !/^(e|w)$/.test(k) && l,
+                C = b.classed("extent"),
+                N = X(),
+                z = Bo.mouse(M),
+                L = Bo.select(Qo).on("keydown.brush", u).on("keyup.brush", p);
+            if (Bo.event.changedTouches ? L.on("touchmove.brush", v).on("touchend.brush", m) : L.on("mousemove.brush", v).on("mouseup.brush", m), S.interrupt().selectAll("*").interrupt(), C) z[0] = s[0] - z[0], z[1] = f[0] - z[1];
+            else if (k) {
+                var T = +/w$/.test(k),
+                    q = +/^n/.test(k);
+                x = [s[1 - T] - z[0], f[1 - q] - z[1]], z[0] = s[T], z[1] = f[q]
+            } else Bo.event.altKey && (y = z.slice());
+            S.style("pointer-events", "none").selectAll(".resize").style("display", null), Bo.select("body").style("cursor", b.style("cursor")), w({
+                type: "brushstart"
+            }), v()
+        }
+        var i, o, a = w(n, "brushstart", "brush", "brushend"),
+            c = null,
+            l = null,
+            s = [0, 0],
+            f = [0, 0],
+            h = !0,
+            g = !0,
+            p = Ul[0];
+        return n.event = function(n) {
+            n.each(function() {
+                var n = a.of(this, arguments),
+                    t = {
+                        x: s,
+                        y: f,
+                        i: i,
+                        j: o
+                    },
+                    e = this.__chart__ || t;
+                this.__chart__ = t, Cl ? Bo.select(this).transition().each("start.brush", function() {
+                    i = e.i, o = e.j, s = e.x, f = e.y, n({
+                        type: "brushstart"
+                    })
+                }).tween("brush:brush", function() {
+                    var e = mu(s, t.x),
+                        r = mu(f, t.y);
+                    return i = o = null,
+                        function(u) {
+                            s = t.x = e(u), f = t.y = r(u), n({
+                                type: "brush",
+                                mode: "resize"
+                            })
+                        }
+                }).each("end.brush", function() {
+                    i = t.i, o = t.j, n({
+                        type: "brush",
+                        mode: "resize"
+                    }), n({
+                        type: "brushend"
+                    })
+                }) : (n({
+                    type: "brushstart"
+                }), n({
+                    type: "brush",
+                    mode: "resize"
+                }), n({
+                    type: "brushend"
+                }))
+            })
+        }, n.x = function(t) {
+            return arguments.length ? (c = t, p = Ul[!c << 1 | !l], n) : c
+        }, n.y = function(t) {
+            return arguments.length ? (l = t, p = Ul[!c << 1 | !l], n) : l
+        }, n.clamp = function(t) {
+            return arguments.length ? (c && l ? (h = !!t[0], g = !!t[1]) : c ? h = !!t : l && (g = !!t), n) : c && l ? [h, g] : c ? h : l ? g : null
+        }, n.extent = function(t) {
+            var e, r, u, a, h;
+            return arguments.length ? (c && (e = t[0], r = t[1], l && (e = e[0], r = r[0]), i = [e, r], c.invert && (e = c(e), r = c(r)), e > r && (h = e, e = r, r = h), (e != s[0] || r != s[1]) && (s = [e, r])), l && (u = t[0], a = t[1], c && (u = u[1], a = a[1]), o = [u, a], l.invert && (u = l(u), a = l(a)), u > a && (h = u, u = a, a = h), (u != f[0] || a != f[1]) && (f = [u, a])), n) : (c && (i ? (e = i[0], r = i[1]) : (e = s[0], r = s[1], c.invert && (e = c.invert(e), r = c.invert(r)), e > r && (h = e, e = r, r = h))), l && (o ? (u = o[0], a = o[1]) : (u = f[0], a = f[1], l.invert && (u = l.invert(u), a = l.invert(a)), u > a && (h = u, u = a, a = h))), c && l ? [
+                [e, u],
+                [r, a]
+            ] : c ? [e, r] : l && [u, a])
+        }, n.clear = function() {
+            return n.empty() || (s = [0, 0], f = [0, 0], i = o = null), n
+        }, n.empty = function() {
+            return !!c && s[0] == s[1] || !!l && f[0] == f[1]
+        }, Bo.rebind(n, a, "on")
+    };
+    var Pl = {
+            n: "ns-resize",
+            e: "ew-resize",
+            s: "ns-resize",
+            w: "ew-resize",
+            nw: "nwse-resize",
+            ne: "nesw-resize",
+            se: "nwse-resize",
+            sw: "nesw-resize"
+        },
+        Ul = [
+            ["n", "e", "s", "w", "nw", "ne", "se", "sw"],
+            ["e", "w"],
+            ["n", "s"],
+            []
+        ],
+        jl = rc.format = lc.timeFormat,
+        Fl = jl.utc,
+        Hl = Fl("%Y-%m-%dT%H:%M:%S.%LZ");
+    jl.iso = Date.prototype.toISOString && +new Date("2000-01-01T00:00:00.000Z") ? Io : Hl, Io.parse = function(n) {
+        var t = new Date(n);
+        return isNaN(t) ? null : t
+    }, Io.toString = Hl.toString, rc.second = Ft(function(n) {
+        return new uc(1e3 * Math.floor(n / 1e3))
+    }, function(n, t) {
+        n.setTime(n.getTime() + 1e3 * Math.floor(t))
+    }, function(n) {
+        return n.getSeconds()
+    }), rc.seconds = rc.second.range, rc.seconds.utc = rc.second.utc.range, rc.minute = Ft(function(n) {
+        return new uc(6e4 * Math.floor(n / 6e4))
+    }, function(n, t) {
+        n.setTime(n.getTime() + 6e4 * Math.floor(t))
+    }, function(n) {
+        return n.getMinutes()
+    }), rc.minutes = rc.minute.range, rc.minutes.utc = rc.minute.utc.range, rc.hour = Ft(function(n) {
+        var t = n.getTimezoneOffset() / 60;
+        return new uc(36e5 * (Math.floor(n / 36e5 - t) + t))
+    }, function(n, t) {
+        n.setTime(n.getTime() + 36e5 * Math.floor(t))
+    }, function(n) {
+        return n.getHours()
+    }), rc.hours = rc.hour.range, rc.hours.utc = rc.hour.utc.range, rc.month = Ft(function(n) {
+        return n = rc.day(n), n.setDate(1), n
+    }, function(n, t) {
+        n.setMonth(n.getMonth() + t)
+    }, function(n) {
+        return n.getMonth()
+    }), rc.months = rc.month.range, rc.months.utc = rc.month.utc.range;
+    var Ol = [1e3, 5e3, 15e3, 3e4, 6e4, 3e5, 9e5, 18e5, 36e5, 108e5, 216e5, 432e5, 864e5, 1728e5, 6048e5, 2592e6, 7776e6, 31536e6],
+        Yl = [
+            [rc.second, 1],
+            [rc.second, 5],
+            [rc.second, 15],
+            [rc.second, 30],
+            [rc.minute, 1],
+            [rc.minute, 5],
+            [rc.minute, 15],
+            [rc.minute, 30],
+            [rc.hour, 1],
+            [rc.hour, 3],
+            [rc.hour, 6],
+            [rc.hour, 12],
+            [rc.day, 1],
+            [rc.day, 2],
+            [rc.week, 1],
+            [rc.month, 1],
+            [rc.month, 3],
+            [rc.year, 1]
+        ],
+        Il = jl.multi([
+            [".%L", function(n) {
+                return n.getMilliseconds()
+            }],
+            [":%S", function(n) {
+                return n.getSeconds()
+            }],
+            ["%I:%M", function(n) {
+                return n.getMinutes()
+            }],
+            ["%I %p", function(n) {
+                return n.getHours()
+            }],
+            ["%a %d", function(n) {
+                return n.getDay() && 1 != n.getDate()
+            }],
+            ["%b %d", function(n) {
+                return 1 != n.getDate()
+            }],
+            ["%B", function(n) {
+                return n.getMonth()
+            }],
+            ["%Y", Ae]
+        ]),
+        Zl = {
+            range: function(n, t, e) {
+                return Bo.range(Math.ceil(n / e) * e, +t, e).map(Vo)
+            },
+            floor: Et,
+            ceil: Et
+        };
+    Yl.year = rc.year, rc.scale = function() {
+        return Zo(Bo.scale.linear(), Yl, Il)
+    };
+    var Vl = Yl.map(function(n) {
+            return [n[0].utc, n[1]]
+        }),
+        Xl = Fl.multi([
+            [".%L", function(n) {
+                return n.getUTCMilliseconds()
+            }],
+            [":%S", function(n) {
+                return n.getUTCSeconds()
+            }],
+            ["%I:%M", function(n) {
+                return n.getUTCMinutes()
+            }],
+            ["%I %p", function(n) {
+                return n.getUTCHours()
+            }],
+            ["%a %d", function(n) {
+                return n.getUTCDay() && 1 != n.getUTCDate()
+            }],
+            ["%b %d", function(n) {
+                return 1 != n.getUTCDate()
+            }],
+            ["%B", function(n) {
+                return n.getUTCMonth()
+            }],
+            ["%Y", Ae]
+        ]);
+    Vl.year = rc.year.utc, rc.scale.utc = function() {
+        return Zo(Bo.scale.linear(), Vl, Xl)
+    }, Bo.text = At(function(n) {
+        return n.responseText
+    }), Bo.json = function(n, t) {
+        return Ct(n, "application/json", Xo, t)
+    }, Bo.html = function(n, t) {
+        return Ct(n, "text/html", $o, t)
+    }, Bo.xml = At(function(n) {
+        return n.responseXML
+    }), "function" == typeof define && define.amd ? define(Bo) : "object" == typeof module && module.exports && (module.exports = Bo), this.d3 = Bo
+}();
```

### Comparing `buildbot-www-3.8.0/buildbot_www/static/img/favicon.ico` & `buildbot-www-v0.9.0b9/buildbot_www/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `buildbot-www-3.8.0/buildbot_www/static/img/nobody.png` & `buildbot-www-v0.9.0b9/buildbot_www/static/img/nobody.png`

 * *Files identical despite different names*

### Comparing `buildbot-www-3.8.0/buildbot_www/static/index.html` & `buildbot-www-v0.9.0b9/buildbot_www/static/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html class="no-js" ng-app="app" xmlns:ng="http://angularjs.org" xmlns:app="ignored"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"></head><title window-title>Buildbot</title><meta name="description" content="Buildbot web UI"><meta name="viewport" content="initial-scale=1, minimum-scale=1, user-scalable=no, maximum-scale=1, width=device-width"><link href="styles.css" rel="stylesheet"><link id="bbicon" href="img/icon.png" rel="icon"><link href="img/icon.svg" title="Buildbot" rel="fluid-icon"><div id="outdated"></div><body ng-cloak><gl-page-with-sidebar><gl-topbar><gl-topbar-contextual-actions></gl-topbar-contextual-actions><loginbar></loginbar></gl-topbar><connectionstatus></connectionstatus><ui-view></ui-view></gl-page-with-sidebar></body><script src="browser-warning.js"></script><link href="browser-warning.css" rel="stylesheet"><script src="browser-warning-list.js"></script><script>window.T =  {{ custom_templates | tojson }};</script><script src="scripts.js?_1681694432577"></script>{% for app in config.plugins -%}<script src="{{app}}/scripts.js?_1681694432577"></script><link href="{{app}}/styles.css?_1681694432577" rel="stylesheet"><script>angular.module('app').requires.push('{{app}}')</script>{% endfor %}<script>angular.module("buildbot_config", []).constant("config", {{configjson|safe}})</script></html>
+<!DOCTYPE html><html xmlns:ng="http://angularjs.org" xmlns:app="ignored" class="no-js"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"></head><title>Buildbot</title><meta name="description" content="Buildbot web UI"><meta name="viewport" content="initial-scale=1, minimum-scale=1, user-scalable=no, maximum-scale=1, width=device-width"><link rel="stylesheet" href="styles.css"><link rel="icon" href="img/favicon.ico"><body ng-cloak ng-app="app"><gl-page-with-sidebar><gl-topbar><gl-topbar-contextual-actions></gl-topbar-contextual-actions><loginbar></loginbar></gl-topbar><connectionstatus></connectionstatus><ui-view></ui-view></gl-page-with-sidebar></body><script src="scripts.js?_1462994118189"></script>{% for app in config.plugins -%}<script src="{{app}}/scripts.js"></script><link rel="stylesheet" href="{{app}}/styles.css"><script>angular.module('app').requires.push('{{app}}')</script>{% endfor %}<script>angular.module("app").constant("config", {{configjson|safe}})</script></html>
```

### Comparing `buildbot-www-3.8.0/setup.py` & `buildbot-www-v0.9.0b9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,39 +13,36 @@
 # this program; if not, write to the Free Software Foundation, Inc., 51
 # Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 #
 # Copyright Buildbot Team Members
 
 try:
     from buildbot_pkg import setup_www_plugin
+    import mock  # noqa
+    import buildbot  # noqa
 except ImportError:
     import sys
-    print('Please install buildbot_pkg module in order to install that '
-          'package, or use the pre-build .whl modules available on pypi',
-          file=sys.stderr)
+    print >> sys.stderr, "Please install buildbot, buildbot_pkg, and mock modules in order to install that package, or use the pre-build .whl modules available on pypi"
     sys.exit(1)
 
 setup_www_plugin(
     name='buildbot-www',
     description='Buildbot UI',
     author=u'Pierre Tardy',
     author_email=u'tardyp@gmail.com',
-    setup_requires=['buildbot_pkg'],
-    install_requires=['buildbot'],
+    setup_requires=['buildbot', 'buildbot_pkg', 'mock'],
     url='http://buildbot.net/',
+    license='GNU GPL',
     packages=['buildbot_www'],
     package_data={
         '': [
             'VERSION',
             'static/*',
             'static/img/*',
             'static/fonts/*',
         ]
     },
     entry_points="""
         [buildbot.www]
         base = buildbot_www:ep
-    """,
-    classifiers=[
-        'License :: OSI Approved :: GNU General Public License v2 (GPLv2)'
-    ],
+    """
 )
```

