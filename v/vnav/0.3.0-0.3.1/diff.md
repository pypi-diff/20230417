# Comparing `tmp/vnav-0.3.0-py2.py3-none-any.whl.zip` & `tmp/vnav-0.3.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5344 bytes, number of entries: 6
--rwxr-xr-x  2.0 unx     9307 b- defN 22-Feb-04 20:16 vnav-0.3.0.data/scripts/parse_vNav_Motion.py
--rw-r--r--  2.0 unx     1057 b- defN 22-Feb-04 20:16 vnav-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      309 b- defN 22-Feb-04 20:16 vnav-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Feb-04 20:16 vnav-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 22-Feb-04 20:16 vnav-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      471 b- defN 22-Feb-04 20:16 vnav-0.3.0.dist-info/RECORD
-6 files, 11255 bytes uncompressed, 4490 bytes compressed:  60.1%
+Zip file size: 5427 bytes, number of entries: 6
+-rwxr-xr-x  2.0 unx     9600 b- defN 23-Apr-17 14:29 vnav-0.3.1.data/scripts/parse_vNav_Motion.py
+-rw-r--r--  2.0 unx     1057 b- defN 23-Apr-17 14:29 vnav-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      286 b- defN 23-Apr-17 14:29 vnav-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-17 14:29 vnav-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-17 14:29 vnav-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      471 b- defN 23-Apr-17 14:29 vnav-0.3.1.dist-info/RECORD
+6 files, 11525 bytes uncompressed, 4573 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: vnav-0.3.0.data/scripts/parse_vNav_Motion.py
+Filename: vnav-0.3.1.data/scripts/parse_vNav_Motion.py
 Comment: 
 
-Filename: vnav-0.3.0.dist-info/LICENSE
+Filename: vnav-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: vnav-0.3.0.dist-info/METADATA
+Filename: vnav-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: vnav-0.3.0.dist-info/WHEEL
+Filename: vnav-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: vnav-0.3.0.dist-info/top_level.txt
+Filename: vnav-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vnav-0.3.0.dist-info/RECORD
+Filename: vnav-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `vnav-0.3.0.data/scripts/parse_vNav_Motion.py` & `vnav-0.3.1.data/scripts/parse_vNav_Motion.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,28 +25,35 @@
   quaternions = [(
     np.array([1,0,0,0]),
     np.array([0,0,0])
   )]
   for x in ds[1:]:
     instance = x.InstanceNumber
     acquisition = x.AcquisitionNumber
-    # check if vNav failed
-    if re.match('^\? F:', x.ImageComments):
+    '''
+    vNav failures do not appear to be encoded consistently. The following regular
+    expression was crafted based on a small number of examples.
+    '''
+    if re.match('^.*\? F:', x.ImageComments):
         print(f'failure detected instance={instance}, acquisition={acquisition}')
         failed = (instance, acquisition)
         break
     y = str.split(x.ImageComments)
     rotation = np.array(list(map(float, y[1:5])))
     translation = np.array(list(map(float, y[6:9])))
     quaternions.append((rotation, translation))
 
   return quaternions,failed
 
 def readRotAndTransFromJson(js):
-  failure = '^\?_F:'
+  '''
+  vNav failures do not appear to be encoded consistently. The following regular
+  expression was crafted based on a small number of examples.
+  '''
+  failure = '^.*\?_F:'
   pattern = 'R:_(.*?)_(.*?)_(.*?)_(.*?)_T:_(.*?)_(.*?)_(.*?)_F:.'
   failed = None
   # parse ImageComments and return quaternion values
   quaternions = [(
     np.array([1,0,0,0]),
     np.array([0,0,0])
   )]
```

## Comparing `vnav-0.3.0.dist-info/LICENSE` & `vnav-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

