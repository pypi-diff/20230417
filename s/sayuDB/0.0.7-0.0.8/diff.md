# Comparing `tmp/sayuDB-0.0.7.tar.gz` & `tmp/sayuDB-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayuDB-0.0.7.tar", last modified: Sat Apr  8 21:56:34 2023, max compression
+gzip compressed data, was "sayuDB-0.0.8.tar", last modified: Mon Apr 17 20:49:10 2023, max compression
```

## Comparing `sayuDB-0.0.7.tar` & `sayuDB-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 21:56:34.620056 sayuDB-0.0.7/
--rw-rw-rw-   0        0        0     1064 2023-04-08 21:51:28.000000 sayuDB-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     6072 2023-04-08 21:56:34.619053 sayuDB-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5767 2023-04-08 21:51:28.000000 sayuDB-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 21:56:34.604652 sayuDB-0.0.7/sayuDB/
--rw-rw-rw-   0        0        0      635 2023-04-08 21:51:28.000000 sayuDB-0.0.7/sayuDB/__init__.py
--rw-rw-rw-   0        0        0     4799 2023-04-08 21:54:44.000000 sayuDB-0.0.7/sayuDB/__main__.py
--rw-rw-rw-   0        0        0    14630 2023-04-08 21:52:04.000000 sayuDB-0.0.7/sayuDB/processor.py
--rw-rw-rw-   0        0        0     2042 2023-04-08 21:52:33.000000 sayuDB-0.0.7/sayuDB/remote.py
--rw-rw-rw-   0        0        0     3252 2023-04-08 21:52:17.000000 sayuDB-0.0.7/sayuDB/server.py
-drwxrwxrwx   0        0        0        0 2023-04-08 21:56:34.619053 sayuDB-0.0.7/sayuDB.egg-info/
--rw-rw-rw-   0        0        0     6072 2023-04-08 21:56:34.000000 sayuDB-0.0.7/sayuDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-04-08 21:56:34.000000 sayuDB-0.0.7/sayuDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 21:56:34.000000 sayuDB-0.0.7/sayuDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-08 21:56:34.000000 sayuDB-0.0.7/sayuDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-08 21:56:34.000000 sayuDB-0.0.7/sayuDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 21:56:34.620056 sayuDB-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     6275 2023-04-08 21:53:46.000000 sayuDB-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:49:10.823084 sayuDB-0.0.8/
+-rw-rw-rw-   0        0        0     1064 2023-04-08 21:51:28.000000 sayuDB-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     6072 2023-04-17 20:49:10.821672 sayuDB-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5767 2023-04-08 21:51:28.000000 sayuDB-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 20:49:10.815647 sayuDB-0.0.8/sayuDB/
+-rw-rw-rw-   0        0        0      635 2023-04-08 21:51:28.000000 sayuDB-0.0.8/sayuDB/__init__.py
+-rw-rw-rw-   0        0        0     4799 2023-04-17 20:47:46.000000 sayuDB-0.0.8/sayuDB/__main__.py
+-rw-rw-rw-   0        0        0    20386 2023-04-17 20:45:24.000000 sayuDB-0.0.8/sayuDB/processor.py
+-rw-rw-rw-   0        0        0     2042 2023-04-08 21:52:33.000000 sayuDB-0.0.8/sayuDB/remote.py
+-rw-rw-rw-   0        0        0     3252 2023-04-08 21:52:17.000000 sayuDB-0.0.8/sayuDB/server.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:49:10.821672 sayuDB-0.0.8/sayuDB.egg-info/
+-rw-rw-rw-   0        0        0     6072 2023-04-17 20:49:10.000000 sayuDB-0.0.8/sayuDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-04-17 20:49:10.000000 sayuDB-0.0.8/sayuDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 20:49:10.000000 sayuDB-0.0.8/sayuDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-17 20:49:10.000000 sayuDB-0.0.8/sayuDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 20:49:10.000000 sayuDB-0.0.8/sayuDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 20:49:10.823084 sayuDB-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     6275 2023-04-17 20:47:37.000000 sayuDB-0.0.8/setup.py
```

### Comparing `sayuDB-0.0.7/LICENSE` & `sayuDB-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.7/PKG-INFO` & `sayuDB-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sayuDB
-Version: 0.0.7
+Version: 0.0.8
 Summary: Database management system based on python and JSON.
 Home-page: https://github.com/Arsybai/sayuDB
 Author: Arsybai
 Author-email: me@arsybai.com
 License: MIT
 Keywords: database
 Description-Content-Type: text/markdown
```

### Comparing `sayuDB-0.0.7/README.md` & `sayuDB-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.7/sayuDB/__init__.py` & `sayuDB-0.0.8/sayuDB/__init__.py`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.7/sayuDB/__main__.py` & `sayuDB-0.0.8/sayuDB/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except:
     print("Read the doc here : https://github.com/Arsybai/blob/main/README.md")
     print("""Invalid commad. get help by
 --h""")
     exit()
 
 if sys.argv[1] == "help" or sys.argv[1] == '--h':
-    print("sayuDB v0.0.7\nRead the doc here : https://github.com/Arsybai/blob/main/README.md")
+    print("sayuDB v0.0.8\nRead the doc here : https://github.com/Arsybai/blob/main/README.md")
     print("""
 [ USERS ]
 Show Users  \t\t: show users
 Create user \t\t: create user <username> <password>
 Remove user \t\t: remove user <username>
 
 [ DATABASE ]
```

### Comparing `sayuDB-0.0.7/sayuDB/processor.py` & `sayuDB-0.0.8/sayuDB/processor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 import json, os, shutil, sys
 from tabulate import tabulate
 from operator import itemgetter
 import sayuDB.remote as remote
+import datetime, random, time
+
+functions = [
+    "today()",
+    "index()",
+    "genID()",
+    "increase()"
+]
+
+def genID():
+    return random.randint(10000, 99999)
+
+def today():
+    now = datetime.datetime.now()
+    dt_string = now.strftime('%Y-%m-%d %H:%M:%S')
+    return dt_string
 
 def create_database(name: str):
     config_ = {
         "name":name
     }
     if not os.path.isfile(f'{os.path.dirname(__file__)}/datas/{name}.ezdb'):
         with open(f'{os.path.dirname(__file__)}/datas/{name}.ezdb', 'w') as cdb:
@@ -141,46 +157,81 @@
                 headeer_.append(i)
             for i in db_[name]['datas']:
                 row_ = []
                 for u in i:
                     row_.append(i[u])
                 rows_.append(row_)
             print(tabulate(rows_, headers=headeer_))
-            
-    def insert_row(self, table: str, col, contents: list):
-        """_summary_
+
+    def insert_row(self, table:str, col, contents: list):
+        """
+        _summary_
 
         Args:
             table (str): the table name
             col (list): column name. EX ['col1', 'col2']
             contents (list): the content for each column EX ['content 1', 'content 2']
             
             _Note : You can also use str for col with comma for the separated EX 'col1,col2'_
+
+        Contents Function:
+            today()\t\t: Generate today datetime (only work in str typedata)
+            index()\t\t: Indexing the number of row. it can be use as id too (only work in int typedata)
+            genID()\t\t: Generate random 5 digits ID
+            increase()\t: Increase from the last row value (Only work in int typedata)
         """
+
+
         db_ = self.openDB()
+        def index():
+            return len(db_[table]["datas"]) + 1
         if type(col) == str:
             col = col.split(',')
+        column_ = db_[table]["column"]
+        for i in col:
+            if i not in column_:
+                raise Exception(f"Unknown column {i}")
         idx = 0
         data_ = {}
+        for i in column_:
+            if column_[i] == "str":
+                data_[i] = "null"
+            elif column_[i] == "int":
+                data_[i] = 0
+            elif column_[i] == "float":
+                data_[i] = 0.0
+            elif column_[i] == "dict":
+                data_[i] = {}
         for i in col:
             if i not in db_[table]['column']:
                 print(f"Column {i} not found")
                 sys.exit()
             elif len(col) != len(contents):
                 print("The length of column and contents doesn't match")
                 sys.exit()
             elif db_[table]['column'][i] == 'str':
                 try:
-                    data_[i] = str(contents[idx])
+                    if contents[idx] in functions:
+                        data_[i] = eval(contents[idx])
+                    else:
+                        data_[i] = str(contents[idx])
                 except:
                     print(f"The content typedata invalid at column {i} content {contents[idx]}")
                     sys.exit()
             elif db_[table]['column'][i] == 'int':
+                def increase():
+                    try:
+                        return int(db_[table]['datas'][-1][i]) + 1
+                    except:
+                        return 0
                 try:
-                    data_[i] = int(contents[idx])
+                    if contents[idx] in functions:
+                        data_[i] = eval(contents[idx])
+                    else:
+                        data_[i] = int(contents[idx])
                 except:
                     print(f"The content typedata invalid at column {i} content {contents[idx]}")
                     sys.exit()
             elif db_[table]['column'][i] == 'float':
                 try:
                     data_[i] = float(contents[idx])
                 except:
@@ -220,50 +271,137 @@
             table (str): The table name
             col (_type_): The column what you want to show. use * for all column
             where (_type_, optional): where the column contain some value. Defaults to None.
             order_by (_type_, optional): short data by column asc or desc. Defaults to None.
             as_json (bool, optional): return as json or table. Defaults to False.
         """
         db_ = self.openDB()
-        if limit != None:
-            datas_ = db_[table]['datas'][:limit]
-        else:
-            datas_ = db_[table]['datas'][:limit]
+        datas_ = db_[table]['datas']
         if col == '*':
             datas_ = datas_
         else:
             col = col.split(',')
             idx = 0
             for i in datas_:
                 for u in list(i):
                     if u not in col:
                         del i[u]
                 idx += 1
-        if where != None and ' contain ' in where:
+        def findWhere(wheree, type_=None):
             temp_ = []
-            for i in datas_:
-                if self.eval_typedata('str', where.split(" contain ")[1]) in str(i[where.split(" contain ")[0]]):
-                    temp_.append(i)
-            datas_ = temp_
-        if where != None and ' contain ' not in where:
-            temp_ = []
-            for i in datas_:
-                if i[where.split("=")[0]] == self.eval_typedata(db_[table]['column'][where.split("=")[0]], where.split("=")[1]):
-                    temp_.append(i)
-            datas_ = temp_
+            if type_ == "AND":
+                for i in datas_:
+                    def isMatch(ii):
+                        if i[wheree[ii].split("=")[0]] == self.eval_typedata(db_[table]['column'][wheree[ii].split("=")[0]], wheree[ii].split("=")[1]):
+                            return True
+                        return False
+                    def isNot(ii):
+                        if i[wheree[ii].split("!=")[0]] != self.eval_typedata(db_[table]['column'][wheree[ii].split("!=")[0]], wheree[ii].split("!=")[1]):
+                            return True
+                        return False
+                    def isContain(ii):
+                        if self.eval_typedata('str', wheree[ii].split(" contain ")[1]) in str(i[wheree[ii].split(" contain ")[0]]):
+                            return True
+                        return False
+                    
+                    the_e = []
+                    if " contain " in wheree[0]:
+                        the_e.append("isContain(0)")
+                    elif "!=" in wheree[0]:
+                        the_e.append("isNot(0)")
+                    else:
+                        the_e.append("isMatch(0)")
+                    if " contain " in wheree[1]:
+                        the_e.append("isContain(1)")
+                    elif "!=" in wheree[1]:
+                        the_e.append("isNot(1)")
+                    else:
+                        the_e.append("isMatch(1)")
+                    
+                    if eval(the_e[0]) and eval(the_e[1]):
+                        temp_.append(i)
+
+            elif type_ == "OR":
+                for i in datas_:
+                    def isMatch(ii):
+                        if i[wheree[ii].split("=")[0]] == self.eval_typedata(db_[table]['column'][wheree[ii].split("=")[0]], wheree[ii].split("=")[1]):
+                            return True
+                        return False
+                    def isNot(ii):
+                        if i[wheree[ii].split("!=")[0]] != self.eval_typedata(db_[table]['column'][wheree[ii].split("!=")[0]], wheree[ii].split("!=")[1]):
+                            return True
+                        return False
+                    def isContain(ii):
+                        if self.eval_typedata('str', wheree[ii].split(" contain ")[1]) in str(i[wheree[ii].split(" contain ")[0]]):
+                            return True
+                        return False
+                    
+                    the_e = []
+                    if " contain " in wheree[0]:
+                        the_e.append("isContain(0)")
+                    elif "!=" in wheree[0]:
+                        the_e.append("isNot(0)")
+                    else:
+                        the_e.append("isMatch(0)")
+                    if " contain " in wheree[1]:
+                        the_e.append("isContain(1)")
+                    elif "!=" in wheree[1]:
+                        the_e.append("isNot(1)")
+                    else:
+                        the_e.append("isMatch(1)")
+                    
+                    if eval(the_e[0]) or eval(the_e[1]):
+                        temp_.append(i)
+
+            else:
+                for i in datas_:
+                    def isMatch(ii):
+                        if i[wheree[ii].split("=")[0]] == self.eval_typedata(db_[table]['column'][wheree[ii].split("=")[0]], wheree[ii].split("=")[1]):
+                            return True
+                        return False
+                    def isNot(ii):
+                        if i[wheree[ii].split("!=")[0]] != self.eval_typedata(db_[table]['column'][wheree[ii].split("!=")[0]], wheree[ii].split("!=")[1]):
+                            return True
+                        return False
+                    def isContain(ii):
+                        if self.eval_typedata('str', wheree[ii].split(" contain ")[1]) in str(i[wheree[ii].split(" contain ")[0]]):
+                            return True
+                        return False
+                    
+                    the_e = []
+                    if " contain " in wheree[0]:
+                        the_e.append("isContain(0)")
+                    elif "!=" in wheree[0]:
+                        the_e.append("isNot(0)")
+                    else:
+                        the_e.append("isMatch(0)")
+                    
+                    if eval(the_e[0]):
+                        temp_.append(i)
+            return temp_
         
+        if where != None:
+            if " && " in where:
+                datas_ = findWhere(where.split(" && "), "AND")
+            elif " || " in where:
+                datas_ = findWhere(where.split(" || "), "OR")
+            else:
+                datas_ = findWhere([where])
+
         if order_by != None:
             key_ = order_by.split("|")[0]
             sort_ = order_by.split("|")[1]
             if sort_ == 'asc':
                 datas_ = sorted(datas_, key=itemgetter(key_))
             elif sort_ == 'desc':
                 datas_ = sorted(datas_, key=itemgetter(key_), reverse=True)
                     
         #the anu anu
+        if limit != None:
+            datas_ = datas_[:limit]
         if as_json:
             try:
                 return json.loads(datas_)
             except:
                 return datas_
         headeer_ = []
         rows_ = []
@@ -322,33 +460,30 @@
         """
         for i in set_:
             self.update_row(table, f"{i}={set_[i]}", where)
         return "Column updated"
     
     def delete_row(self, table: str, where: str):
         db_ = self.openDB()
+        temp_ = []
         if table not in db_:
             sys.exit("Table not found")
         if '=' in where:
             col_ = where.split('=')[0]
             val_ = where.split('=')[1]
-            idx = 0
             for i in db_[table]['datas']:
-                if str(i[col_]) == str(val_):
-                    db_[table]['datas'].remove(db_[table]['datas'][idx])
-                idx += 1
+                if str(i[col_]) != str(val_):
+                    temp_.append(i)
         elif ' contain ' in where:
             col_ = where.split(' contain ')[0]
             val_ = where.split(' contain ')[1]
-            idx = 0
             for i in db_[table]['datas']:
-                if str(val_) in str(i[col_]):
-                    db_[table]['datas'].remove(db_[table]['datas'][idx])
-                idx += 1
-            
+                if str(val_) not in str(i[col_]):
+                    temp_.append(i)
+        db_[table]["datas"] = temp_
         self.save_table(table, db_)
 
     def alter_table_rename_column(self,table:str, col:str, to_:str):
         db = self.openDB()
         db[table]["column"][to_] = db[table]["column"][col]
         del db[table]["column"][col]
         for i in reversed(db[table]["datas"]):
```

### Comparing `sayuDB-0.0.7/sayuDB/remote.py` & `sayuDB-0.0.8/sayuDB/remote.py`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.7/sayuDB/server.py` & `sayuDB-0.0.8/sayuDB/server.py`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.7/sayuDB.egg-info/PKG-INFO` & `sayuDB-0.0.8/sayuDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sayuDB
-Version: 0.0.7
+Version: 0.0.8
 Summary: Database management system based on python and JSON.
 Home-page: https://github.com/Arsybai/sayuDB
 Author: Arsybai
 Author-email: me@arsybai.com
 License: MIT
 Keywords: database
 Description-Content-Type: text/markdown
```

### Comparing `sayuDB-0.0.7/setup.py` & `sayuDB-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="sayuDB",
-    version="0.0.7",
+    version="0.0.8",
     author="Arsybai",
     description="Database management system based on python and JSON.",
     packages=["sayuDB"],
     license="MIT",
     author_email="me@arsybai.com",
     url="https://github.com/Arsybai/sayuDB",
     keywords=[
```

