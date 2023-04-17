# Comparing `tmp/papers-cli-v1.0.tar.gz` & `tmp/papers-cli-v1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/papers-cli-v1.0.tar", last modified: Wed Mar 10 17:30:48 2021, max compression
+gzip compressed data, was "papers-cli-v1.0.1.tar", last modified: Wed Jul  7 14:49:10 2021, max compression
```

## Comparing `papers-cli-v1.0.tar` & `papers-cli-v1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 perrette  (1000) perrette  (1000)        0 2021-03-10 17:30:48.166218 papers-cli-v1.0/
--rw-rw-r--   0 perrette  (1000) perrette  (1000)      453 2021-03-10 17:30:48.166218 papers-cli-v1.0/PKG-INFO
-drwxrwxr-x   0 perrette  (1000) perrette  (1000)        0 2021-03-10 17:30:48.166218 papers-cli-v1.0/papers/
--rw-rw-r--   0 perrette  (1000) perrette  (1000)      168 2017-11-17 09:42:54.279964 papers-cli-v1.0/papers/__init__.py
--rw-rw-r--   0 perrette  (1000) perrette  (1000)      496 2021-03-10 17:30:48.166218 papers-cli-v1.0/papers/_version.py
--rw-rw-r--   0 perrette  (1000) perrette  (1000)    52278 2021-03-10 14:59:24.407477 papers-cli-v1.0/papers/bib.py
--rw-r--r--   0 perrette  (1000) perrette  (1000)     8951 2020-02-17 17:43:35.442570 papers-cli-v1.0/papers/config.py
--rw-rw-r--   0 perrette  (1000) perrette  (1000)    18884 2020-02-17 17:16:13.922649 papers-cli-v1.0/papers/duplicate.py
--rw-rw-r--   0 perrette  (1000) perrette  (1000)     3132 2018-06-26 19:47:57.698296 papers-cli-v1.0/papers/encoding.py
--rw-rw-r--   0 perrette  (1000) perrette  (1000)    12151 2021-03-10 16:11:50.962333 papers-cli-v1.0/papers/extract.py
--rw-rw-r--   0 perrette  (1000) perrette  (1000)    98547 2017-11-17 09:42:54.435964 papers-cli-v1.0/papers/latexenc.py
-drwxrwxr-x   0 perrette  (1000) perrette  (1000)        0 2021-03-10 17:30:48.166218 papers-cli-v1.0/scripts/
--rw-rw-r--   0 perrette  (1000) perrette  (1000)       90 2017-11-17 09:42:54.635964 papers-cli-v1.0/scripts/papers
--rw-rw-r--   0 perrette  (1000) perrette  (1000)      529 2021-03-10 15:32:49.069426 papers-cli-v1.0/setup.cfg
--rw-rw-r--   0 perrette  (1000) perrette  (1000)      639 2021-03-10 17:14:17.644755 papers-cli-v1.0/setup.py
--rw-rw-r--   0 perrette  (1000) perrette  (1000)    68587 2017-11-17 09:42:54.631964 papers-cli-v1.0/versioneer.py
+drwxrwxr-x   0 perrette  (1000) perrette  (1000)        0 2021-07-07 14:49:10.269550 papers-cli-v1.0.1/
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)      457 2021-07-07 14:49:10.269550 papers-cli-v1.0.1/PKG-INFO
+drwxrwxr-x   0 perrette  (1000) perrette  (1000)        0 2021-07-07 14:49:10.269550 papers-cli-v1.0.1/papers/
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)      168 2017-11-17 09:42:54.279964 papers-cli-v1.0.1/papers/__init__.py
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)      498 2021-07-07 14:49:10.269550 papers-cli-v1.0.1/papers/_version.py
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)    52149 2021-07-07 13:36:36.712921 papers-cli-v1.0.1/papers/bib.py
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)     8951 2021-07-07 13:32:46.613754 papers-cli-v1.0.1/papers/config.py
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)    18884 2021-07-07 13:32:46.613754 papers-cli-v1.0.1/papers/duplicate.py
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)     3132 2018-06-26 19:47:57.698296 papers-cli-v1.0.1/papers/encoding.py
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)    12151 2021-07-07 13:32:46.613754 papers-cli-v1.0.1/papers/extract.py
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)    98547 2017-11-17 09:42:54.435964 papers-cli-v1.0.1/papers/latexenc.py
+drwxrwxr-x   0 perrette  (1000) perrette  (1000)        0 2021-07-07 14:49:10.269550 papers-cli-v1.0.1/scripts/
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)       90 2017-11-17 09:42:54.635964 papers-cli-v1.0.1/scripts/papers
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)      529 2021-03-11 12:22:01.244116 papers-cli-v1.0.1/setup.cfg
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)      639 2021-03-11 12:22:01.244116 papers-cli-v1.0.1/setup.py
+-rw-rw-r--   0 perrette  (1000) perrette  (1000)    68587 2017-11-17 09:42:54.631964 papers-cli-v1.0.1/versioneer.py
```

### Comparing `papers-cli-v1.0/papers/bib.py` & `papers-cli-v1.0.1/papers/bib.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,28 +63,28 @@
     assert Key not in keys, 'not enough letters in the alphabets to solve key conflict? or maybe something went wrong...'
     return Key
 
 
 def generate_key(entry, nauthor=NAUTHOR, ntitle=NTITLE, minwordlen=3, mintitlen=4, keys=None):
     # names = bibtexparser.customization.getnames(entry.get('author','unknown').lower().split(' and '))
     names = family_names(entry.get('author','unknown').lower())
-    authortag = '_'.join([nm for nm in names[:nauthor]]) 
-    yeartag = entry.get('year','0000') 
+    authortag = '_'.join([nm for nm in names[:nauthor]])
+    yeartag = entry.get('year','0000')
     if not ntitle or not entry.get('title',''):
         titletag = ''
     else:
         words = [word for word in entry['title'].lower().strip().split() if len(word) >= minwordlen]
         while len(u''.join(words[:ntitle])) < mintitlen and ntitle < len(words):
             ntitle += 1
         titletag = '_'.join(words[:ntitle])
     key = authortag + yeartag + titletag
     if keys and key in keys: # and not isinstance(keys, set):
         key = append_abc(key, keys)
     return key
- 
+
 
 # DUPLICATE DEFINITION
 # ====================
 
 def _remove_unicode(s, replace='_'):
     s2 = []
     for c in s:
@@ -136,15 +136,15 @@
     """assess two entries' similarity
     """
     if e1 == e2:
         return EXACT_DUPLICATES
 
     id1 = entry_id(e1)
     id2 = entry_id(e2)
-    
+
     logger.debug('{} ?= {}'.format(id1, id2))
 
     if id1 == id2:
         score = GOOD_DUPLICATES
 
     elif all([f1==f2 for f1, f2 in zip(id1, id2) if f1 and f2]): # all defined fields agree
         score = FAIR_DUPLICATES
@@ -167,15 +167,15 @@
     level = dict(
         EXACT = EXACT_DUPLICATES,
         GOOD = GOOD_DUPLICATES,
         FAIR = FAIR_DUPLICATES,
         PARTIAL = PARTIAL_DUPLICATES,
         FUZZY = FUZZY_DUPLICATES,
         )
-    try: 
+    try:
         target = level[similarity]
     except KeyError:
         raise ValueError('similarity must be one of EXACT, GOOD, FAIR, PARTIAL, FUZZY')
 
     score = compare_entries(e1, e2, fuzzy=level==FUZZY_DUPLICATES)
     logger.debug('score: {}, target: {}, similarity: {}'.format(score, target, similarity))
     return score >= target
@@ -293,31 +293,31 @@
         else:
             logger.debug('check duplicates : FALSE')
 
         i = self.index_sorted(entry)  # based on current sort key (e.g. ID)
 
         if i < len(self.entries) and self.key(self.entries[i]) == self.key(entry):
             logger.info('key duplicate: '+self.key(self.entries[i]))
-            
+
             if update_key:
                 newkey = self.append_abc_to_key(entry)  # add abc
                 logger.info('update key: {} => {}'.format(entry['ID'], newkey))
                 entry['ID'] = newkey
 
             else:
                 raise DuplicateKeyError('this error can be avoided if update_key is True')
-       
-        else: 
+
+        else:
             logger.info('new entry: '+self.key(entry))
-        
+
         self.entries.insert(i, entry)
 
 
     def insert_entry_check(self, entry, update_key=False, mergefiles=True, on_conflict='i'):
-        
+
         duplicates = [e for e in self.entries if self.eq(e, entry)]
 
         if not duplicates:
             logger.debug('not a duplicate')
             self.insert_entry(entry, update_key)
 
 
@@ -379,15 +379,15 @@
 
     def fetch_doi(self, doi, **kw):
         bibtex = fetch_bibtex_by_doi(doi)
         self.add_bibtex(bibtex, **kw)
 
 
     def add_pdf(self, pdf, attachments=None, rename=False, copy=False, search_doi=True, search_fulltext=True, scholar=False, **kw):
-        
+
         bibtex = extract_pdf_metadata(pdf, search_doi, search_fulltext, scholar=scholar)
 
         bib = bibtexparser.loads(bibtex)
         entry = bib.entries[0]
 
         files = [pdf]
         if attachments:
@@ -399,39 +399,39 @@
 
         kw.pop('update_key', True)
             # logger.warn('fetched key is always updated when adding PDF to existing bib')
         self.insert_entry(entry, update_key=True, **kw)
 
         if rename:
             self.rename_entry_files(entry, copy=copy)
-            
+
 
     def scan_dir(self, direc, search_doi=True, search_fulltext=True, **kw):
-        
+
         for root, direcs, files in os.walk(direc):
             dirname = os.path.basename(root)
             if dirname.startswith('.'): continue
             if dirname.startswith('_'): continue
-        
+
             # maybe a special entry directory?
             if os.path.exists(hidden_bibtex(root)):
                 logger.debug('read from hidden bibtex')
                 try:
                     entry = read_entry_dir(root)
                     self.insert_entry(entry, **kw)
-                except Exception:  
+                except Exception:
                     logger.warn(root+'::'+str(error))
-                continue 
+                continue
 
             for file in files:
                 if file.startswith('.'):
                     continue
                 path = os.path.join(root, file)
                 try:
-                    if file.endswith('.pdf'): 
+                    if file.endswith('.pdf'):
                         self.add_pdf(path, search_doi=search_doi, search_fulltext=search_fulltext, **kw)
                     elif file.endswith('.bib'):
                         self.add_bibtex_file(path, **kw)
                 except Exception as error:
                     logger.warn(path+'::'+str(error))
                     continue
 
@@ -523,16 +523,16 @@
             try:
                 self.rename_entry_files(e, copy)
             except Exception as error:
                 logger.error(str(error))
                 continue
 
 
-    def fix_entry(self, e, fix_doi=True, fetch=False, fetch_all=False, 
-        fix_key=False, auto_key=False, key_ascii=False, encoding=None, 
+    def fix_entry(self, e, fix_doi=True, fetch=False, fetch_all=False,
+        fix_key=False, auto_key=False, key_ascii=False, encoding=None,
         format_name=True, interactive=False):
 
         e_old = e.copy()
 
         if format_name:
             for k in ['author','editor']:
                 if k in e:
@@ -588,18 +588,18 @@
                 kw['author'] = ' '.join(family_names(e['author']))
                 logger.info(e.get('ID','')+': fetch-all: '+str(kw))
                 try:
                     bibtex = fetch_bibtex_by_fulltext_crossref('', **kw)
                 except Exception as error:
                     logger.warn('...failed to fetch/update bibtex (all): '+str(error))
 
-            if bibtex:                        
+            if bibtex:
                 db = bibtexparser.loads(bibtex)
                 e2 = db.entries[0]
-                self.fix_entry(e2, encoding=encoding, format_name=True) 
+                self.fix_entry(e2, encoding=encoding, format_name=True)
                 strip_e = lambda e_: {k:e_[k] for k in e_ if k not in ['ID', 'file'] and k in e2}
                 if strip_e(e) != strip_e(e2):
                     logger.info('...fetch-update entry')
                     e.update(strip_e(e2))
                 else:
                     logger.info('...fetch-update: already up to date')
 
@@ -654,20 +654,20 @@
     if not isvaliddoi(doi):
         raise ValueError(e['ID']+': invalid parsed doi: '+doi)
 
     if doi.lower() != e['doi'].lower():
         raise ValueError(e['ID']+': doi: entry <=> pdf : {} <=> {}'.format(e['doi'].lower(), doi.lower()))
 
 
-def entry_filecheck(e, delete_broken=False, fix_mendeley=False, 
+def entry_filecheck(e, delete_broken=False, fix_mendeley=False,
     check_hash=False, check_metadata=False, interactive=True, image=False):
 
     if 'file' not in e:
         return
-    
+
     if check_hash:
         import hashlib
 
     newfiles = []
     hashes = set()
     realpaths = set()
     fixed = {}
@@ -675,32 +675,32 @@
     for i, file in enumerate(parse_file(e['file'])):
 
         realpath = os.path.realpath(file)
         if realpath in realpaths:
             logger.info(e['ID']+': remove duplicate path: "{}"'.format(fixed.get(file, file)))
             continue
         realpaths.add(realpath) # put here so that for identical
-                                   # files that are checked and finally not 
-                                   # included, the work is done only once 
+                                   # files that are checked and finally not
+                                   # included, the work is done only once
 
         if fix_mendeley and not os.path.exists(file):
             old = file
 
             # replace any "{\_}" with "_"
             try:
                 file = latex_to_unicode(file)
             except KeyError as error:
                 logger.warn(e['ID']+': '+str(error)+': failed to convert latex symbols to unicode: '+file)
 
             # fix root (e.g. path starts with home instead of /home)
             dirname = os.path.dirname(file)
             candidate = os.path.sep + file
             if (not file.startswith(os.path.sep) and dirname # only apply when some directory name is specified
-                and not os.path.exists(dirname) 
-                and os.path.exists(os.path.dirname(candidate))): # simply requires that '/'+directory exists 
+                and not os.path.exists(dirname)
+                and os.path.exists(os.path.dirname(candidate))): # simply requires that '/'+directory exists
                 # and os.path.exists(newfile)):
                     # logger.info('prepend "/" to file name: "{}"'.format(file))
                     file = candidate
 
             if old != file:
                 logger.info(e['ID']+u': file name fixed: "{}" => "{}".'.format(old, file))
                 fixed[old] = file # keep record of fixed files
@@ -762,59 +762,59 @@
     egrp.add_argument('--debug', action='store_const', dest='logging_level', const=logging.DEBUG)
     egrp.add_argument('--info', action='store_const', dest='logging_level', const=logging.INFO)
     egrp.add_argument('--warn', action='store_const', dest='logging_level', const=logging.WARN)
     egrp.add_argument('--error', action='store_const', dest='logging_level', const=logging.ERROR)
 
     cfg = argparse.ArgumentParser(add_help=False, parents=[loggingp])
     grp = cfg.add_argument_group('config')
-    grp.add_argument('--filesdir', default=config.filesdir, 
+    grp.add_argument('--filesdir', default=config.filesdir,
         help='files directory (default: %(default)s)')
     grp.add_argument('--bibtex', default=config.bibtex,
         help='bibtex database (default: %(default)s)')
-    grp.add_argument('--dry-run', action='store_true', 
+    grp.add_argument('--dry-run', action='store_true',
         help='no PDF renaming/copying, no bibtex writing on disk (for testing)')
 
     # status
     # ======
-    statusp = subparsers.add_parser('status', 
+    statusp = subparsers.add_parser('status',
         description='view install status',
         parents=[cfg])
     statusp.add_argument('--no-check-files', action='store_true', help='faster, less info')
     statusp.add_argument('-v','--verbose', action='store_true', help='app status info')
 
     def statuscmd(o):
         if o.bibtex:
             config.bibtex = o.bibtex
         if o.filesdir is not None:
-            config.filesdir = o.filesdir        
+            config.filesdir = o.filesdir
         print(config.status(check_files=not o.no_check_files, verbose=o.verbose))
-        
+
 
     # install
     # =======
 
     installp = subparsers.add_parser('install', description='setup or update papers install',
         parents=[cfg])
-    installp.add_argument('--reset-paths', action='store_true') 
+    installp.add_argument('--reset-paths', action='store_true')
     # egrp = installp.add_mutually_exclusive_group()
-    installp.add_argument('--local', action='store_true', 
-        help="""save config file in current directory (global install by default). 
-        This file will be loaded instead of the global configuration file everytime 
-        papers is executed from this directory. This will affect the default bibtex file, 
+    installp.add_argument('--local', action='store_true',
+        help="""save config file in current directory (global install by default).
+        This file will be loaded instead of the global configuration file everytime
+        papers is executed from this directory. This will affect the default bibtex file,
         the files directory, as well as the git-tracking option. Note this option does
         not imply anything about the actual location of bibtex file and files directory.
         """)
-    installp.add_argument('--git', action='store_true', 
-        help="""Track bibtex files with git. 
+    installp.add_argument('--git', action='store_true',
+        help="""Track bibtex files with git.
         Each time the bibtex is modified, a copy of the file is saved in a git-tracked
-        global directory (see papers status), and committed. Note the original bibtex name is 
+        global directory (see papers status), and committed. Note the original bibtex name is
         kept, so that different files can be tracked simultaneously, as long as the names do
         not conflict. This option is mainly useful for backup purposes (local or remote).
         Use in combination with `papers git`'
-        """) 
+        """)
     installp.add_argument('--gitdir', default=config.gitdir, help='default: %(default)s')
 
     grp = installp.add_argument_group('status')
     # grp.add_argument('-l','--status', action='store_true')
     # grp.add_argument('-v','--verbose', action='store_true')
     # grp.add_argument('-c','--check-files', action='store_true')
     grp.add_argument('--no-check-files', action='store_true', help='faster, less info')
@@ -902,43 +902,43 @@
     # ===
     addp = subparsers.add_parser('add', description='add PDF(s) or bibtex(s) to library',
         parents=[cfg])
     addp.add_argument('file', nargs='+')
     # addp.add_argument('-f','--force', action='store_true', help='disable interactive')
 
     grp = addp.add_argument_group('duplicate check')
-    grp.add_argument('--no-check-duplicate', action='store_true', 
+    grp.add_argument('--no-check-duplicate', action='store_true',
         help='disable duplicate check (faster, create duplicates)')
-    grp.add_argument('--no-merge-files', action='store_true', 
+    grp.add_argument('--no-merge-files', action='store_true',
         help='distinct "file" field considered a conflict, all other things being equal')
-    grp.add_argument('-u', '--update-key', action='store_true', 
+    grp.add_argument('-u', '--update-key', action='store_true',
         help='update added key according to any existing duplicate (otherwise an error might be raised on identical insert key)')
     # grp.add_argument('-f', '--force', action='store_true', help='no interactive')
     grp.add_argument('-m', '--mode', default='i', choices=['u', 'U', 'o', 's', 'r', 'i','a'],
-        help='''if duplicates are found, the default is to start an (i)nteractive dialogue, 
+        help='''if duplicates are found, the default is to start an (i)nteractive dialogue,
         unless "mode" is set to (r)aise, (s)skip new, (u)pdate missing, (U)pdate with new, (o)verwrite completely.
         ''')
 
     grp = addp.add_argument_group('directory scan')
-    grp.add_argument('--recursive', action='store_true', 
+    grp.add_argument('--recursive', action='store_true',
         help='accept directory as argument, for recursive scan \
         of .pdf files (bibtex files are ignored in this mode')
-    grp.add_argument('--ignore-errors', action='store_true', 
+    grp.add_argument('--ignore-errors', action='store_true',
         help='ignore errors when adding multiple files')
 
     grp = addp.add_argument_group('pdf metadata')
     grp.add_argument('--no-query-doi', action='store_true', help='do not attempt to parse and query doi')
     grp.add_argument('--no-query-fulltext', action='store_true', help='do not attempt to query fulltext in case doi query fails')
     grp.add_argument('--scholar', action='store_true', help='use google scholar instead of crossref')
 
     grp = addp.add_argument_group('attached files')
     grp.add_argument('-a','--attachment', nargs='+', help=argparse.SUPPRESS) #'supplementary material')
-    grp.add_argument('-r','--rename', action='store_true', 
+    grp.add_argument('-r','--rename', action='store_true',
         help='rename PDFs according to key')
-    grp.add_argument('-c','--copy', action='store_true', 
+    grp.add_argument('-c','--copy', action='store_true',
         help='copy file instead of moving them')
 
 
 
     def addcmd(o):
 
         if os.path.exists(o.bibtex):
@@ -946,54 +946,54 @@
         else:
             my = Biblio.newbib(o.bibtex, o.filesdir)
 
         if len(o.file) > 1 and o.attachment:
             logger.error('--attachment is only valid for one added file')
             addp.exit(1)
 
-        kw = {'on_conflict':o.mode, 'check_duplicate':not o.no_check_duplicate, 
+        kw = {'on_conflict':o.mode, 'check_duplicate':not o.no_check_duplicate,
             'mergefiles':not o.no_merge_files, 'update_key':o.update_key}
 
         for file in o.file:
             try:
                 if os.path.isdir(file):
                     if o.recursive:
-                        my.scan_dir(file, rename=o.rename, copy=o.copy, 
+                        my.scan_dir(file, rename=o.rename, copy=o.copy,
                             search_doi=not o.no_query_doi,
                             search_fulltext=not o.no_query_fulltext,
                               **kw)
                     else:
                         raise ValueError(file+' is a directory, requires --recursive to explore')
 
                 elif file.endswith('.pdf'):
-                    my.add_pdf(file, attachments=o.attachment, rename=o.rename, copy=o.copy, 
+                    my.add_pdf(file, attachments=o.attachment, rename=o.rename, copy=o.copy,
                             search_doi=not o.no_query_doi,
-                            search_fulltext=not o.no_query_fulltext, 
-                            scholar=o.scholar, 
+                            search_fulltext=not o.no_query_fulltext,
+                            scholar=o.scholar,
                             **kw)
 
                 else: # file.endswith('.bib'):
                     my.add_bibtex_file(file, **kw)
 
             except Exception as error:
-                # print(error) 
+                # print(error)
                 # addp.error(str(error))
                 raise
                 logger.error(str(error))
                 if not o.ignore_errors:
-                    if len(o.file) or (os.isdir(file) and o.recursive)> 1: 
+                    if len(o.file) or (os.isdir(file) and o.recursive)> 1:
                         logger.error('use --ignore to add other files anyway')
                     addp.exit(1)
 
         savebib(my, o)
 
 
     # check
     # =====
-    checkp = subparsers.add_parser('check', description='check and fix entries', 
+    checkp = subparsers.add_parser('check', description='check and fix entries',
         parents=[cfg])
     checkp.add_argument('-k', '--keys', nargs='+', help='apply check on this key subset')
     checkp.add_argument('-f','--force', action='store_true', help='do not ask')
 
     grp = checkp.add_argument_group('entry key')
     grp.add_argument('--fix-key', action='store_true', help='fix key based on author name and date (in case misssing or digit)')
     grp.add_argument('--key-ascii', action='store_true', help='replace keys unicode character with ascii')
@@ -1025,66 +1025,66 @@
         #     o.fix_doi = True
         #     o.fetch_all = True
         #     o.fix_key = True
 
         for e in my.entries:
             if o.keys and e.get('ID','') not in o.keys:
                 continue
-            my.fix_entry(e, fix_doi=o.fix_doi, fetch=o.fetch, fetch_all=o.fetch_all, fix_key=o.fix_key, 
-                auto_key=o.auto_key, format_name=o.format_name, encoding=o.encoding, 
+            my.fix_entry(e, fix_doi=o.fix_doi, fetch=o.fetch, fetch_all=o.fetch_all, fix_key=o.fix_key,
+                auto_key=o.auto_key, format_name=o.format_name, encoding=o.encoding,
                 key_ascii=o.key_ascii, interactive=not o.force)
 
 
         if o.duplicates:
             my.check_duplicates(mode=o.mode)
 
         savebib(my, o)
 
 
     # filecheck
     # =====
     filecheckp = subparsers.add_parser('filecheck', description='check attached file(s)',
         parents=[cfg])
-    # filecheckp.add_argument('-f','--force', action='store_true', 
+    # filecheckp.add_argument('-f','--force', action='store_true',
     #     help='do not ask before performing actions')
 
     # action on files
-    filecheckp.add_argument('-r','--rename', action='store_true', 
+    filecheckp.add_argument('-r','--rename', action='store_true',
         help='rename files')
-    filecheckp.add_argument('-c','--copy', action='store_true', 
+    filecheckp.add_argument('-c','--copy', action='store_true',
         help='in combination with --rename, keep a copy of the file in its original location')
 
     # various metadata and duplicate checks
-    filecheckp.add_argument('--metadata-check', action='store_true', 
+    filecheckp.add_argument('--metadata-check', action='store_true',
         help='parse pdf metadata and check against metadata (currently doi only)')
 
-    filecheckp.add_argument('--hash-check', action='store_true', 
+    filecheckp.add_argument('--hash-check', action='store_true',
         help='check file hash sum to remove any duplicates')
 
-    filecheckp.add_argument('-d', '--delete-broken', action='store_true', 
+    filecheckp.add_argument('-d', '--delete-broken', action='store_true',
         help='remove file entry if the file link is broken')
 
-    filecheckp.add_argument('--fix-mendeley', action='store_true', 
+    filecheckp.add_argument('--fix-mendeley', action='store_true',
         help='fix a Mendeley bug where the leading "/" is omitted.')
 
-    filecheckp.add_argument('--force', action='store_true', help='no interactive prompt, strictly follow options') 
+    filecheckp.add_argument('--force', action='store_true', help='no interactive prompt, strictly follow options')
     # filecheckp.add_argument('--search-for-files', action='store_true',
     #     help='search for missing files')
     # filecheckp.add_argument('--searchdir', nargs='+',
     #     help='search missing file link for existing bibtex entries, based on doi')
-    # filecheckp.add_argument('-D', '--delete-free', action='store_true', 
+    # filecheckp.add_argument('-D', '--delete-free', action='store_true',
         # help='delete file which is not associated with any entry')
     # filecheckp.add_argument('-a', '--all', action='store_true', help='--hash and --meta')
 
     def filecheckcmd(o):
         my = Biblio.load(o.bibtex, o.filesdir)
 
         # fix ':home' entry as saved by Mendeley
         for e in my.entries:
-            entry_filecheck(e, delete_broken=o.delete_broken, fix_mendeley=o.fix_mendeley, 
+            entry_filecheck(e, delete_broken=o.delete_broken, fix_mendeley=o.fix_mendeley,
                 check_hash=o.hash_check, check_metadata=o.metadata_check, interactive=not o.force)
 
         if o.rename:
             my.rename_entries_files(o.copy)
 
         savebib(my, o)
 
@@ -1261,20 +1261,20 @@
 
 
     # doi
     # ===
     doip = subparsers.add_parser('doi', description='parse DOI from PDF')
     doip.add_argument('pdf')
     doip.add_argument('--image', action='store_true', help='convert to image and use tesseract instead of pdftotext')
-    
+
     def doicmd(o):
         print(extract_pdf_doi(o.pdf, image=o.image))
 
     # fetch
-    # =====   
+    # =====
     fetchp = subparsers.add_parser('fetch', description='fetch bibtex from DOI')
     fetchp.add_argument('doi')
 
     def fetchcmd(o):
         print(fetch_bibtex_by_doi(o.doi))
 
 
@@ -1303,26 +1303,26 @@
         # my = Biblio(o.bibtex, o.filesdir)
         logger.info(o.bibtex+' <==> '+back)
         shutil.copy(o.bibtex, tmp)
         shutil.move(back, o.bibtex)
         shutil.move(tmp, back)
         savebib(None, o)
 
-        
+
 
     # git
     # ===
     gitp = subparsers.add_parser('git', description='git subcommand')
     gitp.add_argument('gitargs', nargs=argparse.REMAINDER)
 
 
     def gitcmd(o):
         try:
             out = sp.check_output(['git']+o.gitargs, cwd=config.gitdir)
-            print(out)
+            print(out.decode())
         except:
             gitp.error('failed to execute git command')
 
 
     o = parser.parse_args()
 
     # verbosity
@@ -1361,12 +1361,14 @@
     elif o.cmd == 'doi':
         doicmd(o)
     elif o.cmd == 'fetch':
         fetchcmd(o)
     elif o.cmd == 'extract':
         extractcmd(o)
     else:
-        raise ValueError('this is a bug')
+        parser.print_help()
+        parser.exit(1)
+        # raise ValueError('this is a bug')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `papers-cli-v1.0/papers/config.py` & `papers-cli-v1.0.1/papers/config.py`

 * *Files identical despite different names*

### Comparing `papers-cli-v1.0/papers/duplicate.py` & `papers-cli-v1.0.1/papers/duplicate.py`

 * *Files identical despite different names*

### Comparing `papers-cli-v1.0/papers/encoding.py` & `papers-cli-v1.0.1/papers/encoding.py`

 * *Files identical despite different names*

### Comparing `papers-cli-v1.0/papers/extract.py` & `papers-cli-v1.0.1/papers/extract.py`

 * *Files identical despite different names*

### Comparing `papers-cli-v1.0/papers/latexenc.py` & `papers-cli-v1.0.1/papers/latexenc.py`

 * *Files identical despite different names*

### Comparing `papers-cli-v1.0/setup.cfg` & `papers-cli-v1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `papers-cli-v1.0/setup.py` & `papers-cli-v1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `papers-cli-v1.0/versioneer.py` & `papers-cli-v1.0.1/versioneer.py`

 * *Files identical despite different names*

