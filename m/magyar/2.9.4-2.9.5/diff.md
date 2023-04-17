# Comparing `tmp/magyar-2.9.4.tar.gz` & `tmp/magyar-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.9.4.tar", last modified: Mon Apr 17 21:14:44 2023, max compression
+gzip compressed data, was "magyar-2.9.5.tar", last modified: Mon Apr 17 21:35:19 2023, max compression
```

## Comparing `magyar-2.9.4.tar` & `magyar-2.9.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-17 21:14:44.427517 magyar-2.9.4/
--rw-rw-r--   0 bela      (1000) bela      (1000)     3419 2023-04-17 21:14:44.427517 magyar-2.9.4/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     3048 2023-04-17 21:12:46.000000 magyar-2.9.4/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-17 21:14:44.427517 magyar-2.9.4/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     3419 2023-04-17 21:14:44.000000 magyar-2.9.4/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-17 21:14:44.000000 magyar-2.9.4/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-17 21:14:44.000000 magyar-2.9.4/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-17 21:14:44.000000 magyar-2.9.4/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    29782 2023-04-17 21:12:46.000000 magyar-2.9.4/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-17 21:14:44.427517 magyar-2.9.4/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-17 19:59:27.000000 magyar-2.9.4/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-17 21:35:19.640199 magyar-2.9.5/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     3884 2023-04-17 21:35:19.640199 magyar-2.9.5/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     3513 2023-04-17 21:33:22.000000 magyar-2.9.5/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-17 21:35:19.640199 magyar-2.9.5/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     3884 2023-04-17 21:35:19.000000 magyar-2.9.5/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-17 21:35:19.000000 magyar-2.9.5/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-17 21:35:19.000000 magyar-2.9.5/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-17 21:35:19.000000 magyar-2.9.5/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    31836 2023-04-17 21:33:22.000000 magyar-2.9.5/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-17 21:35:19.640199 magyar-2.9.5/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-17 21:33:22.000000 magyar-2.9.5/setup.py
```

### Comparing `magyar-2.9.4/PKG-INFO` & `magyar-2.9.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.4
+Version: 2.9.5
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,27 +15,28 @@
 
 ## Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
 1. vezetéknevek   =  magyar.vezeteknev
 2. női keresztnevek  = magyar.keresztnev_n
 3. férfi keresztnevek = magyar.keresztnev_f
-4. utcanevek = magyar.utca
-5. telelpülésnevek= magyar.telepules
-6. vármegyék nevei = magyar.megye
-7. folyók nevei = magyar.folyo
-8. a hét napjai = magyar.nap
-9. az év hónapjai = magyar.honap
-10. gyümölcsok = magyar.gyumolcs
-11. zöldségek = magyar.zoldseg
-12. haszonállatok = magyar.haszonallat
-13. vadallatok Magyarországon = magyar.vadallat
-14. Magyarország halai = magyar.hal
-15. Magyarország madarai = magyar.madar
-16. A naprendszer bolygóinak magyar neve = magyar.bolygo
+4. Vegyes magyar keresztnevek= magyar.keresztnev_v
+5. utcanevek = magyar.utca
+6. telelpülésnevek= magyar.telepules
+7. vármegyék nevei = magyar.megye
+8. folyók nevei = magyar.folyo
+9. a hét napjai = magyar.nap
+10. az év hónapjai = magyar.honap
+11. gyümölcsok = magyar.gyumolcs
+12. zöldségek = magyar.zoldseg
+13. haszonállatok = magyar.haszonallat
+14. vadallatok Magyarországon = magyar.vadallat
+15. Magyarország halai = magyar.hal
+16. Magyarország madarai = magyar.madar
+17. A naprendszer bolygóinak magyar neve = magyar.bolygo
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
@@ -85,16 +86,22 @@
     magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
     magyar.orszag:             {'orszag': 'főváros'}
 
 ## Metódus
    A  szótárakból választhatsz véletlenszerű KULCSOT. (szótár neve, elemek száma)
                     
     szotarbol_veletlen_kulcs(szotar, n)
+Pl:
+    import magyar
+    print(magyar.szotarbol_veletlen_kulcs(magyar.jaras,15))
+Eredmény:
+    ['Szekszárdi járás', 'Gönci járás', 'Szigetvári járás', 'Mezőkovácsházi járás', 'Bátonyterenyei járás',
+    'Körmendi járás', 'Váci járás', 'Edelényi járás', 'Pilisvörösvári járás', 'Kaposvári járás', 'Hódmezővásárhelyi járás',
+    'Hatvani járás', 'Törökszentmiklósi járás', 'Putnoki járás', 'Mezőkövesdi járás']
 
-    pl: szotarbol_veletlen_kulcs(magyar.megye, 12)
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-2.9.4/README.md` & `magyar-2.9.5/magyar.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,42 @@
+Metadata-Version: 2.1
+Name: magyar
+Version: 2.9.5
+Summary: Hungarian names...
+Home-page: https://github.com/kobanya/nevek
+Author: Nagy Béla
+Author-email: nagy.belabudapest@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # magyar
 
 
 ## Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
 1. vezetéknevek   =  magyar.vezeteknev
 2. női keresztnevek  = magyar.keresztnev_n
 3. férfi keresztnevek = magyar.keresztnev_f
-4. utcanevek = magyar.utca
-5. telelpülésnevek= magyar.telepules
-6. vármegyék nevei = magyar.megye
-7. folyók nevei = magyar.folyo
-8. a hét napjai = magyar.nap
-9. az év hónapjai = magyar.honap
-10. gyümölcsok = magyar.gyumolcs
-11. zöldségek = magyar.zoldseg
-12. haszonállatok = magyar.haszonallat
-13. vadallatok Magyarországon = magyar.vadallat
-14. Magyarország halai = magyar.hal
-15. Magyarország madarai = magyar.madar
-16. A naprendszer bolygóinak magyar neve = magyar.bolygo
+4. Vegyes magyar keresztnevek= magyar.keresztnev_v
+5. utcanevek = magyar.utca
+6. telelpülésnevek= magyar.telepules
+7. vármegyék nevei = magyar.megye
+8. folyók nevei = magyar.folyo
+9. a hét napjai = magyar.nap
+10. az év hónapjai = magyar.honap
+11. gyümölcsok = magyar.gyumolcs
+12. zöldségek = magyar.zoldseg
+13. haszonállatok = magyar.haszonallat
+14. vadallatok Magyarországon = magyar.vadallat
+15. Magyarország halai = magyar.hal
+16. Magyarország madarai = magyar.madar
+17. A naprendszer bolygóinak magyar neve = magyar.bolygo
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
@@ -73,18 +86,24 @@
     magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
     magyar.orszag:             {'orszag': 'főváros'}
 
 ## Metódus
    A  szótárakból választhatsz véletlenszerű KULCSOT. (szótár neve, elemek száma)
                     
     szotarbol_veletlen_kulcs(szotar, n)
+Pl:
+    import magyar
+    print(magyar.szotarbol_veletlen_kulcs(magyar.jaras,15))
+Eredmény:
+    ['Szekszárdi járás', 'Gönci járás', 'Szigetvári járás', 'Mezőkovácsházi járás', 'Bátonyterenyei járás',
+    'Körmendi járás', 'Váci járás', 'Edelényi járás', 'Pilisvörösvári járás', 'Kaposvári járás', 'Hódmezővásárhelyi járás',
+    'Hatvani járás', 'Törökszentmiklósi járás', 'Putnoki járás', 'Mezőkövesdi járás']
 
-    pl: szotarbol_veletlen_kulcs(magyar.megye, 12)
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
-Oktatási célra készült, szabadon használható.
+Oktatási célra készült, szabadon használható.
```

### Comparing `magyar-2.9.4/magyar.py` & `magyar-2.9.5/magyar.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,34 @@
                 'József', 'Kálmán', 'Károly', 'Kázmér', 'Kelemen', 'Kende', 'Kornél', 'Kristóf',
                 'Lajos', 'László', 'Levente', 'Lóránt', 'Lóránd', 'Lukács', 'Márió', 'Márk', 'Márton', 'Mátyás',
                 'Miklós', 'Milán', 'Mózes', 'Nándor', 'Nikolasz', 'Noé', 'Norbert', 'Olivér', 'Ödön', 'Oszkár',
                 'Ottó', 'Pál', 'Patrik', 'Péter', 'Róbert', 'Rudolf', 'Sámuel', 'Sándor', 'Sebestyén', 'Soma',
                 'Szabolcs', 'Szilárd', 'Szilveszter', 'Tamás', 'Tihamér', 'Tibor', 'Tivadar', 'Tódor', 'Tóbiás',
                 'Vencel', 'Viktor', 'Vilmos', 'Vince', 'Zalán', 'Zétény', 'Zoltán', 'Zsigmond', 'Zsolt']
 
+keresztnev_v =['Ábel', 'Ádám', 'Ákos', 'Aladár', 'Albert', 'Albin', 'Alekszander', 'Alfréd', 'Ambrus', 'Andor',
+                'András', 'Áron', 'Árpád', 'Attila', 'Aurél', 'Bálint', 'Barna', 'Barnabás', 'Béla', 'Benedek',
+                'Benjámin', 'Bernát', 'Botond', 'Csongor', 'Dénes', 'Dániel', 'Dávid', 'Dezső', 'Dominik', 'Donát',
+                'Edgár', 'Edmund', 'Ede', 'Eduárd', 'Endre', 'Erik', 'Ernő', 'Fábián', 'Farkas', 'Ferenc', 'Flórián',
+                'Gábor', 'Géza', 'Gergely', 'Gusztáv', 'György', 'Győző', 'Hunor', 'Igor', 'Imre', 'István', 'János',
+                'József', 'Kálmán', 'Károly', 'Kázmér', 'Kelemen', 'Kende', 'Kornél', 'Kristóf',
+                'Lajos', 'László', 'Levente', 'Lóránt', 'Lóránd', 'Lukács', 'Márió', 'Márk', 'Márton', 'Mátyás',
+                'Miklós', 'Milán', 'Mózes', 'Nándor', 'Nikolasz', 'Noé', 'Norbert', 'Olivér', 'Ödön', 'Oszkár',
+                'Ottó', 'Pál', 'Patrik', 'Péter', 'Róbert', 'Rudolf', 'Sámuel', 'Sándor', 'Sebestyén', 'Soma',
+                'Szabolcs', 'Szilárd', 'Szilveszter', 'Tamás', 'Tihamér', 'Tibor', 'Tivadar', 'Tódor', 'Tóbiás',
+                'Vencel', 'Viktor', 'Vilmos', 'Vince', 'Zalán', 'Zétény', 'Zoltán', 'Zsigmond', 'Zsolt',
+               'Anna', 'Cecília', 'Erika', 'Hanna', 'Katalin', 'Mária', 'Nóra', 'Orsolya', 'Réka', 'Szilvia',
+               'Tünde', 'Viktória', 'Dóra', 'Eszter', 'Flóra', 'Hajnalka', 'Izabella', 'Jázmin', 'Kamilla', 'Nikolett',
+               'Panna', 'Rita', 'Sarolta', 'Zsófia', 'Ágota', 'Csilla', 'Lilla', 'Orsolya', 'Panna',
+               'Szandra', 'Tamara', 'Ágnes', 'Júlia', 'Kincső', 'Babett', 'Barbara', 'Beáta', 'Bianka',
+               'Blanka', 'Boglárka', 'Borbála', 'Boróka', 'Brigitta', 'Bernadett', 'Bettina', 'Berta', 'Betti',
+               'Bianka', 'Cecília', 'Cintia', 'Csenge', 'Csilla', 'Detti', 'Diana', 'Dóra', 'Dalma', 'Daniella',
+               'Debóra', 'Dolli', 'Dominika'
+               ]
+
 utca = ['Ady Endre utca', 'Akácfa utca', 'Alkotmány utca', 'Almássy tér', 'Andrássy út', 'Apáczai Csere János utca',
         'Aradi utca', 'Árpád fejedelem útja', 'Attila utca', 'Bajcsy-Zsilinszky út', 'Balassi Bálint utca',
         'Baross utca', 'Bartók Béla út', 'Batthyány tér', 'Bécsi utca', 'Belgrád rakpart', 'Bethlen Gábor tér',
         'Béke tér', 'Bem rakpart', 'Benczúr utca', 'Bérkocsis utca', 'Berzsenyi utca', 'Bihari utca', 'Bocskai utca',
         'Budaörsi út', 'Csarnok tér', 'Csévi utca', 'Csillaghegyi út', 'Csokonai utca', 'Csömöri utca', 'Dandár utca',
         'Darázs utca', 'Deák Ferenc utca', 'Dózsa György út', 'Egyetem tér', 'Erzsébet körút', 'Erzsébet tér',
         'Fadrusz utca', 'Fehérvári út', 'Kőrösi Csoma Sándor út', 'Ferenciek tere', 'Ferenc körút', 'Ferenc tér',
```

### Comparing `magyar-2.9.4/setup.py` & `magyar-2.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="2.9.4",
+    version="2.9.5",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian names...",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

