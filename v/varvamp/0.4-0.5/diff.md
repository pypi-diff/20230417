# Comparing `tmp/varvamp-0.4.tar.gz` & `tmp/varvamp-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvamp-0.4.tar", last modified: Tue Mar 28 15:10:39 2023, max compression
+gzip compressed data, was "varvamp-0.5.tar", last modified: Sun Apr 16 15:24:48 2023, max compression
```

## Comparing `varvamp-0.4.tar` & `varvamp-0.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:10:39.530141 varvamp-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-28 15:10:39.530141 varvamp-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-03-28 15:10:22.000000 varvamp-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 15:10:39.530141 varvamp-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-28 15:10:22.000000 varvamp-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:10:39.526141 varvamp-0.4/varvamp/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:10:39.530141 varvamp-0.4/varvamp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/scripts/consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/scripts/conserved.py
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/scripts/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/scripts/primers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/scripts/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-03-28 15:10:22.000000 varvamp-0.4/varvamp/scripts/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 15:10:39.526141 varvamp-0.4/varvamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-28 15:10:39.000000 varvamp-0.4/varvamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-28 15:10:39.000000 varvamp-0.4/varvamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 15:10:39.000000 varvamp-0.4/varvamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-28 15:10:39.000000 varvamp-0.4/varvamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 15:10:39.000000 varvamp-0.4/varvamp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-28 15:10:39.000000 varvamp-0.4/varvamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-28 15:10:39.000000 varvamp-0.4/varvamp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:24:48.841364 varvamp-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-04-16 15:24:48.841364 varvamp-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-16 15:24:30.000000 varvamp-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 15:24:48.841364 varvamp-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-16 15:24:31.000000 varvamp-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:24:48.837364 varvamp-0.5/varvamp/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:24:48.837364 varvamp-0.5/varvamp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/scripts/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/scripts/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/scripts/conserved.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/scripts/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/scripts/primers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/scripts/qpcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/scripts/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-04-16 15:24:31.000000 varvamp-0.5/varvamp/scripts/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:24:48.837364 varvamp-0.5/varvamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-04-16 15:24:48.000000 varvamp-0.5/varvamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-16 15:24:48.000000 varvamp-0.5/varvamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:24:48.000000 varvamp-0.5/varvamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 15:24:48.000000 varvamp-0.5/varvamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:24:48.000000 varvamp-0.5/varvamp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-16 15:24:48.000000 varvamp-0.5/varvamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 15:24:48.000000 varvamp-0.5/varvamp.egg-info/top_level.txt
```

### Comparing `varvamp-0.4/PKG-INFO` & `varvamp-0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-Metadata-Version: 2.1
-Name: varvamp
-Version: 0.4
-Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
-Home-page: https://github.com/jonas-fuchs/varVAMP
-Author: Dr. Jonas Fuchs
-Author-email: jonas.fuchs@uniklinik-freiburg.de
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 **var**iable **V**irus**AMP**licons (varVAMP) is a tool to design primers for highly diverse viruses. The input is an alignment of your viral (full-genome) sequences.
 
 # varVAMP
+[![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
+[![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0)
+[![PiPy](https://img.shields.io/pypi/v/varvamp?label=pypi%20version)](https://pypi.org/project/varvamp/)
+[![PiPy](https://static.pepy.tech/personalized-badge/varvamp?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pypi.org/project/varvamp/)
+[![CONDA](https://img.shields.io/conda/v/bioconda/varvamp?label=conda%20version)](https://anaconda.org/bioconda/varvamp)
+[![CONDA](https://img.shields.io/conda/dn/bioconda/varvamp?label=conda%20downloads)](https://anaconda.org/bioconda/varvamp)
+<img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg /> 
 
-[![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0) <img src=https://img.shields.io/github/v/release/jonas-fuchs/varvamp /> <img src=https://img.shields.io/badge/language-%3Epython3.9-red />
 
-For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this, by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
+For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
 
 **varVAMP comes in three different flavors:**
 
 <img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/varvamp.png" alt="varVAMP logo" />
 
 **SANGER**: varVAMP searches for the very best primers and reports back non-overlapping amplicons which can be used for PCR-based screening approaches.
 
 **TILED**: varVAMP uses a graph based approach to design overlapping amplicons that tile the entire viral genome. This designs amplicons that are suitable for Oxford Nanopore or Illumina based full-genome sequencing.
 
-**QPCR** *(coming soon)*: varVAMP searches for small amplicons with an internal primer for the probe. It minimizes temperature differences between the primers.
+**QPCR**: varVAMP searches for small amplicons with an optimized internal probe (TaqMan). It minimizes temperature differences between the primers and checks for amplicon secondary structures.
 
 This program is currently being developed and in an alpha state. You are welcome to use this software. If you successfully design primers, drop me a mail. It might be possible to collaborate! Ideas and suggestions are highly welcome.
 
 # Documentation
 
 * [Installation](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/installation.md)
 * [Preparing the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md)
```

### Comparing `varvamp-0.4/setup.py` & `varvamp-0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     license_files=('LICENSE'),
     packages=find_packages(),
     install_requires=[
         "biopython>=1.79",
         "matplotlib>=3.5.1",
         "primer3-py>=1.1.0",
         "pandas>=1.4.4",
-        "numpy>=1.23.3"
+        "numpy>=1.23.3",
+        "seqfold>=0.7.15"
     ],
     description='Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses',
     url='https://github.com/jonas-fuchs/varVAMP',
     author='Dr. Jonas Fuchs',
     author_email='jonas.fuchs@uniklinik-freiburg.de',
     classifiers=[
         "Programming Language :: Python :: 3.9",
```

### Comparing `varvamp-0.4/varvamp/scripts/alignment.py` & `varvamp-0.5/varvamp/scripts/alignment.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.4/varvamp/scripts/config.py` & `varvamp-0.5/varvamp/scripts/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 """
-This contains all varVAMP parameters. Options that can be adjusted by arguments
-are FREQUENCY_THRESHOLD, PRIMER_ALLOWED_N_AMB, AMPLICON_MIN_OVERLAP, AMPLICON_OPT_LENGTH,
-AMPLICON_MAX_LENGTH.
+This contains all varVAMP parameters.
 """
 
-# CAN BE CHANGED
-
+# CAN BE CHANGED, DO NOT DELETE
 # basic primer parameters
-PRIMER_TMP = (57, 63, 60)  # temperatur (min, max, opt)
-PRIMER_GC_RANGE = (40, 60, 50)  # gc (min, max, opt)
-PRIMER_SIZES = (17, 27, 20)  # size (min, max, opt)
-PRIMER_MAX_POLYX = 4  # max number of polyx repeats
-PRIMER_MAX_DINUC_REPEATS = 4  # max number of dinucleotide repeats
-PRIMER_HAIRPIN = 47  # max melting temp for secondary structures
-PRIMER_MAX_GC_END = 3  # max GCs in the last 5 bases of the primer
-PRIMER_GC_CLAMP = 1  # min number of GC nucleotides at the very 3' end
-PRIMER_MIN_3_WITHOUT_AMB = 2  # min len of 3' without ambiguous charaters
+PRIMER_TMP = (57, 63, 60)  # melting temperatur (min, max, opt)
+PRIMER_GC_RANGE = (35, 65, 50)  # gc (min, max, opt)
+PRIMER_SIZES = (18, 24, 21)  # size (min, max, opt)
+PRIMER_MAX_POLYX = 3  # max number of polyx repeats
+PRIMER_MAX_DINUC_REPEATS = 3  # max number of dinucleotide repeats
+PRIMER_HAIRPIN = 47  # max melting temp for secondary structure
+PRIMER_GC_END = (0, 4)  # min/max GCs in the last 5 bases of the 3' end
+PRIMER_MIN_3_WITHOUT_AMB = 3  # min len of 3' without ambiguous charaters
 PRIMER_MAX_DIMER_TMP = 47  # max melting temp for dimers (homo- or heterodimers)
 
+# QPCR parameters
+# basic probe parameters
+QPROBE_TMP = (64, 70, 67)  # mean 7°C higher than the primer temp
+QPROBE_SIZES = (20, 30, 25)
+QPROBE_GC_RANGE = (40, 80, 60)
+QPROBE_GC_END = (0, 4)
+# constraints for amplicon design
+QPRIMER_DIFF = 2  # maximal temperature diff of qPCR primers
+QPROBE_TEMP_DIFF = (5, 10)  # min/max temp diff between probe and primers
+QPROBE_DISTANCE = (4, 15)  # min/max distance to the primer on the same strand
+QAMPLICON_LENGTH = (70, 200)  # min/max length of the qPCR amplicon
+QAMPLICON_GC = (40, 60)  # GC min/max of the qPCR amplicon
+QAMPLICON_DELTAG_CUTOFF = -1  # minimum free energy (kcal/mol/K) at the lowest primer temp
+
 # PCR parameters
-PCR_MV_CONC = 50  # monovalent cations mM
+PCR_MV_CONC = 100  # monovalent cations mM
 PCR_DV_CONC = 2  # divalent cations mM
 PCR_DNTP_CONC = 0.8  # dntp concentration mM
-PCR_DNA_CONC = 50  # primer concentration nM
+PCR_DNA_CONC = 15  # primer concentration nM
 
-# multipliers for primer base penalties
+# multipliers for primer and qpcr probe penalties
 PRIMER_TM_PENALTY = 2  # temperature penalty
 PRIMER_GC_PENALTY = 0.2  # gc penalty
 PRIMER_SIZE_PENALTY = 0.5  # size penalty
 PRIMER_MAX_BASE_PENALTY = 8  # max base penalty for a primer
-PRIMER_3_PENALTY = (10, 10, 10)  # penalties for 3' mismatches
+PRIMER_3_PENALTY = (32, 16, 8, 4, 2)  # penalties for 3' mismatches
 PRIMER_PERMUTATION_PENALTY = 0.1  # penalty for the number of permutations
 
 
 # DO NOT CHANGE
 # nucleotide definitions
-nucs = set("atcg")
-ambig_nucs = {
+NUCS = set("atcg")
+AMBIG_NUCS = {
     "r": ["a", "g"],
     "y": ["c", "t"],
     "s": ["g", "c"],
     "w": ["a", "t"],
     "k": ["g", "t"],
     "m": ["a", "c"],
     "b": ["c", "g", "t"],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `varvamp-0.4/varvamp/scripts/consensus.py` & `varvamp-0.5/varvamp/scripts/consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         nucleotide_list.append(sequence[1][idx])
     # count occurences of nucleotides
     counter = dict(collections.Counter(nucleotide_list))
     # get permutations of an ambiguous nucleotide
     to_delete = []
     temp_dict = {}
     for nucleotide in counter:
-        if nucleotide in config.ambig_nucs:
+        if nucleotide in config.AMBIG_NUCS:
             to_delete.append(nucleotide)
-            permutations = config.ambig_nucs[nucleotide]
+            permutations = config.AMBIG_NUCS[nucleotide]
             adjusted_freq = 1/len(permutations)
             for permutation in permutations:
                 if permutation in temp_dict:
                     temp_dict[permutation] += adjusted_freq
                 else:
                     temp_dict[permutation] = adjusted_freq
         if nucleotide == "-":
@@ -68,15 +68,15 @@
     return consensus_nucleotides
 
 
 def get_ambiguous_char(nucleotides):
     """
     get ambiguous char from a list of nucleotides
     """
-    for ambiguous, permutations in config.ambig_nucs.items():
+    for ambiguous, permutations in config.AMBIG_NUCS.items():
         if set(permutations) == set(nucleotides):
             return ambiguous
 
 
 def create_consensus(alignment, threshold):
     """
     build a majority sequence and a sequence that
```

### Comparing `varvamp-0.4/varvamp/scripts/conserved.py` & `varvamp-0.5/varvamp/scripts/conserved.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,28 +17,28 @@
     writable = False
     in_ambiguous_region = True
     last_amb = 0
     conserved_regions = []
 
     seq = str(consensus_amb) + 2*'N'
     for idx, nuc in enumerate(seq):
-        if in_ambiguous_region and nuc in config.nucs:
+        if in_ambiguous_region and nuc in config.NUCS:
             in_ambiguous_region = False
             # just entered a new stretch of non-ambiguous bases
             # may be time to open a new window
             if not current_window:
                 current_window = [idx, 0]
                 amb_pos = []
                 # create new window if none is there. First element
                 # keeps track of start of the window, second element is
                 # a counter that resets if two ambiguous chars are longer
                 # than specified apart and last one counts all ambiguous
                 # chars. also track all amb chars after a window has opened
             continue
-        if nuc not in config.nucs:
+        if nuc not in config.NUCS:
             if current_window:
                 in_ambiguous_region = True
                 amb_to_amb_len = idx - last_amb
                 if nuc != "N":
                     # track previous amb pos only if current pos is not a N as this
                     # region is witeable
                     amb_pos.append(idx)
@@ -95,23 +95,23 @@
 def digest_seq(seq, kmer_size):
     """
     digest the sequence into kmers
     """
     return[[seq[i:i+kmer_size], i, i+len(seq[i:i+kmer_size])] for i in range(len(seq)-kmer_size+1)]
 
 
-def produce_kmers(conserved_regions, consensus):
+def produce_kmers(conserved_regions, consensus, sizes=config.PRIMER_SIZES):
     """
     produce kmers for all conserved regions
     """
     kmers = []
 
     for region in conserved_regions:
         sliced_seq = consensus[region[0]:region[1]]
-        for kmer_size in range(config.PRIMER_SIZES[0], config.PRIMER_SIZES[1]+1):
+        for kmer_size in range(sizes[0], sizes[1]+1):
             kmers_temp = digest_seq(sliced_seq, kmer_size)
             # adjust the start and stop position of the kmers
             for kmer_temp in kmers_temp:
                 kmer_temp[1] = kmer_temp[1]+region[0]
                 kmer_temp[2] = kmer_temp[2]+region[0]
             kmers += kmers_temp
```

### Comparing `varvamp-0.4/varvamp/scripts/primers.py` & `varvamp-0.5/varvamp/scripts/primers.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,40 +101,23 @@
     check how many gc nucleotides
     are within the last 5 bases of
     the 3' end
     """
     return seq[-5:].count('g') + seq[-5:].count('c')
 
 
-def gc_clamp_present(seq):
-    """
-    checks if a gc clamp is present
-    """
-    if config.PRIMER_GC_CLAMP > 0:
-        for nuc in seq[-config.PRIMER_GC_CLAMP:]:
-            if nuc in "cg":
-                clamp_present = True
-            else:
-                clamp_present = False
-                break
-    else:
-        clamp_present = True
-
-    return clamp_present
-
-
 def is_three_prime_ambiguous(amb_seq):
     """
     determine if a sequence contains an ambiguous char at the 3'prime
     """
     len_3_prime = config.PRIMER_MIN_3_WITHOUT_AMB
 
     if len_3_prime != 0:
         for nuc in amb_seq[len(amb_seq)-len_3_prime:]:
-            if nuc not in config.nucs:
+            if nuc not in config.NUCS:
                 is_amb = True
                 break
             else:
                 is_amb = False
     else:
         is_amb = False
 
@@ -152,60 +135,60 @@
     """
     get all permutations of a primer with ambiguous
     nucleotides and multiply with permutation penalty
     """
     permutations = 0
 
     for nuc in amb_seq:
-        if nuc in config.ambig_nucs:
-            n = len(config.ambig_nucs[nuc])
+        if nuc in config.AMBIG_NUCS:
+            n = len(config.AMBIG_NUCS[nuc])
             if permutations != 0:
                 permutations = permutations*n
             else:
                 permutations = n
 
     return permutations*config.PRIMER_PERMUTATION_PENALTY
 
 
-def calc_base_penalty(seq):
+def calc_base_penalty(seq, primer_temps, gc_range, primer_sizes):
     """
     Calculate intrinsic primer penalty.
     """
     penalty = 0
 
     tm = calc_temp(seq)
     gc = calc_gc(seq)
     size = len(seq)
 
     # TEMP penalty
-    if tm > config.PRIMER_TMP[2]:
+    if tm > primer_temps[2]:
         penalty += config.PRIMER_TM_PENALTY*(
-            tm - config.PRIMER_TMP[2]
+            tm - primer_temps[2]
             )
-    if tm < config.PRIMER_TMP[2]:
+    if tm < primer_temps[2]:
         penalty += config.PRIMER_TM_PENALTY*(
-            config.PRIMER_TMP[2] - tm
+            primer_temps[2] - tm
             )
     # GC penalty
-    if gc > config.PRIMER_GC_RANGE[2]:
+    if gc > gc_range[2]:
         penalty += config.PRIMER_GC_PENALTY*(
-            gc - config.PRIMER_GC_RANGE[2]
+            gc - gc_range[2]
             )
-    if gc < config.PRIMER_GC_RANGE[2]:
+    if gc < gc_range[2]:
         penalty += config.PRIMER_GC_PENALTY*(
-            config.PRIMER_GC_RANGE[2] - gc
+            gc_range[2] - gc
         )
     # SIZE penalty
-    if size > config.PRIMER_SIZES[2]:
+    if size > primer_sizes[2]:
         penalty += config.PRIMER_SIZE_PENALTY*(
-            size - config.PRIMER_SIZES[2]
+            size - primer_sizes[2]
         )
-    if size < config.PRIMER_SIZES[2]:
+    if size < primer_sizes[2]:
         penalty += config.PRIMER_SIZE_PENALTY * (
-            config.PRIMER_SIZES[2] - size
+            primer_sizes[2] - size
         )
 
     return penalty
 
 
 def calc_per_base_mismatches(kmer, alignment, ambiguous_consensus):
     """
@@ -225,31 +208,31 @@
         seq_slice = sequence[1][kmer[1]:kmer[2]]
         for idx, slice_nuc in enumerate(seq_slice):
             # find the respective nuc to that of the slice
             current_kmer_pos = amb_kmer[idx]
             if slice_nuc == current_kmer_pos:
                 continue
             # check if the slice nucleotide is an amb pos
-            if slice_nuc in config.ambig_nucs:
+            if slice_nuc in config.AMBIG_NUCS:
                 # check if the kmer has an amb pos
-                if current_kmer_pos in config.ambig_nucs:
-                    slice_nuc_set = set(config.ambig_nucs[slice_nuc])
-                    pri_set = set(config.ambig_nucs[current_kmer_pos])
+                if current_kmer_pos in config.AMBIG_NUCS:
+                    slice_nuc_set = set(config.AMBIG_NUCS[slice_nuc])
+                    pri_set = set(config.AMBIG_NUCS[current_kmer_pos])
                     # check if these sets have no overlap
                     # -> mismatch
                     if len(slice_nuc_set.intersection(pri_set)) == 0:
                         mismatches[idx] += 1
                 # if no amb pos is in kmer then check if kmer nuc
                 # is part of the amb slice nuc
-                elif current_kmer_pos not in config.ambig_nucs[slice_nuc]:
+                elif current_kmer_pos not in config.AMBIG_NUCS[slice_nuc]:
                     mismatches[idx] += 1
             # check if kmer has an amb pos but the current
             # slice_nuc is not part of this amb nucleotide
-            elif current_kmer_pos in config.ambig_nucs:
-                if slice_nuc not in config.ambig_nucs[current_kmer_pos]:
+            elif current_kmer_pos in config.AMBIG_NUCS:
+                if slice_nuc not in config.AMBIG_NUCS[current_kmer_pos]:
                     mismatches[idx] += 1
             # mismatch
             else:
                 mismatches[idx] += 1
 
     # gives a percent mismatch over all positions of the kmer from 5' to 3'
     mismatches = [round(x/len(alignment), 2) for x in mismatches]
@@ -271,25 +254,25 @@
             penalty = sum([m * p for m, p in zip(mismatches[::-1][0:len(config.PRIMER_3_PENALTY)], config.PRIMER_3_PENALTY)])
     else:
         penalty = 0
 
     return(penalty)
 
 
-def filter_kmer_direction_independent(seq):
+def filter_kmer_direction_independent(seq, primer_temps=config.PRIMER_TMP, gc_range=config.PRIMER_GC_RANGE, primer_sizes=config.PRIMER_SIZES):
     """
     filter kmer for temperature, gc content,
     poly x, dinucleotide repeats and homodimerization
     """
     return(
-        (config.PRIMER_TMP[0] <= calc_temp(seq) <= config.PRIMER_TMP[1])
-        and (config.PRIMER_GC_RANGE[0] <= calc_gc(seq) <= config.PRIMER_GC_RANGE[1])
+        (primer_temps[0] <= calc_temp(seq) <= primer_temps[1])
+        and (gc_range[0] <= calc_gc(seq) <= gc_range[1])
         and (calc_max_polyx(seq) <= config.PRIMER_MAX_POLYX)
         and (calc_max_dinuc_repeats(seq) <= config.PRIMER_MAX_DINUC_REPEATS)
-        and (calc_base_penalty(seq) <= config.PRIMER_MAX_BASE_PENALTY)
+        and (calc_base_penalty(seq, primer_temps, gc_range, primer_sizes) <= config.PRIMER_MAX_BASE_PENALTY)
         and (calc_dimer(seq, seq).tm <= config.PRIMER_MAX_DIMER_TMP)
     )
 
 
 def filter_kmer_direction_dependend(direction, kmer, ambiguous_consensus):
     """
     filter for 3'ambiguous, hairpin temp and end GC content.
@@ -301,16 +284,15 @@
         amb_kmer_seq = ambiguous_consensus[kmer[1]:kmer[2]]
     elif direction == "-":
         kmer_seq = rev_complement(kmer[0])
         amb_kmer_seq = rev_complement(ambiguous_consensus[kmer[1]:kmer[2]])
     # filter kmer
     return(
         (calc_hairpin(kmer_seq).tm <= config.PRIMER_HAIRPIN)
-        and (calc_end_gc(kmer_seq) <= config.PRIMER_MAX_GC_END)
-        and gc_clamp_present(kmer_seq)
+        and (config.PRIMER_GC_END[0] <= calc_end_gc(kmer_seq) <= config.PRIMER_GC_END[1])
         and not is_three_prime_ambiguous(amb_kmer_seq)
     )
 
 
 def find_primers(kmers, ambiguous_consensus, alignment):
     """
     filter kmers direction specific and append penalties
@@ -320,15 +302,15 @@
     right_primer_candidates = []
 
     for kmer in kmers:
         # filter kmers based on their direction independend stats
         if not filter_kmer_direction_independent(kmer[0]):
             continue
         # calc base penalty
-        base_penalty = calc_base_penalty(kmer[0])
+        base_penalty = calc_base_penalty(kmer[0],config.PRIMER_TMP, config.PRIMER_GC_RANGE, config.PRIMER_SIZES)
         # calcualte per base mismatches
         per_base_mismatches = calc_per_base_mismatches(
                                 kmer,
                                 alignment,
                                 ambiguous_consensus
                             )
         # calculate permutation penealty
@@ -365,18 +347,18 @@
     creates a primer dictionary from primer list
     """
     primer_dict = {}
     primer_idx = 0
 
     for primer in primer_candidates:
         if direction == "+":
-            direction_name = "LEFT"
+            direction_name = "FW"
         elif direction == "-":
-            direction_name = "RIGHT"
-        primer_name = direction_name + "_" + str(primer_idx)
+            direction_name = "RW"
+        primer_name = f"{direction_name}_{primer_idx}"
         primer_dict[primer_name] = primer
         primer_idx += 1
 
     return primer_dict
 
 
 def find_best_primers(left_primer_candidates, right_primer_candidates):
```

### Comparing `varvamp-0.4/varvamp/scripts/scheme.py` & `varvamp-0.5/varvamp/scripts/scheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,17 +386,18 @@
         # some could be solved. lets check the updated scheme again.
         else:
             primer_dimers = test_scheme_for_dimers(amplicon_scheme)
 
     return not_solvable
 
 
-def find_best_amplicons(amplicons, all_primers, n):
+def find_sanger_amplicons(amplicons, all_primers, n):
     """
-    find the best scoring non-overlapping amplicons from all found amplicons
+    find the best scoring non-overlapping amplicons
+    from all found amplicons. only for the SANGER mode.
     """
     # sort amplicons
     sorted_amplicons = sorted(amplicons.items(), key=lambda x: x[1][5])
     to_retain = [sorted_amplicons[0]]
     amplicon_range = list(range(sorted_amplicons[0][1][0], sorted_amplicons[0][1][1]+1))
     amplicon_set = set(amplicon_range)
     # find lowest non-overlapping
```

### Comparing `varvamp-0.4/varvamp.egg-info/PKG-INFO` & `varvamp-0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.4
+Version: 0.5
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 **var**iable **V**irus**AMP**licons (varVAMP) is a tool to design primers for highly diverse viruses. The input is an alignment of your viral (full-genome) sequences.
 
 # varVAMP
+[![language](https://img.shields.io/badge/python-%3E3.9-green)](https://www.python.org/)
+[![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0)
+[![PiPy](https://img.shields.io/pypi/v/varvamp?label=pypi%20version)](https://pypi.org/project/varvamp/)
+[![PiPy](https://static.pepy.tech/personalized-badge/varvamp?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pypi.org/project/varvamp/)
+[![CONDA](https://img.shields.io/conda/v/bioconda/varvamp?label=conda%20version)](https://anaconda.org/bioconda/varvamp)
+[![CONDA](https://img.shields.io/conda/dn/bioconda/varvamp?label=conda%20downloads)](https://anaconda.org/bioconda/varvamp)
+<img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg /> 
 
-[![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0) <img src=https://img.shields.io/github/v/release/jonas-fuchs/varvamp /> <img src=https://img.shields.io/badge/language-%3Epython3.9-red />
 
-For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this, by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
+For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
 
 **varVAMP comes in three different flavors:**
 
 <img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/varvamp.png" alt="varVAMP logo" />
 
 **SANGER**: varVAMP searches for the very best primers and reports back non-overlapping amplicons which can be used for PCR-based screening approaches.
 
 **TILED**: varVAMP uses a graph based approach to design overlapping amplicons that tile the entire viral genome. This designs amplicons that are suitable for Oxford Nanopore or Illumina based full-genome sequencing.
 
-**QPCR** *(coming soon)*: varVAMP searches for small amplicons with an internal primer for the probe. It minimizes temperature differences between the primers.
+**QPCR**: varVAMP searches for small amplicons with an optimized internal probe (TaqMan). It minimizes temperature differences between the primers and checks for amplicon secondary structures.
 
 This program is currently being developed and in an alpha state. You are welcome to use this software. If you successfully design primers, drop me a mail. It might be possible to collaborate! Ideas and suggestions are highly welcome.
 
 # Documentation
 
 * [Installation](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/installation.md)
 * [Preparing the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md)
```

### Comparing `varvamp-0.4/varvamp.egg-info/SOURCES.txt` & `varvamp-0.5/varvamp.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 varvamp/scripts/__init__.py
 varvamp/scripts/alignment.py
 varvamp/scripts/config.py
 varvamp/scripts/consensus.py
 varvamp/scripts/conserved.py
 varvamp/scripts/logging.py
 varvamp/scripts/primers.py
+varvamp/scripts/qpcr.py
 varvamp/scripts/reporting.py
 varvamp/scripts/scheme.py
```

