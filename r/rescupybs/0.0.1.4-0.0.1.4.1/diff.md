# Comparing `tmp/rescupybs-0.0.1.4-py3-none-any.whl.zip` & `tmp/rescupybs-0.0.1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9010 bytes, number of entries: 10
--rwxrwxrwx  2.0 unx       29 b- defN 23-Apr-15 16:23 rescupybs/__init__.py
--rwxrwxrwx  2.0 unx     8451 b- defN 23-Apr-15 22:42 rescupybs/functions.py
--rwxrwxrwx  2.0 unx     6786 b- defN 23-Mar-31 04:58 rescupybs/plots.py
--rwxrwxrwx  2.0 unx    12318 b- defN 23-Apr-15 22:01 rescupybs/wrapper.py
--rwxrwxrwx  2.0 unx     1060 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/LICENSE
--rwxrwxrwx  2.0 unx     2963 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       88 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx       10 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      813 b- defN 23-Apr-15 22:43 rescupybs-0.0.1.4.dist-info/RECORD
-10 files, 32610 bytes uncompressed, 7620 bytes compressed:  76.6%
+Zip file size: 9034 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx       31 b- defN 23-Apr-17 15:02 rescupybs/__init__.py
+-rw-rw-r--  2.0 unx     8451 b- defN 23-Apr-17 15:02 rescupybs/functions.py
+-rw-rw-r--  2.0 unx     6786 b- defN 23-Apr-17 15:02 rescupybs/plots.py
+-rw-rw-r--  2.0 unx    12318 b- defN 23-Apr-17 15:02 rescupybs/wrapper.py
+-rwxrwxr-x  2.0 unx     1060 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2965 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       88 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      825 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/RECORD
+10 files, 32626 bytes uncompressed, 7620 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: rescupybs/plots.py
 Comment: 
 
 Filename: rescupybs/wrapper.py
 Comment: 
 
-Filename: rescupybs-0.0.1.4.dist-info/LICENSE
+Filename: rescupybs-0.0.1.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: rescupybs-0.0.1.4.dist-info/METADATA
+Filename: rescupybs-0.0.1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: rescupybs-0.0.1.4.dist-info/WHEEL
+Filename: rescupybs-0.0.1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: rescupybs-0.0.1.4.dist-info/entry_points.txt
+Filename: rescupybs-0.0.1.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rescupybs-0.0.1.4.dist-info/top_level.txt
+Filename: rescupybs-0.0.1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rescupybs-0.0.1.4.dist-info/RECORD
+Filename: rescupybs-0.0.1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rescupybs/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.0.1.4"
+__version__ = "0.0.1.4.1"
```

## rescupybs/functions.py

 * *Ordering differences only*

```diff
@@ -151,14 +151,15 @@
     i, vb = np.where(eigenvalues_s==max)
     i, cb = np.where(eigenvalues_s==min)
     return vb[0], max, cb[0], min
 
 # rescuiso
 
 def isosurfaces_wf(input, output, kpt, band, spin):
+    calc = TotalEnergy.read(input+'.json')
     if not output:
         output = input+'_'+str(kpt)+'_'+str(band)+'_'+str(spin)+'.vasp'
     if calc.system.hamiltonian.ispin == 1:
         att = f"wavefunctions/{kpt + 1}/field"
     else:
         if spin == 1:
             att = f"wavefunctions/spin-up/{kpt + 1}/field"
@@ -175,15 +176,14 @@
     if band < fld.shape[-1]:
         fld = fld[..., band].magnitude
     else:
         raise Exception("The band is out of range in *.h5 file.")
     f_abs = np.abs(fld)
     f_div = np.where(np.abs(np.angle(fld)) < np.pi / 2, f_abs, -f_abs)
     f_div = np.reshape(f_div, (f_div.shape[-1], -1), order='F').T
-    calc = TotalEnergy.read(input+'.json')
     pbc = [1, 1, 1]
     positions = calc.system.atoms.positions
     cell = calc.system.cell.avec
     elements_symbols = calc.system.atoms.get_labels()
     stp = ats(elements_symbols,positions=positions,cell=cell,pbc=pbc)
     grid = calc.system.cell.grid
     write(output, stp, direct=True, vasp5=True)
```

## Comparing `rescupybs-0.0.1.4.dist-info/LICENSE` & `rescupybs-0.0.1.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rescupybs-0.0.1.4.dist-info/METADATA` & `rescupybs-0.0.1.4.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rescupybs
-Version: 0.0.1.4
+Version: 0.0.1.4.1
 Summary: Band structure plot from rescuplus json file.
 Home-page: https://github.com/lkccrr/rescupybs
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT rescuplus band plot
 Platform: Unix
```

## Comparing `rescupybs-0.0.1.4.dist-info/RECORD` & `rescupybs-0.0.1.4.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-rescupybs/__init__.py,sha256=EwUBrbjqfFSu5mrlRfgjbaVl39_D-q5WlKKDhiOSkRI,29
-rescupybs/functions.py,sha256=Ume1P3SYVE2iOuK5Tq4taN8PEDgRldr8NSMnr11RNVI,8451
+rescupybs/__init__.py,sha256=uRZB6lfluFaiILvY9xTIJNSWH8uUi3PptihixnpR9i4,31
+rescupybs/functions.py,sha256=763QQvahDztZM7nW48EnoRWLAUWbhe_ArLKfCDT5mzA,8451
 rescupybs/plots.py,sha256=5_7__zep7lgbxNqw-UZ_Nm2h4uSbtjCbeqB9g3FHLoM,6786
 rescupybs/wrapper.py,sha256=znQ51PrhuD9I7_gd35m8eAIxZ3hdgzMFAckAC4W2kdE,12318
-rescupybs-0.0.1.4.dist-info/LICENSE,sha256=aWH1yhtukPX_iihAaz4foL04PJNxgsrRPqp_iwxlTr0,1060
-rescupybs-0.0.1.4.dist-info/METADATA,sha256=OAE3ReboQQG2B5UDDlGsx2OIheb1Y4KieFSgJwPmHwY,2963
-rescupybs-0.0.1.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-rescupybs-0.0.1.4.dist-info/entry_points.txt,sha256=WpFczXTlVBUla6UWHKetnJ_VGriTtoTlEQ63Tvy635U,88
-rescupybs-0.0.1.4.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
-rescupybs-0.0.1.4.dist-info/RECORD,,
+rescupybs-0.0.1.4.1.dist-info/LICENSE,sha256=aWH1yhtukPX_iihAaz4foL04PJNxgsrRPqp_iwxlTr0,1060
+rescupybs-0.0.1.4.1.dist-info/METADATA,sha256=oefrBkNQMyTn4HJCv8_exo1tuZ8T_OIp4Jdv09tLloE,2965
+rescupybs-0.0.1.4.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+rescupybs-0.0.1.4.1.dist-info/entry_points.txt,sha256=WpFczXTlVBUla6UWHKetnJ_VGriTtoTlEQ63Tvy635U,88
+rescupybs-0.0.1.4.1.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
+rescupybs-0.0.1.4.1.dist-info/RECORD,,
```

