# Comparing `tmp/bintang-0.1.6-py3-none-any.whl.zip` & `tmp/bintang-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 21384 bytes, number of entries: 14
+Zip file size: 22856 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       25 b- defN 22-Sep-15 02:00 bintang/__init__.py
 -rw-rw-rw-  2.0 fat     6439 b- defN 22-Jul-05 11:25 bintang/besqlite.py
--rw-rw-rw-  2.0 fat     1319 b- defN 22-Dec-22 23:56 bintang/cell.py
+-rw-rw-rw-  2.0 fat     1526 b- defN 23-Apr-14 06:25 bintang/cell.py
 -rw-rw-rw-  2.0 fat      566 b- defN 23-Mar-29 02:17 bintang/column.py
--rw-rw-rw-  2.0 fat    23341 b- defN 23-Apr-11 09:18 bintang/core.py
--rw-rw-rw-  2.0 fat      186 b- defN 23-Feb-13 06:10 bintang/log.py
--rw-rw-rw-  2.0 fat     1385 b- defN 22-Dec-21 22:40 bintang/row.py
--rw-rw-rw-  2.0 fat    47313 b- defN 23-Apr-11 11:28 bintang/table.py
--rw-rw-rw-  2.0 fat     4981 b- defN 23-Feb-20 03:30 bintang/travdict.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-11 12:32 bintang-0.1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      249 b- defN 23-Apr-11 12:32 bintang-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 12:32 bintang-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-11 12:32 bintang-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1043 b- defN 23-Apr-11 12:32 bintang-0.1.6.dist-info/RECORD
-14 files, 88039 bytes uncompressed, 19684 bytes compressed:  77.6%
+-rw-rw-rw-  2.0 fat    24155 b- defN 23-Apr-17 08:28 bintang/core.py
+-rw-rw-rw-  2.0 fat     5027 b- defN 23-Apr-14 06:27 bintang/iterdict.py
+-rw-rw-rw-  2.0 fat      186 b- defN 23-Apr-17 08:59 bintang/log.py
+-rw-rw-rw-  2.0 fat     1385 b- defN 23-Apr-12 12:29 bintang/row.py
+-rw-rw-rw-  2.0 fat    53510 b- defN 23-Apr-17 09:08 bintang/table.py
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-17 09:20 bintang-0.1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      249 b- defN 23-Apr-17 09:20 bintang-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 09:20 bintang-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-17 09:20 bintang-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1043 b- defN 23-Apr-17 09:20 bintang-0.1.7.dist-info/RECORD
+14 files, 95303 bytes uncompressed, 21156 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -9,35 +9,35 @@
 
 Filename: bintang/column.py
 Comment: 
 
 Filename: bintang/core.py
 Comment: 
 
+Filename: bintang/iterdict.py
+Comment: 
+
 Filename: bintang/log.py
 Comment: 
 
 Filename: bintang/row.py
 Comment: 
 
 Filename: bintang/table.py
 Comment: 
 
-Filename: bintang/travdict.py
-Comment: 
-
-Filename: bintang-0.1.6.dist-info/LICENSE
+Filename: bintang-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: bintang-0.1.6.dist-info/METADATA
+Filename: bintang-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: bintang-0.1.6.dist-info/WHEEL
+Filename: bintang-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: bintang-0.1.6.dist-info/top_level.txt
+Filename: bintang-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: bintang-0.1.6.dist-info/RECORD
+Filename: bintang-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bintang/cell.py

```diff
@@ -20,26 +20,33 @@
     # DEPRECATED - use super() instead
     # def __init__(self,columnid, path_list, value):
     #     Cell.__init__(self, columnid, value)
     #     self.path_list = path_list
             
 
     def __repr__(self):
-        return "{}(columnid:{}, value:{}, path_list:{}, get_columnname():{}, is_parent_key:{})".format\
+        return "{}(columnid:{}, value:{}, path_list:{}, get_column():{}, is_parent_key:{})".format\
             (__class__.__name__, str(self.columnid), str(self.value)\
-            ,str(self.path_list), self.get_columnname(), self.is_key)    
+            ,str(self.path_list), self.get_column(), self.is_key)    
         
     def gen_path_list_norowid(self):
         pathl_norowid = [x for x in self.path_list if not isinstance(x, int)]
         return pathl_norowid
      
 
-    def get_columnname(self):
+    def get_column(self):
         pathl_norowid = self.gen_path_list_norowid()
-        return pathl_norowid[-1]
+        colname = pathl_norowid[-1]
+        if pathl_norowid.count(colname) > 1: # resolve name if table and column would use the same name
+            return colname + '_' + colname
+        else:
+            return pathl_norowid[-1]
+    
+
+
```

## bintang/core.py

```diff
@@ -1,15 +1,15 @@
 from openpyxl import load_workbook
 import pyodbc
 import os
 import json
 import copy
 from bintang.table import Table, Table_Path
 from bintang.table import _match_primitive, _match_caseless, _match_caseless_unicode
-from bintang import travdict
+from bintang import iterdict
 from pathlib import Path
 from bintang.log import log
 from thefuzz import process as thefuzzprocess
 # import logging
 
 # log = logging.getLogger(__name__)
 # FORMAT = "[%(filename)s:%(lineno)s - %(funcName)10s() ] %(message)s"
@@ -23,14 +23,15 @@
 #         self.message = "Cannot find table '{}'.".format(tablename)
 #         super().__init__(self.message)
 
 
 class Bintang():
     def __init__(self, name=None, backend=None):
         self.name = name
+        self.parent = 'dad'
         self.__tables = {} # this must be a dict of id:table object
         self.__last_assigned_tableid= -1 #
         self.__be = None
         if backend is not None:
             from bintang.besqlite import Besqlite
             self.__be = Besqlite(self.name)
  
@@ -66,22 +67,23 @@
         import shutil
         if dest == None:
             dest = os.getcwd()
         shutil.copy(self.__be.dbpath, dest)      
 
 
     def create_table(self, name, columns=None):
-        tobj = Table(name) # create a tobj object
+        tobj = Table(name, bing=self) # create a tobj object
         self.add_table(tobj)
         if self.__be is not None:   # if is_persistent is True then update the tobj attributes and pass the connection
             tobj._Table__be = self.__be           
             tobj._Table__be.add_table(self.get_tableid(name), name)
         if columns is not None:
             for column in columns: # add column
                 tobj.add_column(column)
+        return tobj        
 
     def delete_table(self, tablename):
         tableid = self.get_tableid(tablename)
         if tableid is None:
             tablenames = self.get_tables()
             extracted = thefuzzprocess.extract(tablename, tablenames, limit=2)
             fuzzies = [x[0] for x in extracted if x[1]>95]
@@ -167,15 +169,15 @@
         self.__tables[tablename].drop_column(column)
 
 
     def insert(self,tablename,columns,values):
         self.get_table(tablename).insert(columns,values)
         
 
-    def get_cells_bycolumnnames(self,tablename,row,columns):
+    def _get_cells_bycolumns(self,tablename,row,columns):
         _cells = {} # to hold the results cells
         for name in columns:
             columnid = self.__tables[tablename].get_columnid(name)
             # only assign if columnid exists to avoid a KeyError
             if columnid in row.cells:
                 _cells[columnid] = row.cells[columnid]
         return _cells
@@ -208,23 +210,27 @@
             # suggest = process.extract(tablename, tablenames, limit=2)
             # print('hello',suggest)
             # print('yes')
             # quit()
             raise ValueError('Tablename {} does not exist.'.format(tablename))
 
 
-    def iterrows(self, tablename, columns=None, row_type = 'dict', rowid=False):
+    def iterrows(self, table, columns=None, row_type = 'dict', rowid=False):
         """get the table form the collection
         then yield idx and row from table's iterrows()
         """
         
-        self.raise_valueerror_tablename(tablename)
-        for idx, row in self.get_table(tablename).iterrows(columns, row_type=row_type, rowid=rowid):
-            yield idx, row
-            
+        #self.raise_valueerror_tablename(tablename)
+        if isinstance(table, Table):
+            for idx, row in table.iterrows(columns, row_type=row_type, rowid=rowid):
+                yield idx, row
+        else:
+            for idx, row in self.get_table(table).iterrows(columns, row_type=row_type, rowid=rowid):
+                yield idx, row
+                
 
     def dev_read_db(self, connstr, tablename, columns = None):
         self.create_table(tablename)
         self[tablename].connstr = connstr
         import pyodbc
         conn = pyodbc.connect(connstr)
         cursor = conn.cursor()
@@ -288,16 +294,16 @@
         conn.close() 
 
 
     def read_excel(self, path, sheetname, table=None):
         table_ = sheetname
         if table is not None:
             table_ = table
-  
-        self.create_table(table_)        
+        if table_ not in self.get_tables():
+            self.create_table(table_)        
         if self.__be is not None:
             self.__be.create_table(table_)
         wb = load_workbook(path, read_only=True, data_only=True)
         ws = wb[sheetname]
         columns = []
         Nonecolumn_cnt = 0
         for rownum, row_cells in enumerate(ws.iter_rows(),start=1):
@@ -312,22 +318,26 @@
                         columns.append(cell.value)
                 if Nonecolumn_cnt > 0:
                     log.warning('Warning! Noname column detected!')          
             
             if rownum > 1:
                 for cell in row_cells:
                     values.append(cell.value)
-                self.get_table(table_).insert(values, columns)
+                # if rownum == 370:
+                #     log.debug(f'{values} at rownum 370.')
+                #     log.debug(any(values))
+                if any(values):
+                    self.get_table(table_).insert(values, columns)
         if self.__be is not None:
             self.get_table(table_).add_row_into_be()
 
 
     def read_dict(self, dict_obj, tablepaths=[]):
         debug = False
-        for tprow in travdict.traverse_dict(dict_obj, tablepaths):
+        for tprow in iterdict.iterdict(dict_obj, tablepaths):
             # if debug:
             #     print("\n---------------------in bintang---------------------")
             #     print(row)
             
             for k,v in tprow.cells.items():
                 # print(k,'->',v)
                 
@@ -363,15 +373,15 @@
         cursor = conn.cursor()
         if params is not None:
             cursor.execute(sql_str, params)
         else:
             cursor.execute(sql_str)
         columns = [col[0] for col in cursor.description]
         for row in cursor.fetchall():
-            self.insert(tablename, columns, row)
+            self.insert(tablename, row, columns)
              
 
     def VOID_get_row_asdict(self, tablename, idx, columns=None):
         return self.get_table(tablename).get_row_asdict(idx, columns=columns)
 
 
     def _add_lcell(self, lidx, ltable, outrow, out_table, out_lcolumns, rowid):
@@ -385,36 +395,36 @@
                 if k in out_lcolumns:
                     cell = self[out_table].make_cell(k,v)
                     outrow.add_cell(cell)
         return outrow            
 
 
     def _add_rcell(self, ridx, rtable, outrow, out_table, out_rcolumns, rcol_resolved, rowid):
-        for k, v in self[rtable].get_row_asdict(ridx,rowid=rowid).items():
+        for k, v in rtable.get_row_asdict(ridx,rowid=rowid).items():
             if out_rcolumns is None:
                 cell = self[out_table].make_cell(rcol_resolved[k],v)
                 outrow.add_cell(cell)
             if out_rcolumns is not None:
                 # include only the passed columns
                 if k in out_rcolumns:
                     cell = self[out_table].make_cell(rcol_resolved[k],v)
                     outrow.add_cell(cell)
         return outrow
 
 
-    def _resolve_join_columns (self,ltable, rtable, rowid=False):
+    def _resolve_join_columns (self,ltable, rtable_obj, rowid=False):
         # resolve any conflict column by prefixing its tablename
         # notes: conflict column occurs when the same column being used in two joining table.
         rcol_resolved = {}
         if rowid:
             rcol_resolved['rowid_'] = ltable + '_' + 'rowid_'
         lcolumns = self[ltable].get_columns()
-        for col in self[rtable].get_columns():
+        for col in rtable_obj.get_columns():
             if col in lcolumns:
-                rcol_resolved[col] = rtable + '_' + col
+                rcol_resolved[col] = rtable_obj.name + '_' + col
             else:
                 rcol_resolved[col] = col
         return rcol_resolved  
 
 
 
     # def _DEPRECATED_innerjoin(self,ltable, lkeys
@@ -463,59 +473,67 @@
     #                 out_tobj.add_row(outrow)
     #     #debug merged.print() 
     #     return out_tobj
 
 
     def innerjoin(self
                 ,ltable: str #, lkeys
-                ,rtable: str #, rkeys
-                ,on: list # list of lkey & r key tuple
+                ,rtable: str | Table #, rkeys
+                ,on: list[tuple] # list of lkey & r key tuple
                 ,into: str
                 ,out_lcolumns: list=None
                 ,out_rcolumns: list=None
                 ,rowid=False) -> Table:
-
+        
+        rtable_obj = None
+        if isinstance(rtable,Table):
+            rtable_obj = rtable
+            rtable = rtable.name
+        else:
+            rtable_obj = self[rtable]
         # validate input eg. column etc
         lkeys = [x[0] for x in on] # generate lkeys from on (1st sequence)
         rkeys = [x[1] for x in on] # generate rkeys from on (2nd sequence)
         lkeys = self[ltable].validate_columns(lkeys)
-        rkeys = self[rtable].validate_columns(rkeys)
+        #rkeys = self[rtable].validate_columns(rkeys)
+        rkeys = rtable_obj.validate_columns(rkeys)
         if out_lcolumns is not None:
             out_lcolumns = self[ltable].validate_columns(out_lcolumns)
         if out_rcolumns is not None:
-            out_rcolumns = self[rtable].validate_columns(out_rcolumns)
+            # out_rcolumns = self[rtable].validate_columns(out_rcolumns)
+            out_rcolumns = rtable_obj.validate_columns(out_rcolumns)
 
         # resolve columns conflicts
-        rcol_resolved = self._resolve_join_columns(ltable, rtable, rowid)
+        rcol_resolved = self._resolve_join_columns(ltable, rtable_obj, rowid)
         # create an output table
         out_table = into
         self.create_table(out_table)
         out_tobj = self.get_table(out_table)
 
         # for debuging create merged table to store the matching rowids
         #merged = self.create_table("merged",["lrowid","rrowid"])
 
         numof_keys = len(on) #(lkeys)
         # loop left table
         for lidx, lrow in self.iterrows(ltable, columns=lkeys, rowid=rowid):
             # loop right table
-            for ridx, rrow in self.iterrows(rtable, columns=rkeys, rowid=rowid):
+            for ridx, rrow in self.iterrows(rtable_obj, columns=rkeys, rowid=rowid):
                 matches = 0 # store matches for each rrow
                 # compare value for any matching keys, if TRUE then increment matches
                 for i in range(numof_keys): 
                     if _match_caseless_unicode(lrow[lkeys[i]], rrow[rkeys[i]]):
                         matches += 1 # incremented!
                 if matches == numof_keys: # if fully matched, create the row & add into the output table
                     #debug merged.insert(["lrowid","rrowid"], [lrow["_rowid"], rrow["_rowid"]])
                     #and add the row to output table
                     outrow = out_tobj.make_row()
                     # add cells from left table
                     outrow = self._add_lcell(lidx, ltable, outrow, out_table, out_lcolumns, rowid)
                     # add cells from right table
-                    outrow = self._add_rcell(ridx, rtable, outrow, out_table, out_rcolumns, rcol_resolved, rowid)   
+                    outrow = self._add_rcell(ridx, rtable_obj, outrow, out_table, out_rcolumns, rcol_resolved, rowid)   
                     out_tobj.add_row(outrow)
         #debug merged.print() 
         return out_tobj
                 
 
     def leftjoin(self,ltable, rtable, lkeys, rkeys
                 ,out_lcolumns=None
```

## bintang/table.py

```diff
@@ -1,7 +1,8 @@
+#from bintang.core import Bintang
 from bintang.column import Column
 from bintang.cell import Cell
 from bintang.row import Row
 import json
 import sqlite3
 import uuid
 import re
@@ -11,35 +12,38 @@
 # import logging
 
 # log = logging.getLogger(__name__)
 # FORMAT = "[%(filename)s:%(lineno)s - %(funcName)10s() ] %(message)s"
 # logging.basicConfig(format=FORMAT)
 # log.setLevel(logging.DEBUG)
 
+PARENT_PREFIX = ''
 
 class ColumnNotFoundError(Exception):
     def __init__(self,table, column):
         self.message = "Cannot find column '{}' in table {}.".format(column, table)
         super().__init__(self.message)
     
         
 
 class Table(object):
     """Define a Bintang table object
        - provide columns to store a dictionary of column objects
        - provide rows to store a dictionary of row objects
     """
-    def __init__(self,name):
+    def __init__(self,name, bing=None):
+        self.bing = bing
         self.name = name
         self.__columns = {}
         self.__rows = {}
         self.__temprows = []
         self.__last_assigned_columnid= -1 #
         self.__last_assigned_rowid = -1
         self.__be = None
+        
 
 
     def __getitem__(self, idx): # subscriptable version of self.get_row_asdict()
         #return self.__rows[idx] # bad design. a raw row isn't that useful at client code
         return self.get_row_asdict(idx)
 
 
@@ -70,15 +74,15 @@
             return columns
         
 
     def to_sql(self, conn, schema, table, columns, method='prep', max_rows = 1):
         if method == 'prep':
             return self.to_sql_prep(conn, schema, table, columns, max_rows=max_rows)
         elif method =='string':
-            return self.to_sql_string(self, conn, schema, table, columns, max_rows=max_rows)
+            return self.to_sql_string(conn, schema, table, columns, max_rows=max_rows)
 
  
     def to_sql_string(self, conn, schema, table, columns, max_rows = 300):
         colmap = self.set_to_sql_colmap(columns)
         src_cols = [x for x in colmap.values()]
         dest_columns = [x for x in colmap.keys()]
        
@@ -129,28 +133,28 @@
             value = value.replace("'","''")
         return "{}{}{}".format('' if literals[0] is None else literals[0], value, '' if literals[1] is None else literals[1])
     
 
     def get_sql_typeinfo_table(self, conn):
         cursor = conn.cursor()
         sql_type_info_tuple = cursor.getTypeInfo(sqlType = None)
-        columnnames = [column[0] for column in cursor.description]
+        columns_ = [column[0] for column in cursor.description]
         tobj = Table('sql_typeinfo')
         for row in sql_type_info_tuple:
-            tobj.insert(columnnames, row)        
+            tobj.insert(row, columns_)        
         return tobj
     
 
     def set_sql_datatype(self, dest_columns, conn, schema, table):
         cursor = conn.cursor()
         sql_columns = cursor.columns(schema=schema, table=table)
-        columns = [column[0] for column in cursor.description]
+        columns_ = [column[0] for column in cursor.description]
         tobj = Table('sql_columns_')
         for row in sql_columns: #cursor.columns(schema=schema, table=table):
-            tobj.insert(columns, row)
+            tobj.insert(row, columns_)
         sql_columns_withtype = {}
         for col in dest_columns:
             _type = tobj.get_value('type_name', where = lambda row: row['column_name']==col)
             sql_columns_withtype[col] = _type
         return sql_columns_withtype
     
 
@@ -184,14 +188,16 @@
         cursor = conn.cursor()
         temp_rows = []
         total_rowcount = 0
         for idx, row in self.iterrows(src_cols, row_type='list'):
             for v in row:
                 temp_rows.append(v)
             if len(temp_rows) == (mrpb * numof_col):
+                # log.debug(prep_stmt)
+                # log.debug(temp_rows)
                 cursor.execute(prep_stmt, temp_rows)
                 total_rowcount += cursor.rowcount
                 temp_rows.clear()     
         
         if len(temp_rows) > 0: # if any reminder
             param_markers = self.gen_row_param_markers(numof_col, int(len(temp_rows)/numof_col))
             prep_stmt = sql_template.format(schema,table,",".join(['"{}"'.format(x) for x in dest_columns]),param_markers)
@@ -207,24 +213,38 @@
             params.append(param)
         return ",".join(params)
     
 
 
     def gen_create_sqltable(self, dbms):
         # scanning table to get column properties
-        # and assin the data type and size (when able)
+        # and assign the data type and size (when able)
         self.set_data_props()
         for col in self.get_columns():
             cobj = self.__columns[self.get_columnid(col)]
-            for type, prop in cobj.data_props.items():
-                if type == 'str':
-                    cobj.data_type = 'str' #type_map['str'][0]
-                    cobj.column_size = prop['column_size']
-                else:
-                    cobj.data_type = type #type_map[type][0]    
+            if cobj.data_type is None:
+                if len(cobj.data_props) == 0: # a column that has no data at all
+                    cobj.data_type = 'str'  # force to str
+                    cobj.column_size = 50 # force to 50
+                # loop through the data props for column that has it
+                if 'str' in cobj.data_props:
+                    cobj.data_type = 'str'
+                    col_size = cobj.data_props['str']['column_size']
+                    # loop through any other type if the column_size bigger, if it is assign it.
+                    for k, v in cobj.data_props.items():
+                        if v['column_size'] > col_size:
+                            col_size = v['column_size']
+                    cobj.column_size = col_size #cobj.data_props['str']['column_size']
+                elif 'datetime' in cobj.data_props:
+                    cobj.data_type = 'datetime'
+                    cobj.column_size = cobj.dataprops['datetime']['column_size']
+                else: # just get the first one and break. to be observed later on!
+                    for type, prop in cobj.data_props.items():
+                        cobj.data_type = type
+                        break
         
         # use type_map to translate the type
         create_columns = []
         for col in self.get_columns():
             cobj = self.__columns[self.get_columnid(col)]
             if cobj.data_type == 'str':
                 create_item = ['[{}]'.format(cobj.name), type_map[dbms][cobj.data_type],'({})'.format(cobj.column_size)]
@@ -239,14 +259,17 @@
                 create_item_str.append('\t')
             for i in citem:
                 create_item_str.append(i)
             create_item_str.append('\n')
             create_columns_str.append(' '.join(create_item_str))
         create_sqltable_templ = "CREATE TABLE {} (\n{})".format(self.name, '\t,'.join(create_columns_str))
         return create_sqltable_templ 
+    
+
+
         
 
     def add_column(self,name, data_type=None, column_size=None):
         # check if the passed name already exists
         columnid = self.get_columnid(name)
         if columnid is None:
             cobj = Column(name)
@@ -572,49 +595,43 @@
                 return idx
         # if debug:
         #     print("\n  ------------------out get_row_rowid (table.py) -------------------")
         return None    
 
 
     def upsert_table_path_row(self, tprow):
-        debug = False
-        if debug:
-            print("\n  ------------------in upsert_table_path_row (table.py) --------------------")
+        #log.debug("\n  ------------------in upsert_table_path_row (table.py) --------------------")
         # extract the rowid and use it as the table index (the key of rows{})
         # create a row if the rowid not found in the table's index
         res_idx = self.get_rowidx_byrowid(tprow.id)
         
         if res_idx is None:
-            if debug:
-                print("inserting... row does not exist", tprow)
+            #log.debug(f'inserting... row does not exist {tprow}')
             row = self.make_row(tprow.id)
             # re-make cells from tprow
             for id, c in tprow.cells.items():
-                if debug:
-                    print('cell:', id, ";", c)
+                #log.debug(f'{id} cell: {c}')
                 if c.is_key == True:
-                    cell = self.make_cell('/' + c.get_column(), c.value)
+                    cell = self.make_cell(PARENT_PREFIX + c.get_column(), c.value)
                 else:
                     cell = self.make_cell(c.get_column(), c.value)
 
                 row.add_cell(cell)
             # add to rows
             self.add_row(row)
             
         elif res_idx is not None:
-            if debug:
-                print("updating... row exists", tprow)
+            #log.debug(f"updating... row exists {tprow}")
             for id, c in tprow.cells.items():
                 if c.is_key == True:
-                    cell = self.make_cell('/' + c.get_column(), c.value)
+                    cell = self.make_cell(PARENT_PREFIX + c.get_column(), c.value)
                 else:
                     cell = self.make_cell(c.get_column(), c.value)
                 self.__rows[res_idx].add_cell(cell)        
-        if debug:
-            print("\n  ------------------out upsert_table_path_row (table.py)-------------------"    )
+        #log.debug("\n  ------------------out upsert_table_path_row (table.py)-------------------")
 
 
     def make_cell(self,column,value,new_column=True):
         columnid = self.get_columnid(column)
         if columnid is None: # if columnid is None then assume user wants a new column
             if new_column == True:
                 self.add_column(column)
@@ -698,25 +715,29 @@
         if columns is None:
             columns = self.get_columns()
         columnids = self.get_columnids(columns)
         return self._gen_row_aslist(self.__rows[idx],columnids)
 
 
     def _gen_row_aslist(self, row, columnids):
-        #columnids = self.get_columnids(columns)
         return row.get_values(columnids)
 
        
-    def iterrows(self, columns=None, row_type='dict', rowid=False):
+    def iterrows(self, columns=None, row_type='dict', where=None, rowid=False):
         if columns is None:
                 columns = self.get_columns() # assign all available column names
         if row_type == 'dict': 
             if self.__be is None:
-                for idx, row in self.__rows.items():
-                    yield idx, self._gen_row_asdict(row,columns,rowid)
+                if where is not None:
+                    for idx, row in self.__rows.items():
+                        if where(self._gen_row_asdict(row, columns, rowid)):
+                            yield idx, self._gen_row_asdict(row,columns,rowid)
+                else:
+                    for idx, row in self.__rows.items():
+                        yield idx, self._gen_row_asdict(row,columns,rowid)
             if self.__be is not None:
                 for idx, row in self.__be.iterrows_asdict(self.name, columns):
                     yield idx, row
         elif row_type == 'list':
             columnids = self.get_columnids(columns)
             for idx, row in self.__rows.items():
                 yield idx, self._gen_row_aslist(row,columnids)
@@ -974,18 +995,115 @@
                         values = self.get_row_aslist(idx,columns_)
                         tobj.insert(columns_,values)
                 except:
                     pass        
         return tobj
 
 
+    def innerjoin(self
+                #,ltable: str #, lkeys
+                ,rtable: str #, rkeys
+                ,on: list[tuple] # list of lkey & r key tuple
+                ,into: str
+                ,out_lcolumns: list=None
+                ,out_rcolumns: list=None
+                ,rowid=False):
+        
+        rtable_obj = None
+        if isinstance(rtable,Table):
+            rtable_obj = rtable
+            rtable = rtable.name
+        else:
+            rtable_obj = self.bing[rtable]
+        
+        # validate input eg. column etc
+        lkeys = [x[0] for x in on] # generate lkeys from on (1st sequence)
+        rkeys = [x[1] for x in on] # generate rkeys from on (2nd sequence)
+        lkeys = self.validate_columns(lkeys)
+        #rkeys = self[rtable].validate_columns(rkeys)
+        rkeys = rtable_obj.validate_columns(rkeys)
+        if out_lcolumns is not None:
+            out_lcolumns = self.validate_columns(out_lcolumns)
+        if out_rcolumns is not None:
+            # out_rcolumns = self[rtable].validate_columns(out_rcolumns)
+            out_rcolumns = rtable_obj.validate_columns(out_rcolumns)
+
+        # resolve columns conflicts
+        rcol_resolved = self._resolve_join_columns(rtable_obj, rowid)
+        # create an output table
+        out_table = into
+        out_tobj = self.bing.create_table(out_table)
+        out_tobj = self.bing.get_table(out_table)
+        
+        # for debuging create merged table to store the matching rowids
+        #merged = self.create_table("merged",["lrowid","rrowid"])
+
+        numof_keys = len(on) #(lkeys)
+        # loop left table
+        for lidx, lrow in self.iterrows(columns=lkeys, rowid=rowid):
+            # loop right table
+            for ridx, rrow in rtable_obj.iterrows(columns=rkeys, rowid=rowid):
+                matches = 0 # store matches for each rrow
+                # compare value for any matching keys, if TRUE then increment matches
+                for i in range(numof_keys): 
+                    if _match_caseless_unicode(lrow[lkeys[i]], rrow[rkeys[i]]):
+                        matches += 1 # incremented!
+                if matches == numof_keys: # if fully matched, create the row & add into the output table
+                    #debug merged.insert(["lrowid","rrowid"], [lrow["_rowid"], rrow["_rowid"]])
+                    #and add the row to output table
+                    outrow = out_tobj.make_row()
+                    # add cells from left table
+                    log.debug(f'{lidx}')
+                    outrow = self._add_lcell(lidx,  outrow, out_table, out_lcolumns, rowid)
+                    # add cells from right table
+                    outrow = self._add_rcell(ridx, rtable_obj, outrow, out_table, out_rcolumns, rcol_resolved, rowid)   
+                    out_tobj.add_row(outrow)
+        #debug merged.print() 
+        return out_tobj
+
+
+    def _resolve_join_columns (self, rtable_obj, rowid=False):
+        # resolve any conflict column by prefixing its tablename
+        # notes: conflict column occurs when the same column being used in two joining table.
+        rcol_resolved = {}
+        if rowid:
+            rcol_resolved['rowid_'] = rtable_obj.name + '_' + 'rowid_'
+        lcolumns = self.get_columns()
+        for col in rtable_obj.get_columns():
+            if col in lcolumns:
+                rcol_resolved[col] = rtable_obj.name + '_' + col
+            else:
+                rcol_resolved[col] = col
+        return rcol_resolved
     
-
-
-
+    def _add_lcell(self, lidx, outrow, out_table, out_lcolumns, rowid):
+        for k, v in self.get_row_asdict(lidx,rowid=rowid).items():
+            if out_lcolumns is None:
+                # incude all columns
+                cell = self.bing[out_table].make_cell(k,v)
+                outrow.add_cell(cell)
+            if out_lcolumns is not None:
+                # include only the passed columns
+                if k in out_lcolumns:
+                    cell = self.bing[out_table].make_cell(k,v)
+                    outrow.add_cell(cell)
+        return outrow            
+
+
+    def _add_rcell(self, ridx, rtable, outrow, out_table, out_rcolumns, rcol_resolved, rowid):
+        for k, v in rtable.get_row_asdict(ridx,rowid=rowid).items():
+            if out_rcolumns is None:
+                cell = self.bing[out_table].make_cell(rcol_resolved[k],v)
+                outrow.add_cell(cell)
+            if out_rcolumns is not None:
+                # include only the passed columns
+                if k in out_rcolumns:
+                    cell = self.bing[out_table].make_cell(rcol_resolved[k],v)
+                    outrow.add_cell(cell)
+        return outrow
     # def get_type_used(self, column):
     #     # iterate through the table and suss out the type
     #     used_types = []
     #     for idx, row in self.iterrows(columns=[column]):
     #         #if row[column] is not None:
     #         used_type = type(row[column]).__name__
     #         if used_type not in used_types:
@@ -1006,53 +1124,55 @@
     #         used_type = type(row[column]).__name__
     #         if used_type not in used_types:
     #             used_types.append(used_type)
     #     return used_types    
 
 
     #def blookup(self, rtable, keys, lkkeys, out_rcolumns, ret_ascolumns = None):
-    def blookup(self, rtable, on, out_rcolumns):    
+    def blookup(self, rtable, on, out_rcolumns):
+        #rtable = self.bing[rtable] 
+        
         # validate input eg. column etc
         lkeys = [x[0] for x in on] # generate lkeys from on (1st sequence)
         rkeys = [x[1] for x in on] # generate rkeys from on (2nd sequence)
         lkeys = self.validate_columns(lkeys)
-        rkeys = rtable.validate_columns(rkeys)
+        rkeys = self.bing[rtable].validate_columns(rkeys)
         lcolumn_prematch = self.get_columns() # will use this list when matching occurs below
         # validate out_rcolumns once:
         # otherwise will make lots of call later
         valid_out_rcolumns = []
         for item in out_rcolumns:
             if isinstance(item,str):
-                item = rtable.validate_column(item)
+                item = self.bing[rtable].validate_column(item)
                 valid_out_rcolumns.append(item)
             if isinstance(item, tuple):
-                valid_column  = rtable.validate_column(item[0])
+                valid_column  = self.bing[rtable].validate_column(item[0])
                 item_ = tuple([valid_column,item[1]])
                 valid_out_rcolumns.append(item_)
         numof_keys = len(on)
         for lidx, lrow in self.iterrows(lkeys, rowid=True):
-            for ridx, rrow in rtable.iterrows():
+            for ridx, rrow in self.bing[rtable].iterrows():
                 matches = 0
                 for i in range(numof_keys):
                     # if lrow[lkeys[i]] == rrow[rkeys[i]]:
                     if _match_caseless_unicode(lrow[lkeys[i]], rrow[rkeys[i]]):
                         matches += 1 # increment
                 if matches == numof_keys:
                     # update this table lrow for each out_rcolumns
                     for item in valid_out_rcolumns:
                         if isinstance(item, str): # if item is a column
-                            value = rtable[ridx][item]
+                            value = self.bing[rtable][ridx][item]
                             if item in lcolumn_prematch:
                                 print('item',item,'in',self.name)
-                                self.update_row(lidx, rtable.name + '_' + item, value)
+                                self.update_row(lidx, self.bing[rtable].name + '_' + item, value)
                             else:
                                 self.update_row(lidx, item, value)
                         if isinstance(item, tuple): # if a tuple
-                            value = rtable[ridx][item[0]]
-                            self.update_row(lidx, item[1], value)
+                            value = self.bing[rtable][ridx][item[0]]
+                            self.update_row(lidx, item[1], value)                   
 
     def groupbycount(self, column):
         res_dict = {}
         for idx, row in self.iterrows(column):
             value = next(iter(row.values()))
             if value not in res_dict:
                 res_dict[value] = 1
@@ -1156,15 +1276,15 @@
         columns = []
         for k,v in self._Table__columns.items():
             columns.append(dict(id=v.id, name=v.name))
         tbl['columns'] = columns
         return json.dumps(tbl, indent=2)
 
 
-    def get_path_aslist(self):
+    def DEPRECATED_get_path_aslist(self):
         path_as_list = []
         if self.path == '/': # if root
             path_as_list.append('/')
             return path_as_list
         for node in self.path.split("/"):
             if node == '': # if the 1st one. 1st node have discarded by split
                 path_as_list.append('/')
@@ -1206,11 +1326,13 @@
 
 type_map = {
     'sqlserver': {
                 'str':'nvarchar'
                 ,'int':'int'
                 ,'datetime':'datetime'
                 ,'float':'float'
+                ,'bool':'bit'
+                ,'bytes':'varbinary'
                 }
     }
```

## Comparing `bintang/travdict.py` & `bintang/iterdict.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,31 @@
+import copy
 from bintang.cell import Cell_Path_List
 from bintang.row import Row_Table_Path
-import copy
-
-
-def _traverse(dict_or_list, path=[]):
-    if isinstance(dict_or_list, dict):
-        iterator = dict_or_list.items()
-    else:
-        iterator = enumerate(dict_or_list)
-    for k, v in iterator:
-        yield path + [k], v
-        if isinstance(v, (dict, list)):
-            for k, v in _traverse(v, path + [k]):
-                yield k,v
+from bintang.log import log
 
+TABLEPATH_SEP = '_'
 
 def gen_tablepath(path_list):
     pathl_norowid = [x for x in path_list if not isinstance(x, int)]
     if path_list[-1] == pathl_norowid[-1]:
         # this should work for pattern #1 and #2
         del pathl_norowid[-1]
-        tablepath = '/'.join(pathl_norowid)
-        if len(tablepath) > 2:
-            tablepath = tablepath[1:]
+        tablepath = TABLEPATH_SEP.join(pathl_norowid)
+        # if len(tablepath) > 2:
+        #     tablepath = tablepath[1:]
+        #log.debug(tablepath)
         return tablepath
     if (path_list[-2] == pathl_norowid[-1]) and isinstance(path_list[-1], int):
         # this shold work for pattern #3
-        tablepath = '/'.join(pathl_norowid)
-        if len(tablepath) > 2:
-            tablepath = tablepath[1:]
+        #log.debug(pathl_norowid)
+        tablepath = TABLEPATH_SEP.join(pathl_norowid)
+        # if len(tablepath) > 2:
+        #     tablepath = tablepath[1:]
+        #log.debug(tablepath)
         return tablepath
 
 
 def gen_rowid(path_list):
     if isinstance(path_list[-1], str):
         pathl_copy = copy.deepcopy(path_list)
         del pathl_copy[-1]
@@ -42,89 +35,91 @@
     
 
 def gen_table_path_row(path_list, value):
     # there are two types of cell will be created as the result of data path location
     # 1. main cell
     # 2. parent cell (if any)
     # for the path_list 
-    debug = False
     rowid = gen_rowid(path_list)
     row = Row_Table_Path(rowid)
     row.tablepath = gen_tablepath(path_list)
     pathl = copy.deepcopy(path_list) 
     
-    if debug:
-        print('\n---------------------in gen_table_path_row (travdict.py)--------------------------')
-        print('  {}-> path_list {}'.format(len(pathl),path_list))
+    log.debug('\n---------------------in gen_table_path_row (travdict.py)--------------------------')
+    log.debug(f'  {pathl}-> path_list {path_list}')
     
     # # create the first cell    
     # cell = Cell_Path_List(len(pathl), path_list, value)
     # row.add_cell(cell)
     # if debug:
     #     print('  {}-> {}'.format(len(pathl),cell))
     
 
     # take the last item of the path
     if isinstance(pathl[-1], int):
         # if a list
-        if debug: print('  a list...')
+        log.debug('  a list...')
         del pathl[-1]
         del pathl[-1]
-        if debug:
-            print('  {}-> pathl after {}'.format(len(pathl),pathl))
+        log.debug(f'  {len(pathl)}-> pathl after {pathl}')
     elif isinstance(pathl[-1], str):
         # if a dict
-        if debug: print('  a dict...')
+        log.debug('  a dict...')
         del pathl[-1]
     
-    
     # create 'parent key' cells
     while len(pathl) > 1: # if 0 then the root (/) will be included in the result set
-        if debug:
-            print('  {}->>> pathl {}'.format(len(pathl),pathl))
+        log.debug(f'  {len(pathl)}->>> pathl {pathl}')
         #create the cell
         if isinstance(pathl[-1], int):
             # this is a list
             pathl_copy = copy.deepcopy(pathl) # to make it persistent and be used in making cell    
             cell = Cell_Path_List(len(pathl), pathl_copy, pathl[-1])
             cell.is_key = True
             row.add_cell(cell)
-            if debug:
-                print('  {}-> {}'.format(len(pathl),cell))
+            log.debug(f' len pathl {len(pathl)}-> cell {cell}')
             del pathl[-1]
             del pathl[-1]
             
         elif isinstance(pathl[-1], str):
             # this is a dict
             pathl_copy = copy.deepcopy(pathl) # to make it persistent and be used in making cell    
             cell = Cell_Path_List(len(pathl), pathl_copy, pathl[-1])
             cell.is_key = True
             row.add_cell(cell)
-            if debug:
-                print('  {}-> {}'.format(len(pathl),cell))
+            log.debug(f'  len pathl {len(pathl)}-> cell {cell}')
             del pathl[-1]
 
-    # create the first cell    
+    # create the cell
+    pathl_norowid = [x for x in path_list if not isinstance(x, int)]
     cell = Cell_Path_List(len(pathl), path_list, value)
     row.add_cell(cell)
-    if debug:
-        print('  {}-> {}'.format(len(pathl),cell))
-                
-    if debug:
-        print('---------------------out gen_table_path_row (travdict.py)-----------------------') 
+    log.debug(f'  len pathl {pathl}-> cell {cell}')
+    log.debug('---------------------out gen_table_path_row (travdict.py)-----------------------') 
     return row           
     
 
+def _iterdict(dict_or_list, path=['root']):
+    if isinstance(dict_or_list, dict):
+        iterator = dict_or_list.items()
+    else:
+        iterator = enumerate(dict_or_list)
+    for k, v in iterator:
+        yield path + [k], v
+        if isinstance(v, (dict, list)):
+            for k, v in _iterdict(v, path + [k]):
+                yield k,v
+
 
-def traverse_dict(dict_obj, tablepaths=[]):
+def iterdict(dict_obj, tablepaths=None):
     # yield a tprow (row with a table path)
-    # also allow to yield only the row that matches tablepath list from client.
-    for path_list, value, in _traverse(dict_obj, path=['/']):        
+    # also allow to yield only the row that matches tablepath list arg.
+    for i, (path_list, value) in enumerate(_iterdict(dict_obj),0): # path=['/']):
+        #log.debug(f'{i} k-> {path_list} v--> {value}')
         if isinstance(value,(list,dict)):
-            #print('-->',path_list,":",value)
             continue # use continue and comment the below line value = None to create column with list/dict
             #value = '[]'  # include column with list/dict in the table but set value as None
         # print(path_list, value)
         if len(tablepaths) == 0:
             # client wants to return all available tablepaths
             yield gen_table_path_row(path_list,value)
         elif len(tablepaths) > 0:
```

## Comparing `bintang-0.1.6.dist-info/LICENSE` & `bintang-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bintang-0.1.6.dist-info/RECORD` & `bintang-0.1.7.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 bintang/__init__.py,sha256=UIuTaljC0GQNjj4BVS-PnG1uX2B54DR-LKlh14xIHR8,25
 bintang/besqlite.py,sha256=4vfwMAheTgqudMuCH3wlwwWyGJY5aVDd_tmTCiStcJg,6439
-bintang/cell.py,sha256=Zq7hS_ahK2iqIAVfdI2h-ZyHF7bfWpW-HCVcRTqIQaI,1319
+bintang/cell.py,sha256=JW-k_CgYu4nHX3Qk1nTcBP6fkjlsSXMgOuGRz5Dwcs4,1526
 bintang/column.py,sha256=zTMxofr4FXGR95Zcru9G2DlR35e8I3IVifEzOissONM,566
-bintang/core.py,sha256=1WUG_b9dE-hpgEHkwkxtc1PqpCV3i7WuVyiutIs7JoU,23341
+bintang/core.py,sha256=6rupSkjfpEGcJny5SvdFPg-R5JRgF4L7FxnoKp49FU4,24155
+bintang/iterdict.py,sha256=lTxhrivwbCWhSQNN_TrPWaCg2QyeKa9vqf0X5j3vv2M,5027
 bintang/log.py,sha256=N6LImpolwYOJn4zW-nEpX6o63gInJKSzsw2NKM9V1sE,186
 bintang/row.py,sha256=I63-FY9p-lxmaeOOutKQbF9-jOPC3fTW-6frTqmzBOc,1385
-bintang/table.py,sha256=n_p6VKfEIfAXJkYKNw882ys4JstCj0aSQCb27HVktBQ,47313
-bintang/travdict.py,sha256=uWy-FHD6OJVbtcODBuyWBxyPz3nLFvGmTA9uCQ4PBVU,4981
-bintang-0.1.6.dist-info/LICENSE,sha256=nDP3WePgnPckoI4QkIfBpSx_ZNsectSpMKuVHjBb_68,1092
-bintang-0.1.6.dist-info/METADATA,sha256=qpo7RleIbqsiIg0xikdaa8Fvz_CaFbHldfS3lUyzHL4,249
-bintang-0.1.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bintang-0.1.6.dist-info/top_level.txt,sha256=I6MnAK-RhSd0NBsMpB51A4oOOs3-EjdS3IldTjtaR3I,8
-bintang-0.1.6.dist-info/RECORD,,
+bintang/table.py,sha256=ijaGmD1S7JOisq_Rqg-NNG_0dDcBJYuXHG7ITenF9gs,53510
+bintang-0.1.7.dist-info/LICENSE,sha256=nDP3WePgnPckoI4QkIfBpSx_ZNsectSpMKuVHjBb_68,1092
+bintang-0.1.7.dist-info/METADATA,sha256=g4GFwu1N-2AJh_6eTCCOSfEeKwLGZvPHs7Rn7niXP5M,249
+bintang-0.1.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bintang-0.1.7.dist-info/top_level.txt,sha256=I6MnAK-RhSd0NBsMpB51A4oOOs3-EjdS3IldTjtaR3I,8
+bintang-0.1.7.dist-info/RECORD,,
```

