# Comparing `tmp/magyar-2.9.3.tar.gz` & `tmp/magyar-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.9.3.tar", last modified: Sun Apr 16 15:54:19 2023, max compression
+gzip compressed data, was "magyar-2.9.4.tar", last modified: Mon Apr 17 21:14:44 2023, max compression
```

## Comparing `magyar-2.9.3.tar` & `magyar-2.9.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-16 15:54:19.770351 magyar-2.9.3/
--rw-rw-r--   0 bela      (1000) bela      (1000)     2925 2023-04-16 15:54:19.770351 magyar-2.9.3/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     2554 2023-04-16 15:50:54.000000 magyar-2.9.3/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-16 15:54:19.770351 magyar-2.9.3/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     2925 2023-04-16 15:54:19.000000 magyar-2.9.3/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-16 15:54:19.000000 magyar-2.9.3/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-16 15:54:19.000000 magyar-2.9.3/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-16 15:54:19.000000 magyar-2.9.3/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    28123 2023-04-16 15:46:17.000000 magyar-2.9.3/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-16 15:54:19.770351 magyar-2.9.3/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-16 15:54:10.000000 magyar-2.9.3/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-17 21:14:44.427517 magyar-2.9.4/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     3419 2023-04-17 21:14:44.427517 magyar-2.9.4/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     3048 2023-04-17 21:12:46.000000 magyar-2.9.4/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-17 21:14:44.427517 magyar-2.9.4/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     3419 2023-04-17 21:14:44.000000 magyar-2.9.4/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-17 21:14:44.000000 magyar-2.9.4/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-17 21:14:44.000000 magyar-2.9.4/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-17 21:14:44.000000 magyar-2.9.4/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    29782 2023-04-17 21:12:46.000000 magyar-2.9.4/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-17 21:14:44.427517 magyar-2.9.4/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-17 19:59:27.000000 magyar-2.9.4/setup.py
```

### Comparing `magyar-2.9.3/PKG-INFO` & `magyar-2.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.3
+Version: 2.9.4
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,20 +27,22 @@
 9. az év hónapjai = magyar.honap
 10. gyümölcsok = magyar.gyumolcs
 11. zöldségek = magyar.zoldseg
 12. haszonállatok = magyar.haszonallat
 13. vadallatok Magyarországon = magyar.vadallat
 14. Magyarország halai = magyar.hal
 15. Magyarország madarai = magyar.madar
+16. A naprendszer bolygóinak magyar neve = magyar.bolygo
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
+5. Európa országai és fővárosai=  magyar.orszag
 
 ## Description
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
@@ -50,20 +52,22 @@
 9. the months of the year = magyar.honap
 10. fruits = magyar.gyumolcs
 11. vegetables = magyar.zoldseg
 12. domesticated animals = magyar.haszonallat
 13. hungarian wildlife  = magyar.vadallat
 14. Fishes of Hungary = magyar.hal
 15. Birds of Hungary = magyar.madar
+16. Hungarian names of planets = magyar.bolygo
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
-4. Hungarian tram lines  magyar.villamos
+4. Hungarian tram lines = magyar.villamos
+5. Hunngarian names of Europian capitals, states = magyar.orszag
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators. 
        
@@ -74,18 +78,23 @@
 
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
     magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
     magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
     magyar.jaras :             {'megye' : (székhely, megye)}
-    magyar.villamos:    kulcs {'viszonylat', indulas, erkezes, menetido, varos}
-
+    magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
+    magyar.orszag:             {'orszag': 'főváros'}
 
+## Metódus
+   A  szótárakból választhatsz véletlenszerű KULCSOT. (szótár neve, elemek száma)
+                    
+    szotarbol_veletlen_kulcs(szotar, n)
 
+    pl: szotarbol_veletlen_kulcs(magyar.megye, 12)
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-2.9.3/README.md` & `magyar-2.9.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 9. az év hónapjai = magyar.honap
 10. gyümölcsok = magyar.gyumolcs
 11. zöldségek = magyar.zoldseg
 12. haszonállatok = magyar.haszonallat
 13. vadallatok Magyarországon = magyar.vadallat
 14. Magyarország halai = magyar.hal
 15. Magyarország madarai = magyar.madar
+16. A naprendszer bolygóinak magyar neve = magyar.bolygo
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
+5. Európa országai és fővárosai=  magyar.orszag
 
 ## Description
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
@@ -38,20 +40,22 @@
 9. the months of the year = magyar.honap
 10. fruits = magyar.gyumolcs
 11. vegetables = magyar.zoldseg
 12. domesticated animals = magyar.haszonallat
 13. hungarian wildlife  = magyar.vadallat
 14. Fishes of Hungary = magyar.hal
 15. Birds of Hungary = magyar.madar
+16. Hungarian names of planets = magyar.bolygo
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
-4. Hungarian tram lines  magyar.villamos
+4. Hungarian tram lines = magyar.villamos
+5. Hunngarian names of Europian capitals, states = magyar.orszag
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators. 
        
@@ -62,18 +66,23 @@
 
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
     magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
     magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
     magyar.jaras :             {'megye' : (székhely, megye)}
-    magyar.villamos:    kulcs {'viszonylat', indulas, erkezes, menetido, varos}
-
+    magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
+    magyar.orszag:             {'orszag': 'főváros'}
 
+## Metódus
+   A  szótárakból választhatsz véletlenszerű KULCSOT. (szótár neve, elemek száma)
+                    
+    szotarbol_veletlen_kulcs(szotar, n)
 
+    pl: szotarbol_veletlen_kulcs(magyar.megye, 12)
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-2.9.3/magyar.egg-info/PKG-INFO` & `magyar-2.9.4/magyar.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.3
+Version: 2.9.4
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,20 +27,22 @@
 9. az év hónapjai = magyar.honap
 10. gyümölcsok = magyar.gyumolcs
 11. zöldségek = magyar.zoldseg
 12. haszonállatok = magyar.haszonallat
 13. vadallatok Magyarországon = magyar.vadallat
 14. Magyarország halai = magyar.hal
 15. Magyarország madarai = magyar.madar
+16. A naprendszer bolygóinak magyar neve = magyar.bolygo
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
+5. Európa országai és fővárosai=  magyar.orszag
 
 ## Description
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
@@ -50,20 +52,22 @@
 9. the months of the year = magyar.honap
 10. fruits = magyar.gyumolcs
 11. vegetables = magyar.zoldseg
 12. domesticated animals = magyar.haszonallat
 13. hungarian wildlife  = magyar.vadallat
 14. Fishes of Hungary = magyar.hal
 15. Birds of Hungary = magyar.madar
+16. Hungarian names of planets = magyar.bolygo
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
-4. Hungarian tram lines  magyar.villamos
+4. Hungarian tram lines = magyar.villamos
+5. Hunngarian names of Europian capitals, states = magyar.orszag
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators. 
        
@@ -74,18 +78,23 @@
 
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
     magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
     magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
     magyar.jaras :             {'megye' : (székhely, megye)}
-    magyar.villamos:    kulcs {'viszonylat', indulas, erkezes, menetido, varos}
-
+    magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
+    magyar.orszag:             {'orszag': 'főváros'}
 
+## Metódus
+   A  szótárakból választhatsz véletlenszerű KULCSOT. (szótár neve, elemek száma)
+                    
+    szotarbol_veletlen_kulcs(szotar, n)
 
+    pl: szotarbol_veletlen_kulcs(magyar.megye, 12)
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-2.9.3/magyar.py` & `magyar-2.9.4/magyar.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
          'menyhal', 'domolykó', 'keszeg', 'garda', 'paduc', 'compó', 'bodorka', 'nyúldomolykó']
 
 madar = ['feketerigó', 'fülemüle', 'csalogány', 'kékvércse', 'széncinege', 'szajkó', 'szürkebegy', 'búbosbanka',
          'zöldike', 'sármány', 'fácán', 'kakukk', 'bölömbika', 'örvényi sas', 'szirti sas', 'parlagi sas',
          'réti keselyű', 'héja', 'pávaszemes fecske', 'gyurgyalag', 'gólya', 'kócsag', 'hattyú', 'vadkacsa', 'vadlúd',
          'szárcsa', 'rigó', 'szajkó']
 
-
+bolygo =['Merkúr', 'Vénusz', 'Föld', 'Mars', 'Jupiter','Szaturnusz', 'Uránusz', 'Neptunusz']
 
 kiraly = {'Árpád': (895, 907), 'Zoltán': (907, 947), 'Fajsz': (947, 955), 'Taksony': (955, 972), 'Géza': (972, 997),
     'I.István': (997, 1038),'I. Péter': (1038, 1041), 'Sámuel': (1041, 1044), 'Péter-2': (1044, 1045), 'I.András': (1041, 1060),
     'I. Béla': (1060, 1063), 'Salamon': (1063, 1074), 'I. Géza': (1074, 1077), 'I. László': (1077, 1095),
     'Kálmán': (1095, 1116),'II. István': (1116, 1131), 'II. Béla': (1131, 1141), 'II. Géza': (1141,1162),
     'III. István': (1162, 1172), 'III. Béla': (1172, 1196), 'Imre':(1196, 1204), 'III. László': (1204, 1205),
     'II. András': (1205, 1235),'IV. Béla': (1235, 1270), 'V. István': (1270, 1272), 'IV. László': (1272, 1290),
@@ -204,15 +204,15 @@
     'Salgótarjáni járás': ['Salgótarján', 'Nógrád'], 'Szécsényi járás': ['Szécsény', 'Nógrád'],
     'Aszódi járás': ['Aszód', 'Pest'],'Budakeszi járás': ['Budakeszi', 'Pest'],
     'Ceglédi járás': ['Cegléd', 'Pest'],'Dabasi járás': ['Dabas', 'Pest'],
     'Dunakeszi járás': ['Dunakeszi', 'Pest'],'Érdi járás': ['Érd', 'Pest'],
     'Gödöllői járás': ['Gödöllő', 'Pest'], 'Gyáli járás': ['Gyál', 'Pest'],
     'Monori járás': ['Monor', 'Pest'],'Nagykátai járás': ['Nagykáta', 'Pest'],
     'Nagykőrösi járás': ['Nagykőrös', 'Pest'],'Pilisvörösvári járás': ['Pilisvörösvár', 'Pest'],
-     'Ráckevei járás': ['Ráckeve', 'Pest'], 'Szentendrei járás': ['Szentendre', 'Pest'],
+    'Ráckevei járás': ['Ráckeve', 'Pest'], 'Szentendrei járás': ['Szentendre', 'Pest'],
     'Szigetszentmiklósi járás': ['Szigetszentmiklós', 'Pest'],'Szobi járás': ['Szob', 'Pest'],
     'Váci járás': ['Vác', 'Pest'],'Vecsési járás': ['Vecsés', 'Pest'],
     'Barcsi járás': ['Barcs', 'Somogy'],  'Csurgói járás': ['Csurgó', 'Somogy'],
     'Fonyódi járás': ['Fonyód', 'Somogy'], 'Kaposvári járás': ['Kaposvár', 'Somogy'],
     'Marcali járás': ['Marcali', 'Somogy'], 'Nagyatádi járás': ['Nagyatád', 'Somogy'],
     'Siófoki járás': ['Siófok', 'Somogy'], 'Tabi járás': ['Tab', 'Somogy'],
     'Baktalórántházai járás': ['Baktalórántháza', 'Szabolcs-Szatmár-Bereg'],'Csengeri járás': ['Csenger', 'Szabolcs-Szatmár-Bereg'],
@@ -268,8 +268,34 @@
             "DKV2": {"viszonylat": 2, "indulas": "Nagyállomás", "erkezes": "Nagyállomás", "menetido": 44, "varos": "Debrecen"},
             "MVK1": {"viszonylat": 1, "indulas": "Tiszai pályaudvar", "erkezes": "Felső-Majláth", "menetido": 33,"varos": "Miskolc"},
             "MVK2": {"viszonylat": 2, "indulas": "Tiszai pályaudvar", "erkezes": "Újgyőri főtér", "menetido": 26,"varos": "Miskolc"},
             "SZKT1": {"viszonylat": 1, "indulas": "Szeged plaza", "erkezes": "Szeged vasútállomás", "menetido": 33, "varos": "Szeged"},
             "SZKT2": {"viszonylat": 2, "indulas": "Európa liget", "erkezes": "Szeged vasútállomás", "menetido": 33, "varos": "Szeged"},
 }
 
+orszag= {
+    "Albánia": "Tirana","Andorra": "Andorra város", "Ausztria": "Bécs", "Belgium": "Brüsszel",
+    "Bosznia és Hercegovina": "Szarajevó",  "Bulgária": "Szófia",  "Ciprus": "Nicosia",
+    "Csehország": "Prága",  "Dánia": "Koppenhága", "Észtország": "Tallinn", "Finnország": "Helsinki",
+    "Franciaország": "Párizs", "Görögország": "Athén", "Horvátország": "Zágráb", "Izland": "Reykjavík",
+    "Írország": "Dublin", "Koszovó": "Pristina", "Lengyelország": "Varsó", "Lettország": "Riga",
+    "Liechtenstein": "Vaduz",  "Litvánia": "Vilnius",  "Luxemburg": "Luxemburg",
+    "Magyarország": "Budapest",  "Málta": "Valletta",  "Moldova": "Kisinyov",  "Monaco": "Monaco",
+    "Montenegró": "Podgorica", "Németország": "Berlin", "Norvégia": "Oslo", "Olaszország": "Róma",
+    "Portugália": "Lisszabon", "Románia": "Bukarest", "San Marino": "San Marino",
+    "Spanyolország": "Madrid", "Svájc": "Bern",  "Svédország": "Stockholm",  "Szlovákia": "Pozsony",
+    "Szlovénia": "Ljubljana", "Törökország": "Ankara", "Ukrajna": "Kijev", "Vatikán": "Vatikánváros"
+}
+
+def szotarbol_veletlen_kulcs(szotar, n):
+    """
+        szotar (dict): A szótár, amelyből véletlenszerűen választunk kulcsokat.
+        n (int): A választandó kulcsok száma.
+    """
+    kulcsok = list(szotar.keys())
+    veletlen_kulcsok = []
+    for i in range(n):
+        kulcs_index = hash(str(i)) % len(kulcsok)
+        veletlen_kulcs = kulcsok[kulcs_index]
+        veletlen_kulcsok.append(veletlen_kulcs)
+    return veletlen_kulcsok
```

### Comparing `magyar-2.9.3/setup.py` & `magyar-2.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="2.9.3",
+    version="2.9.4",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian names...",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

