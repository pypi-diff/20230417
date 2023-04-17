# Comparing `tmp/onepasswd-0.2.4rc1.tar.gz` & `tmp/onepasswd-0.2.4rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onepasswd-0.2.4rc1.tar", last modified: Thu Apr  6 17:59:23 2023, max compression
+gzip compressed data, was "onepasswd-0.2.4rc2.tar", last modified: Mon Apr 17 04:41:31 2023, max compression
```

## Comparing `onepasswd-0.2.4rc1.tar` & `onepasswd-0.2.4rc2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:59:23.240979 onepasswd-0.2.4rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:59:23.228979 onepasswd-0.2.4rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:59:23.232979 onepasswd-0.2.4rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-06 17:59:23.240979 onepasswd-0.2.4rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:59:23.232979 onepasswd-0.2.4rc1/onepasswd/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/ltlog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5231 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/onepasswd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:59:23.236979 onepasswd-0.2.4rc1/onepasswd/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:59:23.236979 onepasswd-0.2.4rc1/onepasswd/templates/static/
--rw-r--r--   0 runner    (1001) docker     (123)    80578 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/templates/static/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/templates/static/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/templates/static/inconsolata:wght@500.css
--rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/templates/static/jquery-3.6.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    55371 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/templates/static/jsencrypt.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:59:23.240979 onepasswd-0.2.4rc1/onepasswd/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/tools/jdiff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1844 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/tools/jmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/tools/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/onepasswd/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:59:23.236979 onepasswd-0.2.4rc1/onepasswd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-06 17:59:23.000000 onepasswd-0.2.4rc1/onepasswd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-06 17:59:23.000000 onepasswd-0.2.4rc1/onepasswd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 17:59:23.000000 onepasswd-0.2.4rc1/onepasswd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-06 17:59:23.000000 onepasswd-0.2.4rc1/onepasswd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-06 17:59:23.000000 onepasswd-0.2.4rc1/onepasswd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 17:59:23.000000 onepasswd-0.2.4rc1/onepasswd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 17:59:23.240979 onepasswd-0.2.4rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-06 17:59:11.000000 onepasswd-0.2.4rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.018192 onepasswd-0.2.4rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.006191 onepasswd-0.2.4rc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.010192 onepasswd-0.2.4rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 04:41:31.018192 onepasswd-0.2.4rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.014192 onepasswd-0.2.4rc2/onepasswd/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/ltlog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5231 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/onepasswd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.014192 onepasswd-0.2.4rc2/onepasswd/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.014192 onepasswd-0.2.4rc2/onepasswd/templates/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    80578 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/static/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/static/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/static/inconsolata:wght@500.css
+-rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/static/jquery-3.6.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    55371 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/templates/static/jsencrypt.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.018192 onepasswd-0.2.4rc2/onepasswd/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/tools/jdiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1844 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/tools/jmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/tools/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/onepasswd/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:41:31.014192 onepasswd-0.2.4rc2/onepasswd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 04:41:30.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-17 04:41:31.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 04:41:30.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-17 04:41:30.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 04:41:30.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 04:41:30.000000 onepasswd-0.2.4rc2/onepasswd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 04:41:31.018192 onepasswd-0.2.4rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-17 04:41:04.000000 onepasswd-0.2.4rc2/setup.py
```

### Comparing `onepasswd-0.2.4rc1/.github/workflows/ci.yml` & `onepasswd-0.2.4rc2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/client.py` & `onepasswd-0.2.4rc2/onepasswd/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,29 +169,29 @@
 def add(ctx: click.Context, entries: tuple, length, strength):
     d = {}
 
     def getpass():
         passwd = PasswdGen.generate(length, pre_process_strength(strength))
         d['passwd'] = passwd
         return passwd
-    save_passwd(ctx, entries, getpass)
-    give_passwd(ctx, d['passwd'])
-    if click.confirm('sync ?'):
-        ctx.invoke(sync)
+    if save_passwd(ctx, entries, getpass):
+        give_passwd(ctx, d['passwd'])
+        if click.confirm('sync ?'):
+            ctx.invoke(sync)
 
 
 @cli.command('save')
 @click.argument('entries', nargs=-1)
 @click.pass_context
 def save(ctx: click.Context, entries: tuple):
     def getpass():
         return get_passwd(ctx, promt='new password', confirm=True)
-    save_passwd(ctx, entries, getpass)
-    if click.confirm('sync ?'):
-        ctx.invoke(sync)
+    if save_passwd(ctx, entries, getpass):
+        if click.confirm('sync ?'):
+            ctx.invoke(sync)
 
 
 @cli.command('del')
 @click.argument('keywords', nargs=-1)
 @click.pass_context
 def delete(ctx: click.Context, keywords: tuple):
     if len(keywords) == 0:
@@ -246,26 +246,22 @@
 def save_passwd(ctx, entries, getpass):
     assert len(entries) >= 1
     db = get_db(ctx)
     if entries in db:
         item = db.get_item(entries)
         if not click.confirm(
                 f'{passwd_item_str(item)} already in database, update ?'):
-            return
+            return False
         cfg = from_ctx(ctx, 'config')
         db.backup(cfg['backup'])
     passwd = get_passwd(ctx, promt='master password', from_clipboard=False, key='passwd')
     passwd_dec = getpass()
     passwd_enc = crypto.encrypt_passwd(passwd_dec, passwd)
-    item = {
-        'entries': entries,
-        'passwd': passwd_enc,
-        'time': str(time.time())
-    }
-    db[entries] = item
+    db[entries] = passwd_enc
+    return True
 
 
 def pre_process_strength(s):
     strength = set()
     for x in s:
         for i, t in enumerate(PasswdGen.passwd_table):
             if x in t:
```

### Comparing `onepasswd-0.2.4rc1/onepasswd/config.py` & `onepasswd-0.2.4rc2/onepasswd/config.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/crypto.py` & `onepasswd-0.2.4rc2/onepasswd/crypto.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/ltlog.py` & `onepasswd-0.2.4rc2/onepasswd/ltlog.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/onepasswd.py` & `onepasswd-0.2.4rc2/onepasswd/onepasswd.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/templates/index.html` & `onepasswd-0.2.4rc2/onepasswd/templates/index.html`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/templates/static/bootstrap.bundle.min.js` & `onepasswd-0.2.4rc2/onepasswd/templates/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/templates/static/bootstrap.min.css` & `onepasswd-0.2.4rc2/onepasswd/templates/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/templates/static/jquery-3.6.4.min.js` & `onepasswd-0.2.4rc2/onepasswd/templates/static/jquery-3.6.4.min.js`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/templates/static/jsencrypt.min.js` & `onepasswd-0.2.4rc2/onepasswd/templates/static/jsencrypt.min.js`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/tools/jdiff.py` & `onepasswd-0.2.4rc2/onepasswd/tools/jdiff.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/tools/jmerge.py` & `onepasswd-0.2.4rc2/onepasswd/tools/jmerge.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/tools/upgrade.py` & `onepasswd-0.2.4rc2/onepasswd/tools/upgrade.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd/web.py` & `onepasswd-0.2.4rc2/onepasswd/web.py`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/onepasswd.egg-info/SOURCES.txt` & `onepasswd-0.2.4rc2/onepasswd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onepasswd-0.2.4rc1/setup.py` & `onepasswd-0.2.4rc2/setup.py`

 * *Files identical despite different names*

