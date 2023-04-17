# Comparing `tmp/dokos-1.0.3.tar.gz` & `tmp/dokos-1.0.4.tar.gz`

## Comparing `dokos-1.0.3.tar` & `dokos-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 dokos-1.0.3/.gitlab-ci.yml
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 dokos-1.0.3/10-million-password-list-top-1000.txt
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dokos-1.0.3/pyproject.tmpl
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dokos-1.0.3/requirements.txt
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 dokos-1.0.3/.vscode/launch.json
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dokos-1.0.3/src/dokos/VERSION
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dokos-1.0.3/src/dokos/__init__.py
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 dokos-1.0.3/src/dokos/__main__.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 dokos-1.0.3/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 dokos-1.0.3/LICENSE
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dokos-1.0.3/README.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 dokos-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 dokos-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 dokos-1.0.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 dokos-1.0.4/10-million-password-list-top-1000.txt
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dokos-1.0.4/pyproject.tmpl
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dokos-1.0.4/requirements.txt
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 dokos-1.0.4/.vscode/launch.json
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dokos-1.0.4/src/dokos/VERSION
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dokos-1.0.4/src/dokos/__init__.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 dokos-1.0.4/src/dokos/__main__.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 dokos-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 dokos-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dokos-1.0.4/README.md
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 dokos-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 dokos-1.0.4/PKG-INFO
```

### Comparing `dokos-1.0.3/.gitlab-ci.yml` & `dokos-1.0.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dokos-1.0.3/10-million-password-list-top-1000.txt` & `dokos-1.0.4/10-million-password-list-top-1000.txt`

 * *Files identical despite different names*

### Comparing `dokos-1.0.3/pyproject.tmpl` & `dokos-1.0.4/pyproject.tmpl`

 * *Files identical despite different names*

### Comparing `dokos-1.0.3/.vscode/launch.json` & `dokos-1.0.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dokos-1.0.3/src/dokos/__main__.py` & `dokos-1.0.4/src/dokos/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # https://superfastpython.com/thread-safe-print-in-python/
 LOCK = Lock()
 
 # indicates that the thread may continue running
 # used to stop threads if user interrupted processing...
 RUN = True
 ARGS = None
+COUNT = 0
 
 PASSWORDS = []
 
 # found passwords
 FOUND = []
 
 def print_safe(string) :
@@ -83,20 +84,25 @@
 
 def try_passwords(passwords):
     '''
     Try a list of passwords
     '''
 
     for password in passwords :
+        global COUNT
+        COUNT += 1
         # we were interrupted by user
         if not RUN :
             break
         password = password.strip()
         print_safe("login: " + ARGS.login + " password: " + password)
         try_password(password)
+        # stop if we found a password
+        if ARGS.stop_on_first and len(FOUND) > 0:
+            break
 
 def islice(iterable, *args):
     '''
     https://docs.python.org/3/library/itertools.html#recipes
     # islice('ABCDEFG', 2) --> A B
     # islice('ABCDEFG', 2, 4) --> C D
     # islice('ABCDEFG', 2, None) --> C D E F G
@@ -150,14 +156,15 @@
     parser.add_argument('-t', '--threads', type=int, default=10,
     help='Number of threads (default: 10)')
     parser.add_argument('-f', '--failed', default="Bad combination of e-mail and password",
     help='Message indicating a failed attempt (default: "Bad combination of e-mail and password")')
     parser.add_argument('--login_field', default='email')
     parser.add_argument('--password_field', default='password')
     parser.add_argument('url')
+    parser.add_argument('--stop-on-first', action='store_true', default=False, help='Stop on first found password')
 
     ARGS = parser.parse_args()
 
 def validate_arguments() :
     '''
     Check if provided arguments seem valid
     '''
@@ -224,13 +231,13 @@
     read_passwords()
     
     run()
 
     print("Done!")
     end = datetime.now()
     delta_t = (end - start).total_seconds()
-    rate = len(PASSWORDS) / delta_t
+    rate = COUNT / delta_t
     print("Time: " + str(delta_t) + " seconds [" + str(round(rate, 2)) + " passwords/sec]")
     print("Found " + str(len(FOUND)) + " password(s): " + str(FOUND))
 
 if __name__ == "__main__":
     main()
```

### Comparing `dokos-1.0.3/.gitignore` & `dokos-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dokos-1.0.3/LICENSE` & `dokos-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dokos-1.0.3/README.md` & `dokos-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dokos-1.0.3/pyproject.toml` & `dokos-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Dokos"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Thibault Debatty", email="t.debatty@cylab.be" },
 ]
 description = "HTTP login cracker"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `dokos-1.0.3/PKG-INFO` & `dokos-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dokos
-Version: 1.0.3
+Version: 1.0.4
 Summary: HTTP login cracker
 Project-URL: Homepage, https://gitlab.cylab.be/cylab/dokos
 Project-URL: Bug Tracker, https://gitlab.cylab.be/cylab/dokos/-/issues
 Author-email: Thibault Debatty <t.debatty@cylab.be>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

