# Comparing `tmp/proteinTools-0.1.9.tar.gz` & `tmp/proteinTools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-0.1.9.tar", last modified: Thu Apr 13 06:59:48 2023, max compression
+gzip compressed data, was "proteinTools-1.0.1.tar", last modified: Mon Apr 17 19:48:06 2023, max compression
```

## Comparing `proteinTools-0.1.9.tar` & `proteinTools-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-13 06:59:48.494305 proteinTools-0.1.9/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-0.1.9/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-13 06:59:48.491640 proteinTools-0.1.9/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-0.1.9/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-13 06:59:48.420605 proteinTools-0.1.9/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    44440 2023-04-13 05:14:53.000000 proteinTools-0.1.9/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-0.1.9/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-13 06:59:48.479247 proteinTools-0.1.9/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-13 06:59:48.000000 proteinTools-0.1.9/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-13 06:59:48.000000 proteinTools-0.1.9/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-13 06:59:48.000000 proteinTools-0.1.9/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       48 2023-04-13 06:59:48.000000 proteinTools-0.1.9/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-13 06:59:48.000000 proteinTools-0.1.9/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-13 06:59:48.498353 proteinTools-0.1.9/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      512 2023-04-13 06:59:29.000000 proteinTools-0.1.9/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-17 19:48:06.768603 proteinTools-1.0.1/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.0.1/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-17 19:48:06.761246 proteinTools-1.0.1/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.0.1/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-17 19:48:06.595533 proteinTools-1.0.1/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    47068 2023-04-17 19:45:09.000000 proteinTools-1.0.1/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.0.1/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-17 19:48:06.733715 proteinTools-1.0.1/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-17 19:48:06.000000 proteinTools-1.0.1/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-17 19:48:06.000000 proteinTools-1.0.1/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-17 19:48:06.000000 proteinTools-1.0.1/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       48 2023-04-17 19:48:06.000000 proteinTools-1.0.1/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-17 19:48:06.000000 proteinTools-1.0.1/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-17 19:48:06.775256 proteinTools-1.0.1/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      512 2023-04-17 19:47:05.000000 proteinTools-1.0.1/setup.py
```

### Comparing `proteinTools-0.1.9/LICENSE` & `proteinTools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-0.1.9/proteinTools/PT.py` & `proteinTools-1.0.1/proteinTools/PT.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,20 +39,20 @@
 class residue:
     """
     Residue class
     
     This class contains the essential parameters of an individual residue in a protein structural file, including the child atoms, protein sidechain, residue index, and type of amino acid.
     """
     def __init__(self, amino_acid, index, chain):
-        
         self.amino_acid = amino_acid
         self.index = index
         self.atoms = []
         self.chain = chain
-            
+        self.structure = 'undefined'
+        
     @cached_property
     def center(self):
         """
         Residue Center of Mass
     
         This property returns the center of mass of the residue, which is generated from all atom components. 
     
@@ -158,14 +158,40 @@
             z += atom.z
             totmass += atom.mass
         x /= totmass
         y /= totmass
         z /= totmass
         return [x, y, z]
         
+    @cached_property
+    def radius(self):
+        """
+        Ligand Radius of Gyration
+    
+        This property returns the radius of gyration of the ligand, which is generated from all atom components. 
+    
+        Returns
+        -------
+        int
+            The radius of gyration of the ligand molecule
+        """
+        center = self.center
+        x, y, z, totmass = 0, 0, 0, 0
+        for atom in self.atoms:
+            x += pow(atom.x - center[0], 2) * atom.mass
+            y += pow(atom.y - center[1], 2) * atom.mass
+            z += pow(atom.z - center[2], 2) * atom.mass
+            totmass += atom.mass
+        x /= totmass
+        y /= totmass
+        z /= totmass
+        radius = pow(x + y + z, .5)
+        return radius
+        
+        
 #Main protein class
 class Protein:
     """
     Protein Class
 
     This class represents an individual protein, it's provided ID and relevant structural file (generated via Alphafold or scraped from RCSB), and analytical methods and properties for biostatistics and bioinformatics purposes.
     """
@@ -228,15 +254,15 @@
             else:
                 return self.residue_list[key]
         except IndexError:
             print('Residue index out of bounds!')
         except:
             print(traceback.format_exc())
             print('Protein file has not been downloaded yet! Download the protein with <protname>.download()')
-            )
+            
     def download(self, destination = os.getcwd()):
         """
         Download Protein
     
         This method allows the user to download the simulated structural file of the specific protein from Alphafold (if a non-PDB ID is given) or a true structural file from RCSB (if a specific PDB ID is provided). Can identify process cif/mmcif files as well as .pdb files. Downloading the protein also collects all residue and atom information from the structural file, populating the attributes of the protein class.
     
         Parameters
@@ -366,16 +392,18 @@
                         self.residue_list.append(res)
                     element = line[77:79].strip()
                     if element not in atom_keys:
                         element = element[:1]
                     atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), residue = res.chain + str(resnum), data = line)
                     res.atoms.append(atm)
             
-            #Generates ligands if PDB filetype and ligands in file
+            
             if self.ID_type == 'PDB':
+                #Generates ligands if PDB filetype and ligands in file
+                sheet, helix, chainkeys = [], [], list(self.chains.keys())
                 for count, line in enumerate(data):
                     if line[0:6] == 'HETATM':
                         ligands = line[17:20]
                         if ligands == 'HOH':
                             break
                         if ligands != curr_lig:
                             lignum = int(line[22:27])
@@ -385,14 +413,49 @@
                                 self.ligand_list.append(lig)
                                 current_ligand_index += 1
                             element = line[77:79].strip()
                         if element not in atom_keys:
                             element = element[:1]
                         atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), data = line)
                         self.ligand_list[current_ligand_index].atoms.append(atm)
+                     
+                    #Queries secondary structure  
+                    elif line[0:5] == 'SHEET':
+                        line = [i for i in line.split(' ') if i != '']
+                        start = int(line[5])
+                        end = int(line[8])
+                        chain = int(line[4])
+                        chainindex = chainkeys.index(chain)
+                        for i in range(0, chainindex):
+                            start += self.chains[chainkeys[i]]
+                            end += self.chains[chainkeys[i]]
+
+                        for i in range(start, end + 1):
+                            sheet.append(i)
+                    elif line[0:5] == 'HELIX':
+                        line = [i for i in line.split(' ') if i != '']
+                        start = int(line[5])
+                        end = int(line[8])
+                        chain = line[4]
+                        chainindex = chainkeys.index(chain)
+                        for i in range(0, chainindex):
+                            start += self.chains[chainkeys[i]]
+                            end += self.chains[chainkeys[i]]
+                        for i in range(start, end + 1):
+                            helix.append(i)
+                            
+                #Assigns secondary structure
+                for count, res in enumerate(self.residue_list):
+                    if count + 1 in sheet:
+                        res.structure = 'SHEET'
+                    elif count + 1 in helix:
+                        res.structure = 'HELIX'
+                    else:
+                        res.structure = 'UNSTRUCTURED'
+                        
         else:
             with open(self.protein + '.cif', 'r') as f:
                 data = f.readlines()
             
             #Obtains chains from protein file
             numbers, letters, curr_num = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9'], ['A', 'B',' C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z'], 1
             for count, line in enumerate(data):
@@ -1002,18 +1065,19 @@
             print(traceback.format_exc())
             return 'N/A'
     '''
     TODO
     - Add secondary structure prediction to residues (use s4pred?)
     - Add more ID conversions
     '''
+
 '''
 #For unit testing    
 if __name__ == '__main__':
     p = Protein('1HK4')
     p.download()
-    print(p.ligands)
+    print(p[1].structure)
     #new = Protein(p.Uniprot)
     #new.download()
     #print(new.interactions)
     #print(protein.interactions)
 '''
```

### Comparing `proteinTools-0.1.9/setup.py` & `proteinTools-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "0.1.9",
+    version = "1.0.1",
     author = "Christian de Frondeville",
     description = "Lightweight package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene']
 
 )
```

