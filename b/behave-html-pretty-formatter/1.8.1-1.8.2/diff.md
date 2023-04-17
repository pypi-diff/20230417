# Comparing `tmp/behave-html-pretty-formatter-1.8.1.tar.gz` & `tmp/behave-html-pretty-formatter-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behave-html-pretty-formatter-1.8.1.tar", last modified: Mon Mar  6 08:21:52 2023, max compression
+gzip compressed data, was "behave-html-pretty-formatter-1.8.2.tar", last modified: Mon Apr 17 09:12:31 2023, max compression
```

## Comparing `behave-html-pretty-formatter-1.8.1.tar` & `behave-html-pretty-formatter-1.8.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 08:21:52.282687 behave-html-pretty-formatter-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-06 08:21:33.000000 behave-html-pretty-formatter-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-06 08:21:33.000000 behave-html-pretty-formatter-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-03-06 08:21:52.282687 behave-html-pretty-formatter-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-03-06 08:21:33.000000 behave-html-pretty-formatter-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 08:21:52.282687 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-06 08:21:33.000000 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-03-06 08:21:33.000000 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/behave.css
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-03-06 08:21:33.000000 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/behave.js
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-03-06 08:21:33.000000 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/behave.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-03-06 08:21:33.000000 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/behave.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    39173 2023-03-06 08:21:33.000000 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/html_pretty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 08:21:52.282687 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-03-06 08:21:52.000000 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-06 08:21:52.000000 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 08:21:52.000000 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-06 08:21:52.000000 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-06 08:21:52.000000 behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-06 08:21:33.000000 behave-html-pretty-formatter-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 08:21:52.282687 behave-html-pretty-formatter-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-03-06 08:21:33.000000 behave-html-pretty-formatter-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:12:31.813775 behave-html-pretty-formatter-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-04-17 09:12:31.813775 behave-html-pretty-formatter-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:12:31.813775 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39492 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/html_pretty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:12:31.813775 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-04-17 09:12:31.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-17 09:12:31.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:12:31.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 09:12:31.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 09:12:31.000000 behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:12:31.813775 behave-html-pretty-formatter-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-17 09:12:14.000000 behave-html-pretty-formatter-1.8.2/setup.py
```

### Comparing `behave-html-pretty-formatter-1.8.1/LICENSE` & `behave-html-pretty-formatter-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.8.1/PKG-INFO` & `behave-html-pretty-formatter-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behave-html-pretty-formatter
-Version: 1.8.1
+Version: 1.8.2
 Summary: Pretty HTML Formatter for Behave
 Home-page: https://github.com/behave-contrib/behave-html-pretty-formatter
 Author: Michal Odehnal
 Author-email: modehnal@redhat.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `behave-html-pretty-formatter-1.8.1/README.md` & `behave-html-pretty-formatter-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/behave.css` & `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.css`

 * *Files 1% similar despite different names*

```diff
@@ -371,14 +371,19 @@
 }
 
 .step-capsule.commentary {
   background-color: var(--commentary-bg);
   margin-left: 1rem;
 }
 
+.step-capsule.description {
+  background-color: var(--commentary-bg);
+  margin-left: 0rem;
+}
+
 .step-capsule.contrast {
   background-color: rgb(36, 35, 35);
   color: #fff;
   font-size: 1.25rem;
   border: none;
 }
 
@@ -569,14 +574,18 @@
   margin-left: auto;
 }
 
 .margin-top {
   margin-top: 15px;
 }
 
+.no-margin-top {
+  margin-top: 0px;
+}
+
 .margin-bottom {
   margin-bottom: 15px;
 }
 
 /* SMALL SCREEN */
 /* Should be at bottom, to override rules above */
 @media only screen and (max-width: 750px) {
```

### Comparing `behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/behave.js` & `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.js`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/behave.min.css` & `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.min.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-@charset "utf-8"; :root{--body-color:#333;--body-bg:#fff;--strong-color:#000;--feature-bg:#eee;--feature-color:#777;--duration-color:#313131;--summary-passed:#4f8a10;--summary-passed-border:#4f8a10;--summary-failed:#d8000c;--summary-failed-border:#d8000c;--summary-undefined:#945901;--summary-undefined-border:#ffdf61;--summary-skipped:#76adff;--summary-skipped-border:#76adff;--passed-bg:#dff2bf;--passed-step-bg:#c6dba3;--passed-border:#b4cc8c;--failed-bg:#f5c9cd;--failed-step-bg:#ea868f;--failed-border:#dd7a82;--undefined-bg:#ffdf61;--undefined-step-bg:#f1cb32;--undefined-border:#917400;--skipped-bg:#eef5ff;--skipped-step-bg:#cfe2ff;--skipped-border:#b8c9e4;--commentary-bg:#b9b9b9;--table-bg-odd:#fff;--table-bg-even:#eee;--button-bg:#666;--button-color:#eee;--button-bg-active:#898989;--button-color-active:#fff}@media (prefers-color-scheme:dark){:root{--body-color:#ddd;--body-bg:#000;--strong-color:#fff;--feature-bg:#222;--feature-color:#aaa;--duration-color:#cecece;--passed-bg:#42630a;--passed-step-bg:#697e41;--passed-border:#91a86b;--failed-bg:#69272d;--failed-step-bg:#a8666c;--failed-border:#df888f;--undefined-bg:#665a2a;--undefined-step-bg:#b6940d;--undefined-border:#dbb20e;--skipped-bg:#345381;--skipped-step-bg:#3d659e;--skipped-border:#6981a8;--commentary-bg:#5c5c5c;--table-bg-odd:#555;--table-bg-even:#444;--button-bg:#555;--button-color:#cdcdcd;--button-bg-active:#898989;--button-color-active:#fff}}html,body{font-family:Arial,Helvetica,sans-serif;font-size:1rem;margin:0;padding:0;color:var(--body-color);background:var(--body-bg)}body{padding:1rem 1rem;font-size:.85rem}pre,pre *{margin:0}.embed_button::after,.scenario-name::after{position:absolute;top:-0.5em;left:-0.2em;content:"\2304";font-size:1.8em;transition:all .2s linear}.embed_button.collapse::after,.collapse .scenario-name::after{top:-0.29em;left:-0.5em;transform:rotate(-90deg);-moz-transform:rotate(-90deg);-webkit-transform:rotate(-90deg);-ms-transform:rotate(-90deg);-o-transform:rotate(-90deg)}.embed_button,.scenario-name{padding-left:1.2em;position:relative}.feature-title{font-size:1rem;display:flex;flex-wrap:wrap;align-items:center;background-color:var(--feature-bg);color:var(--feature-color);padding:.5em 1rem;margin-bottom:5px}.feature-icon{height:1.2em;display:inline-block;margin-right:.3em;text-align:center;vertical-align:middle}.feature-icon.contrast{display:none}.feature-title.contrast{font-weight:bold;font-size:1.25rem;background-color:#000;color:#fff}.feature-summary-commentary{border-left:.4rem solid var(--feature-color);background-color:var(--commentary-bg);color:var(--strong-color);word-wrap:break-word;max-width:40%;margin-right:1rem;margin-top:.2rem;margin-left:.2rem;padding:.5rem;white-space:pre-wrap}.feature-summary-commentary.contrast{background-color:#242323;color:#f8f8f8;font-size:1rem}.feature-summary-container{display:flex;flex-wrap:wrap;padding:5px;padding-right:1rem;margin-bottom:5px;background-color:var(--feature-bg);color:var(--feature-color);justify-content:start;font-size:.8rem}.feature-summary-container.contrast{background-color:#000;color:#f8f8f8;font-size:1rem}.feature-additional-info-container{padding:5px;background-color:var(--feature-bg);color:var(--feature-color);justify-content:start;font-size:.8rem;flex-basis:100%}.contrast .feature-additional-info-container{background-color:#000;color:#f8f8f8;font-size:1rem}.feature-summary-stats{margin-top:.2em}.feature-summary-stats .button{padding-left:.4em;padding-right:.4em;padding-top:.1em;padding-bottom:.1em;margin-bottom:.1em}.feature-summary-row{color:var(--feature-color);border-left:.4rem solid var(--feature-color);padding-left:.5rem;padding-top:.1em;padding-bottom:.1em;margin-bottom:.1em}.feature-summary-row.passed{color:var(--summary-passed);border-left:.4rem solid var(--summary-passed-border)}.feature-summary-row.failed{color:var(--summary-failed);border-left:.4rem solid var(--summary-failed-border)}.feature-summary-row.undefined{color:var(--summary-undefined);border-left:.4rem solid var(--summary-undefined-border)}.feature-summary-row.skipped{color:var(--summary-skipped);border-left:.4rem solid var(--summary-skipped-border)}.feature-summary-row.contrast{color:#f8f8f8;border-left:.4rem solid #f8f8f8}.feature-container{margin-bottom:2rem}.scenario-capsule{padding:1rem;padding-right:.5rem;padding-top:.3rem;margin-bottom:1rem;color:var(--strong-color)}.scenario-header{padding:1rem;padding-bottom:0;margin-top:0;margin-bottom:0;color:var(--strong-color)}.scenario-capsule:last-child{border:0}.scenario-capsule{background-color:var(--feature-bg)}.scenario-header.passed{background-color:var(--passed-step-bg)}.scenario-header.failed{background-color:var(--failed-step-bg)}.scenario-header.undefined{background-color:var(--undefined-step-bg)}.scenario-header.skipped{background-color:var(--skipped-step-bg)}.scenario-header.contrast,.scenario-capsule.contrast{background-color:#000;color:#fff}.scenario-info{display:flex;flex-wrap:wrap;font-size:1.25rem}.scenario-name{cursor:pointer;font-weight:bold;padding-bottom:.5em}.scenario-duration{align-self:center;margin-left:auto;font-size:.75rem;font-style:italic;padding:0 .5em .5em 0}.scenario-duration.contrast{font-size:1.25rem;color:#fff}.scenario-tags{color:var(--body-color);font-weight:bold;font-size:.75rem;margin:.1rem .8em .5rem 0;display:inline-block}.scenario-tags.contrast{color:white;font-weight:bold;font-size:1rem;margin:.1rem 1em .5rem 0}.step-capsule{margin:2px 0 2px 2px;padding:.5rem;color:var(--strong-color);display:flex;flex-wrap:wrap;font-size:.75rem}.step-capsule.passed{background-color:var(--passed-step-bg);border:1px solid var(--passed-border)}.step-capsule.failed{background-color:var(--failed-step-bg);border:1px solid var(--failed-border)}.step-capsule.undefined{background-color:var(--undefined-step-bg);border:1px solid var(--undefined-step-bg)}.step-capsule.skipped{background-color:var(--skipped-step-bg);border:1px solid var(--skipped-border)}.step-capsule.commentary{background-color:var(--commentary-bg);margin-left:1rem}.step-capsule.contrast{background-color:#242323;color:#fff;font-size:1.25rem;border:none}.step-status{display:none;padding:0 1rem 0 0;font-weight:bold;font-size:1.25rem}.step-decorator{padding:0;padding-right:1.5rem}.step-duration{color:var(--duration-color);font-style:italic;padding:0;padding-right:1.5rem}.step-duration.contrast{color:#f8f8f8}.messages{margin:0 0 4px 1em}.scenario-capsule .messages:last-child{border-bottom:1px dashed var(--strong-color)}.scenario-capsule .messages.contrast:last-child{border-bottom:1px dashed #fff}.embed-capsule{margin:.5em 0}.embed_content{white-space:pre-wrap;word-wrap:break-word;font-size:12px;margin:.5rem}.embed_button{cursor:pointer;margin:0 1rem .5em 0;text-decoration:underline;color:var(--strong-color);font-size:12px;width:max-content}.embed_button.contrast{color:#fff;font-size:20px}th,td{padding:6px}thead{background-color:#333;color:#fff;cursor:pointer}table{color:var(--body-color);margin:2px 1em 4px 1em;border-collapse:collapse;border:1px solid #000;vertical-align:middle}table.contrast{font-size:1rem}table tbody tr:nth-child(odd){background-color:var(--table-bg-odd)}table tbody tr:nth-child(even){background-color:var(--table-bg-even)}table.contrast tbody tr{background-color:#fff;color:#000;border:1px solid #000}img,video{max-width:100%;max-height:100%}a{color:inherit;text-decoration:none}a:hover{text-decoration:underline;text-decoration-color:var(--strong-color)}.contrast a:hover{color:grey;text-decoration:underline;text-decoration-color:grey}.scenario-header.collapse .scenario-tags,.scenario-capsule.collapse{display:none}.scenario-header.collapse{padding:.5rem 1rem 0 1rem;margin-bottom:1rem}.button{display:inline-block;color:var(--button-color);background-color:var(--button-bg);border-radius:.2em;font-weight:bold;text-decoration:none;padding:.5em .9em;text-align:center;cursor:pointer}.button:hover{text-decoration:none;color:var(--button-color-active);background-color:var(--button-bg-active)}.contrast .button{color:#111;background-color:#eee}.contrast .button:hover{text-decoration:none}.display-flex{display:flex}.display-block{display:block}.display-inline{display:inline}.display-block.display-inline{display:inline-block}.flex-gap{column-gap:1em;row-gap:2px}.flex-left-space{margin-left:auto}.margin-top{margin-top:15px}.margin-bottom{margin-bottom:15px}@media only screen and (max-width:750px){.feature-title{flex-direction:column}.feature-summary-container{margin-left:0;margin-top:.25rem;font-size:1rem;display:block}.feature-additional-info-container{margin-left:0;margin-top:.25rem;font-size:1rem}.feature-summary-commentary{max-width:100%;margin-right:0}.flex-left-space{margin-left:initial}.feature-summary-stats{margin-left:.2rem}.scenario-capsule{padding-right:0}}
+@charset "utf-8"; :root{--body-color:#333;--body-bg:#fff;--strong-color:#000;--feature-bg:#eee;--feature-color:#777;--duration-color:#313131;--summary-passed:#4f8a10;--summary-passed-border:#4f8a10;--summary-failed:#d8000c;--summary-failed-border:#d8000c;--summary-undefined:#945901;--summary-undefined-border:#ffdf61;--summary-skipped:#76adff;--summary-skipped-border:#76adff;--passed-bg:#dff2bf;--passed-step-bg:#c6dba3;--passed-border:#b4cc8c;--failed-bg:#f5c9cd;--failed-step-bg:#ea868f;--failed-border:#dd7a82;--undefined-bg:#ffdf61;--undefined-step-bg:#f1cb32;--undefined-border:#917400;--skipped-bg:#eef5ff;--skipped-step-bg:#cfe2ff;--skipped-border:#b8c9e4;--commentary-bg:#b9b9b9;--table-bg-odd:#fff;--table-bg-even:#eee;--button-bg:#666;--button-color:#eee;--button-bg-active:#898989;--button-color-active:#fff}@media (prefers-color-scheme:dark){:root{--body-color:#ddd;--body-bg:#000;--strong-color:#fff;--feature-bg:#222;--feature-color:#aaa;--duration-color:#cecece;--passed-bg:#42630a;--passed-step-bg:#697e41;--passed-border:#91a86b;--failed-bg:#69272d;--failed-step-bg:#a8666c;--failed-border:#df888f;--undefined-bg:#665a2a;--undefined-step-bg:#b6940d;--undefined-border:#dbb20e;--skipped-bg:#345381;--skipped-step-bg:#3d659e;--skipped-border:#6981a8;--commentary-bg:#5c5c5c;--table-bg-odd:#555;--table-bg-even:#444;--button-bg:#555;--button-color:#cdcdcd;--button-bg-active:#898989;--button-color-active:#fff}}html,body{font-family:Arial,Helvetica,sans-serif;font-size:1rem;margin:0;padding:0;color:var(--body-color);background:var(--body-bg)}body{padding:1rem 1rem;font-size:.85rem}pre,pre *{margin:0}.embed_button::after,.scenario-name::after{position:absolute;top:-0.5em;left:-0.2em;content:"\2304";font-size:1.8em;transition:all .2s linear}.embed_button.collapse::after,.collapse .scenario-name::after{top:-0.29em;left:-0.5em;transform:rotate(-90deg);-moz-transform:rotate(-90deg);-webkit-transform:rotate(-90deg);-ms-transform:rotate(-90deg);-o-transform:rotate(-90deg)}.embed_button,.scenario-name{padding-left:1.2em;position:relative}.feature-title{font-size:1rem;display:flex;flex-wrap:wrap;align-items:center;background-color:var(--feature-bg);color:var(--feature-color);padding:.5em 1rem;margin-bottom:5px}.feature-icon{height:1.2em;display:inline-block;margin-right:.3em;text-align:center;vertical-align:middle}.feature-icon.contrast{display:none}.feature-title.contrast{font-weight:bold;font-size:1.25rem;background-color:#000;color:#fff}.feature-summary-commentary{border-left:.4rem solid var(--feature-color);background-color:var(--commentary-bg);color:var(--strong-color);word-wrap:break-word;max-width:40%;margin-right:1rem;margin-top:.2rem;margin-left:.2rem;padding:.5rem;white-space:pre-wrap}.feature-summary-commentary.contrast{background-color:#242323;color:#f8f8f8;font-size:1rem}.feature-summary-container{display:flex;flex-wrap:wrap;padding:5px;padding-right:1rem;margin-bottom:5px;background-color:var(--feature-bg);color:var(--feature-color);justify-content:start;font-size:.8rem}.feature-summary-container.contrast{background-color:#000;color:#f8f8f8;font-size:1rem}.feature-additional-info-container{padding:5px;background-color:var(--feature-bg);color:var(--feature-color);justify-content:start;font-size:.8rem;flex-basis:100%}.contrast .feature-additional-info-container{background-color:#000;color:#f8f8f8;font-size:1rem}.feature-summary-stats{margin-top:.2em}.feature-summary-stats .button{padding-left:.4em;padding-right:.4em;padding-top:.1em;padding-bottom:.1em;margin-bottom:.1em}.feature-summary-row{color:var(--feature-color);border-left:.4rem solid var(--feature-color);padding-left:.5rem;padding-top:.1em;padding-bottom:.1em;margin-bottom:.1em}.feature-summary-row.passed{color:var(--summary-passed);border-left:.4rem solid var(--summary-passed-border)}.feature-summary-row.failed{color:var(--summary-failed);border-left:.4rem solid var(--summary-failed-border)}.feature-summary-row.undefined{color:var(--summary-undefined);border-left:.4rem solid var(--summary-undefined-border)}.feature-summary-row.skipped{color:var(--summary-skipped);border-left:.4rem solid var(--summary-skipped-border)}.feature-summary-row.contrast{color:#f8f8f8;border-left:.4rem solid #f8f8f8}.feature-container{margin-bottom:2rem}.scenario-capsule{padding:1rem;padding-right:.5rem;padding-top:.3rem;margin-bottom:1rem;color:var(--strong-color)}.scenario-header{padding:1rem;padding-bottom:0;margin-top:0;margin-bottom:0;color:var(--strong-color)}.scenario-capsule:last-child{border:0}.scenario-capsule{background-color:var(--feature-bg)}.scenario-header.passed{background-color:var(--passed-step-bg)}.scenario-header.failed{background-color:var(--failed-step-bg)}.scenario-header.undefined{background-color:var(--undefined-step-bg)}.scenario-header.skipped{background-color:var(--skipped-step-bg)}.scenario-header.contrast,.scenario-capsule.contrast{background-color:#000;color:#fff}.scenario-info{display:flex;flex-wrap:wrap;font-size:1.25rem}.scenario-name{cursor:pointer;font-weight:bold;padding-bottom:.5em}.scenario-duration{align-self:center;margin-left:auto;font-size:.75rem;font-style:italic;padding:0 .5em .5em 0}.scenario-duration.contrast{font-size:1.25rem;color:#fff}.scenario-tags{color:var(--body-color);font-weight:bold;font-size:.75rem;margin:.1rem .8em .5rem 0;display:inline-block}.scenario-tags.contrast{color:white;font-weight:bold;font-size:1rem;margin:.1rem 1em .5rem 0}.step-capsule{margin:2px 0 2px 2px;padding:.5rem;color:var(--strong-color);display:flex;flex-wrap:wrap;font-size:.75rem}.step-capsule.passed{background-color:var(--passed-step-bg);border:1px solid var(--passed-border)}.step-capsule.failed{background-color:var(--failed-step-bg);border:1px solid var(--failed-border)}.step-capsule.undefined{background-color:var(--undefined-step-bg);border:1px solid var(--undefined-step-bg)}.step-capsule.skipped{background-color:var(--skipped-step-bg);border:1px solid var(--skipped-border)}.step-capsule.commentary{background-color:var(--commentary-bg);margin-left:1rem}.step-capsule.description{background-color:var(--commentary-bg);margin-left:0}.step-capsule.contrast{background-color:#242323;color:#fff;font-size:1.25rem;border:none}.step-status{display:none;padding:0 1rem 0 0;font-weight:bold;font-size:1.25rem}.step-decorator{padding:0;padding-right:1.5rem}.step-duration{color:var(--duration-color);font-style:italic;padding:0;padding-right:1.5rem}.step-duration.contrast{color:#f8f8f8}.messages{margin:0 0 4px 1em}.scenario-capsule .messages:last-child{border-bottom:1px dashed var(--strong-color)}.scenario-capsule .messages.contrast:last-child{border-bottom:1px dashed #fff}.embed-capsule{margin:.5em 0}.embed_content{white-space:pre-wrap;word-wrap:break-word;font-size:12px;margin:.5rem}.embed_button{cursor:pointer;margin:0 1rem .5em 0;text-decoration:underline;color:var(--strong-color);font-size:12px;width:max-content}.embed_button.contrast{color:#fff;font-size:20px}th,td{padding:6px}thead{background-color:#333;color:#fff;cursor:pointer}table{color:var(--body-color);margin:2px 1em 4px 1em;border-collapse:collapse;border:1px solid #000;vertical-align:middle}table.contrast{font-size:1rem}table tbody tr:nth-child(odd){background-color:var(--table-bg-odd)}table tbody tr:nth-child(even){background-color:var(--table-bg-even)}table.contrast tbody tr{background-color:#fff;color:#000;border:1px solid #000}img,video{max-width:100%;max-height:100%}a{color:inherit;text-decoration:none}a:hover{text-decoration:underline;text-decoration-color:var(--strong-color)}.contrast a:hover{color:grey;text-decoration:underline;text-decoration-color:grey}.scenario-header.collapse .scenario-tags,.scenario-capsule.collapse{display:none}.scenario-header.collapse{padding:.5rem 1rem 0 1rem;margin-bottom:1rem}.button{display:inline-block;color:var(--button-color);background-color:var(--button-bg);border-radius:.2em;font-weight:bold;text-decoration:none;padding:.5em .9em;text-align:center;cursor:pointer}.button:hover{text-decoration:none;color:var(--button-color-active);background-color:var(--button-bg-active)}.contrast .button{color:#111;background-color:#eee}.contrast .button:hover{text-decoration:none}.display-flex{display:flex}.display-block{display:block}.display-inline{display:inline}.display-block.display-inline{display:inline-block}.flex-gap{column-gap:1em;row-gap:2px}.flex-left-space{margin-left:auto}.margin-top{margin-top:15px}.no-margin-top{margin-top:0}.margin-bottom{margin-bottom:15px}@media only screen and (max-width:750px){.feature-title{flex-direction:column}.feature-summary-container{margin-left:0;margin-top:.25rem;font-size:1rem;display:block}.feature-additional-info-container{margin-left:0;margin-top:.25rem;font-size:1rem}.feature-summary-commentary{max-width:100%;margin-right:0}.flex-left-space{margin-left:initial}.feature-summary-stats{margin-left:.2rem}.scenario-capsule{padding-right:0}}
```

### Comparing `behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/behave.min.js` & `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/behave.min.js`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter/html_pretty.py` & `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter/html_pretty.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,14 +499,22 @@
 
                 div(f"Scenario duration: {self.duration:.2f}s", cls="scenario-duration")
 
         with div(
             cls=f"scenario-capsule {self.status.name}",
             id=f"f{self.feature.counter}-s{self.counter}-c",
         ):
+            # add scenario description as "commentary":
+            scenario_description = "\n".join(self._scenario.description)
+            if scenario_description:
+                pre(
+                    f"{scenario_description}",
+                    cls="step-capsule description no-margin-top",
+                )
+
             steps = self.steps
             if self.pseudo_steps:
                 steps = [self.pseudo_steps[0]] + steps + [self.pseudo_steps[1]]
             for step in steps:
                 step.generate_step(formatter, self.status)
```

### Comparing `behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter.egg-info/PKG-INFO` & `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behave-html-pretty-formatter
-Version: 1.8.1
+Version: 1.8.2
 Summary: Pretty HTML Formatter for Behave
 Home-page: https://github.com/behave-contrib/behave-html-pretty-formatter
 Author: Michal Odehnal
 Author-email: modehnal@redhat.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `behave-html-pretty-formatter-1.8.1/behave_html_pretty_formatter.egg-info/SOURCES.txt` & `behave-html-pretty-formatter-1.8.2/behave_html_pretty_formatter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `behave-html-pretty-formatter-1.8.1/setup.py` & `behave-html-pretty-formatter-1.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Return the content of a file."""
     with open(filename, "r", encoding="utf-8") as file:
         return file.read()
 
 
 setuptools.setup(
     name="behave-html-pretty-formatter",
-    version="1.8.1",
+    version="1.8.2",
     author="Michal Odehnal",
     author_email="modehnal@redhat.com",
     description="""
 Pretty HTML Formatter for Behave
 
 Authors:
 Michal Odehnal <modehnal@redhat.com>,
```

