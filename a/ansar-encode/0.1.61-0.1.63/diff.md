# Comparing `tmp/ansar-encode-0.1.61.tar.gz` & `tmp/ansar-encode-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-encode-0.1.61.tar", last modified: Wed Mar  1 20:37:43 2023, max compression
+gzip compressed data, was "ansar-encode-0.1.63.tar", last modified: Mon Apr 17 20:34:44 2023, max compression
```

## Comparing `ansar-encode-0.1.61.tar` & `ansar-encode-0.1.63.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-03-01 20:37:43.800935 ansar-encode-0.1.61/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2022-10-03 18:49:48.000000 ansar-encode-0.1.61/LICENSE
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-03-01 20:37:43.800935 ansar-encode-0.1.61/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      830 2022-10-02 23:59:34.000000 ansar-encode-0.1.61/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      309 2022-10-03 00:32:14.000000 ansar-encode-0.1.61/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-03-01 20:37:43.800935 ansar-encode-0.1.61/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-01-05 21:34:37.000000 ansar-encode-0.1.61/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-03-01 20:37:43.800935 ansar-encode-0.1.61/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-03-01 20:37:43.800935 ansar-encode-0.1.61/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-03-01 20:37:43.800935 ansar-encode-0.1.61/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-02-04 16:29:11.000000 ansar-encode-0.1.61/src/ansar/command/show_release.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-03-01 20:37:43.800935 ansar-encode-0.1.61/src/ansar/encode/
--rw-rw-r--   0 scott     (1000) scott     (1000)     4911 2023-03-01 20:37:40.000000 ansar-encode-0.1.61/src/ansar/encode/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37225 2022-11-04 02:21:50.000000 ansar-encode-0.1.61/src/ansar/encode/codec.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-02-28 08:57:41.000000 ansar-encode-0.1.61/src/ansar/encode/convert.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11215 2023-01-19 23:29:20.000000 ansar-encode-0.1.61/src/ansar/encode/file.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19813 2023-02-28 09:06:01.000000 ansar-encode-0.1.61/src/ansar/encode/folder.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2022-10-03 19:30:53.000000 ansar-encode-0.1.61/src/ansar/encode/json.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-02-28 08:58:39.000000 ansar-encode-0.1.61/src/ansar/encode/message.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-02-05 20:30:57.000000 ansar-encode-0.1.61/src/ansar/encode/portable.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2022-09-05 20:25:39.000000 ansar-encode-0.1.61/src/ansar/encode/release.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6155 2023-02-28 09:06:13.000000 ansar-encode-0.1.61/src/ansar/encode/runtime.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2022-10-25 02:07:57.000000 ansar-encode-0.1.61/src/ansar/encode/version.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2022-08-03 00:49:03.000000 ansar-encode-0.1.61/src/ansar/encode/xml.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-03-01 20:37:43.800935 ansar-encode-0.1.61/src/ansar_encode.egg-info/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-03-01 20:37:43.000000 ansar-encode-0.1.61/src/ansar_encode.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-03-01 20:37:43.000000 ansar-encode-0.1.61/src/ansar_encode.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-03-01 20:37:43.000000 ansar-encode-0.1.61/src/ansar_encode.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-03-01 20:37:43.000000 ansar-encode-0.1.61/src/ansar_encode.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-03-01 20:37:43.000000 ansar-encode-0.1.61/src/ansar_encode.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-03-01 20:37:43.000000 ansar-encode-0.1.61/src/ansar_encode.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:44.004489 ansar-encode-0.1.63/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2022-10-03 18:49:48.000000 ansar-encode-0.1.63/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-04-17 20:34:44.004489 ansar-encode-0.1.63/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      830 2022-10-02 23:59:34.000000 ansar-encode-0.1.63/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      309 2022-10-03 00:32:14.000000 ansar-encode-0.1.63/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-04-17 20:34:44.004489 ansar-encode-0.1.63/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-01-05 21:34:37.000000 ansar-encode-0.1.63/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:43.996489 ansar-encode-0.1.63/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:43.996489 ansar-encode-0.1.63/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:43.996489 ansar-encode-0.1.63/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-02-04 16:29:11.000000 ansar-encode-0.1.63/src/ansar/command/show_release.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:44.004489 ansar-encode-0.1.63/src/ansar/encode/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4911 2023-04-17 20:34:40.000000 ansar-encode-0.1.63/src/ansar/encode/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-17 19:54:59.000000 ansar-encode-0.1.63/src/ansar/encode/codec.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-02-28 08:57:41.000000 ansar-encode-0.1.63/src/ansar/encode/convert.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11215 2023-01-19 23:29:20.000000 ansar-encode-0.1.63/src/ansar/encode/file.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19829 2023-04-15 02:45:44.000000 ansar-encode-0.1.63/src/ansar/encode/folder.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2022-10-03 19:30:53.000000 ansar-encode-0.1.63/src/ansar/encode/json.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-02-28 08:58:39.000000 ansar-encode-0.1.63/src/ansar/encode/message.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-02-05 20:30:57.000000 ansar-encode-0.1.63/src/ansar/encode/portable.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2022-09-05 20:25:39.000000 ansar-encode-0.1.63/src/ansar/encode/release.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6155 2023-02-28 09:06:13.000000 ansar-encode-0.1.63/src/ansar/encode/runtime.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2022-10-25 02:07:57.000000 ansar-encode-0.1.63/src/ansar/encode/version.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2022-08-03 00:49:03.000000 ansar-encode-0.1.63/src/ansar/encode/xml.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-04-17 20:34:44.004489 ansar-encode-0.1.63/src/ansar_encode.egg-info/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-04-17 20:34:43.000000 ansar-encode-0.1.63/src/ansar_encode.egg-info/top_level.txt
```

### Comparing `ansar-encode-0.1.61/LICENSE` & `ansar-encode-0.1.63/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/PKG-INFO` & `ansar-encode-0.1.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.61
+Version: 0.1.63
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.61/README.md` & `ansar-encode-0.1.63/README.md`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/setup.py` & `ansar-encode-0.1.63/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/src/ansar/command/show_release.py` & `ansar-encode-0.1.63/src/ansar/command/show_release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/src/ansar/encode/__init__.py` & `ansar-encode-0.1.63/src/ansar/encode/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Persistence of complex application data.
 
 Repo: git@ansar.gitlab.com:scott-ansar/ansar-encode.git
 Branch: main
-Commit: f230df65002fca3b9720f42b0ddfe24d7a9c5aab
-Version: 0.1.60 (2023-03-02@09:37:40+NZDT)
+Commit: ace301a25c9df66a00df24f4f57e607fbc2591d9
+Version: 0.1.62 (2023-04-18@08:34:40+NZST)
 """
 
 from .portable import Boolean
 from .portable import Byte, Character, Rune
 from .portable import Integer2, Integer4, Integer8
 from .portable import Unsigned2, Unsigned4, Unsigned8
 from .portable import Float4, Float8
```

### Comparing `ansar-encode-0.1.61/src/ansar/encode/codec.py` & `ansar-encode-0.1.63/src/ansar/encode/codec.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,20 +97,16 @@
 
     def __init__(self, note):
         """Construct the exception.
 
         :param note: hint as to what happened
         :type name: str
         """
-        Exception.__init__(self)
-        self.note = note
-
-    def __str__(self):
-        """Auto-convert to text representation. Return string."""
-        return self.note
+        Exception.__init__(self, note)
+        self.note = note				# For quick access.
 
 class CodecUsage(CodecError):
     """Cannot proceed due to its supplied environment such as unusable parameters."""
 
     def __init__(self, note, *a):
         """Construct the exception.
```

### Comparing `ansar-encode-0.1.61/src/ansar/encode/convert.py` & `ansar-encode-0.1.63/src/ansar/encode/convert.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/src/ansar/encode/file.py` & `ansar-encode-0.1.63/src/ansar/encode/file.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/src/ansar/encode/folder.py` & `ansar-encode-0.1.63/src/ansar/encode/folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,20 +83,20 @@
 def remove_folder(path):
     """Delete everything under the given folder, and then the folder."""
     try:
         remove_contents(path)
         os.rmdir(path)
     except OSError as e:
         if e.errno == errno.ENOENT:
-            raise FileNotFound(REMOVE_FOLDER, p, 'name does not exist', e.errno)
+            raise FileNotFound(REMOVE_FOLDER, path, 'name does not exist', e.errno)
         elif e.errno in (errno.EACCES, errno.EPERM):
-            raise FileNoAccess(REMOVE_FOLDER, p, 'access or permissions', e.errno)
+            raise FileNoAccess(REMOVE_FOLDER, path, 'access or permissions', e.errno)
         elif e.errno == errno.ENOTDIR:
-            raise FileNotAFile(REMOVE_FOLDER, p, 'name in path is not a folder', e.errno)
-        raise FileFailure(REMOVE_FOLDER, p, 'unexpected platform code', code=0)
+            raise FileNotAFile(REMOVE_FOLDER, path, 'name in path is not a folder', e.errno)
+        raise FileFailure(REMOVE_FOLDER, path, 'unexpected platform code', code=0)
 #
 #
 def shape_of_folder(path):
     """Walk the given folder, acumulating folders, files and bytes (3-tuple)."""
     folders, files, bytes = 0, 0, 0
     try:
         for f in os.listdir(path):
@@ -274,15 +274,15 @@
                 continue
             if decorate_names:
                 b, e = os.path.splitext(f)
                 if e != extension:
                     continue
                 f = b
             if re:
-                m = re.match(f)
+                m = re.fullmatch(f)
                 if not m:
                     continue
             yield f
 
     def each(self):
         """Process the files in the folder.
```

### Comparing `ansar-encode-0.1.61/src/ansar/encode/json.py` & `ansar-encode-0.1.63/src/ansar/encode/json.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/src/ansar/encode/message.py` & `ansar-encode-0.1.63/src/ansar/encode/message.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/src/ansar/encode/portable.py` & `ansar-encode-0.1.63/src/ansar/encode/portable.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/src/ansar/encode/release.py` & `ansar-encode-0.1.63/src/ansar/encode/release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/src/ansar/encode/runtime.py` & `ansar-encode-0.1.63/src/ansar/encode/runtime.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/src/ansar/encode/version.py` & `ansar-encode-0.1.63/src/ansar/encode/version.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/src/ansar/encode/xml.py` & `ansar-encode-0.1.63/src/ansar/encode/xml.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.61/src/ansar_encode.egg-info/PKG-INFO` & `ansar-encode-0.1.63/src/ansar_encode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.61
+Version: 0.1.63
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.suzuki@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-encode-0.1.61/src/ansar_encode.egg-info/SOURCES.txt` & `ansar-encode-0.1.63/src/ansar_encode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

