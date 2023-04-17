# Comparing `tmp/bhokacha-0.1.0-py3-none-any.whl.zip` & `tmp/bhokacha-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 1414 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-17 07:01 bhokacha/__init__.py
--rw-rw-rw-  2.0 fat      209 b- defN 23-Apr-17 07:27 bhokacha/pal.py
--rw-rw-rw-  2.0 fat      109 b- defN 23-Apr-17 07:32 bhokacha-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 07:32 bhokacha-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-17 07:32 bhokacha-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      445 b- defN 23-Apr-17 07:32 bhokacha-0.1.0.dist-info/RECORD
-6 files, 864 bytes uncompressed, 602 bytes compressed:  30.3%
+-rw-rw-rw-  2.0 fat      197 b- defN 23-Apr-17 07:42 bhokacha/pal.py
+-rw-rw-rw-  2.0 fat      109 b- defN 23-Apr-17 09:53 bhokacha-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 09:53 bhokacha-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-17 09:53 bhokacha-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      445 b- defN 23-Apr-17 09:53 bhokacha-0.2.0.dist-info/RECORD
+6 files, 852 bytes uncompressed, 602 bytes compressed:  29.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: bhokacha/__init__.py
 Comment: 
 
 Filename: bhokacha/pal.py
 Comment: 
 
-Filename: bhokacha-0.1.0.dist-info/METADATA
+Filename: bhokacha-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: bhokacha-0.1.0.dist-info/WHEEL
+Filename: bhokacha-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: bhokacha-0.1.0.dist-info/top_level.txt
+Filename: bhokacha-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bhokacha-0.1.0.dist-info/RECORD
+Filename: bhokacha-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bhokacha/pal.py

```diff
@@ -5,8 +5,7 @@
     reverse=b[::-1]
 
     if b==reverse:
         print('palidrome')
     else:
         print('nonpalidrome')    
 
-palidrome(a)
```

