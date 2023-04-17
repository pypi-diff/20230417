# Comparing `tmp/odbc2orm-1.0.6.tar.gz` & `tmp/odbc2orm-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2orm-1.0.6.tar", last modified: Mon Apr 17 04:11:12 2023, max compression
+gzip compressed data, was "odbc2orm-1.0.7.tar", last modified: Mon Apr 17 04:16:52 2023, max compression
```

## Comparing `odbc2orm-1.0.6.tar` & `odbc2orm-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 04:11:12.653104 odbc2orm-1.0.6/
--rw-rw-rw-   0        0        0     9221 2023-04-17 04:11:12.653104 odbc2orm-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     8457 2023-04-16 14:47:11.000000 odbc2orm-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 04:11:12.606222 odbc2orm-1.0.6/odbc2orm/
--rw-rw-rw-   0        0        0        0 2023-04-14 04:28:25.000000 odbc2orm-1.0.6/odbc2orm/__init__.py
--rw-rw-rw-   0        0        0     5271 2023-04-16 13:06:20.000000 odbc2orm-1.0.6/odbc2orm/__main__.py
--rw-rw-rw-   0        0        0      331 2023-04-16 13:02:50.000000 odbc2orm-1.0.6/odbc2orm/config.py
--rw-rw-rw-   0        0        0     3316 2023-04-16 12:34:31.000000 odbc2orm-1.0.6/odbc2orm/convert.py
--rw-rw-rw-   0        0        0     3958 2023-04-14 07:48:05.000000 odbc2orm-1.0.6/odbc2orm/database.py
--rw-rw-rw-   0        0        0     4789 2023-04-17 04:06:58.000000 odbc2orm-1.0.6/odbc2orm/template.py
--rw-rw-rw-   0        0        0     1030 2023-04-17 04:08:53.000000 odbc2orm-1.0.6/odbc2orm/version.py
-drwxrwxrwx   0        0        0        0 2023-04-17 04:11:12.653104 odbc2orm-1.0.6/odbc2orm.egg-info/
--rw-rw-rw-   0        0        0     9221 2023-04-17 04:11:12.000000 odbc2orm-1.0.6/odbc2orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-04-17 04:11:12.000000 odbc2orm-1.0.6/odbc2orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 04:11:12.000000 odbc2orm-1.0.6/odbc2orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-17 04:11:12.000000 odbc2orm-1.0.6/odbc2orm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-17 04:11:12.000000 odbc2orm-1.0.6/odbc2orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 04:11:12.000000 odbc2orm-1.0.6/odbc2orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      369 2023-04-17 04:11:12.668719 odbc2orm-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2042 2023-04-17 04:10:39.000000 odbc2orm-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 04:16:52.622955 odbc2orm-1.0.7/
+-rw-rw-rw-   0        0        0     9221 2023-04-17 04:16:52.622955 odbc2orm-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8457 2023-04-16 14:47:11.000000 odbc2orm-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 04:16:52.591712 odbc2orm-1.0.7/odbc2orm/
+-rw-rw-rw-   0        0        0        0 2023-04-14 04:28:25.000000 odbc2orm-1.0.7/odbc2orm/__init__.py
+-rw-rw-rw-   0        0        0     5359 2023-04-17 04:14:16.000000 odbc2orm-1.0.7/odbc2orm/__main__.py
+-rw-rw-rw-   0        0        0      331 2023-04-16 13:02:50.000000 odbc2orm-1.0.7/odbc2orm/config.py
+-rw-rw-rw-   0        0        0     3316 2023-04-16 12:34:31.000000 odbc2orm-1.0.7/odbc2orm/convert.py
+-rw-rw-rw-   0        0        0     3958 2023-04-14 07:48:05.000000 odbc2orm-1.0.7/odbc2orm/database.py
+-rw-rw-rw-   0        0        0     4789 2023-04-17 04:15:38.000000 odbc2orm-1.0.7/odbc2orm/template.py
+-rw-rw-rw-   0        0        0     1030 2023-04-17 04:16:27.000000 odbc2orm-1.0.7/odbc2orm/version.py
+drwxrwxrwx   0        0        0        0 2023-04-17 04:16:52.622955 odbc2orm-1.0.7/odbc2orm.egg-info/
+-rw-rw-rw-   0        0        0     9221 2023-04-17 04:16:52.000000 odbc2orm-1.0.7/odbc2orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-04-17 04:16:52.000000 odbc2orm-1.0.7/odbc2orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 04:16:52.000000 odbc2orm-1.0.7/odbc2orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-17 04:16:52.000000 odbc2orm-1.0.7/odbc2orm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-17 04:16:52.000000 odbc2orm-1.0.7/odbc2orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 04:16:52.000000 odbc2orm-1.0.7/odbc2orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2023-04-17 04:16:52.638580 odbc2orm-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2042 2023-04-17 04:10:39.000000 odbc2orm-1.0.7/setup.py
```

### Comparing `odbc2orm-1.0.6/PKG-INFO` & `odbc2orm-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbc2orm
-Version: 1.0.6
+Version: 1.0.7
 Summary: Convert ODBC schema to ORM
 Home-page: https://github.com/pe2mbs/odbc2orm
 Author: Marc Bertens-Nguyen
 Author-email: m.bertens@pe2mbs.nl
 Project-URL: Source Public, https://github.com/pe2mbs/odbc2orm/
 Project-URL: Bug Reports, https://github.com/pe2mbs/odbc2orm/issues
 Project-URL: Say Thanks!, https://github.com/pe2mbs/odbc2orm/saythanks
```

### Comparing `odbc2orm-1.0.6/README.md` & `odbc2orm-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.6/odbc2orm/__main__.py` & `odbc2orm-1.0.7/odbc2orm/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 -v                      Verbose output.
 -h/--help               This help information. 
 -o/--output <filename>  write Python code file, instead of stdout.
                         default STDOUT   
 -c/--config <filename>  Configure driver, output and template files.
 -d/--driver <driver>    The ODBC driver to be used,
                         default "Microsoft Access Driver (*.mdb, *.accdb)"
+-D/--dump               Include dump function in output file.                         
 -t/--template <folder>  Create template files and configuration YAML file
                         for personal customizing.                         
 """)
 
 
 def main():
     ALLOWED_TEMPLATES = ( 'leadin', 'table_leadin', 'table_column', 'table_leadout', 'leadout' )
```

### Comparing `odbc2orm-1.0.6/odbc2orm/convert.py` & `odbc2orm-1.0.7/odbc2orm/convert.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.6/odbc2orm/database.py` & `odbc2orm-1.0.7/odbc2orm/database.py`

 * *Files identical despite different names*

### Comparing `odbc2orm-1.0.6/odbc2orm/template.py` & `odbc2orm-1.0.7/odbc2orm/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 leadout = """
 __engine = None
 __session = None
 
 
 def getEngine( database: Optional[str] = None ):
     driver = '${ config.get('driver','' ) }'
-    if not datanase:
+    if not database:
         # This the file with this file was created. 
         database = '${database}'
           
     connection_string = f"DRIVER={{{driver}}};DBQ={database};;ExtendedAnsiSQL=1;"
     connection_url = engine.URL.create( "access+pyodbc",
                                         query = { "odbc_connect": connection_string } )
     global __engine
```

### Comparing `odbc2orm-1.0.6/odbc2orm/version.py` & `odbc2orm-1.0.7/odbc2orm/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
-version         = '1.0.6'
-date            = '13-02-2023'
+version         = '1.0.7'
+date            = '17-02-2023'
 copyright       = '2023'
 author          = 'Marc Bertens-Nguyen'
 author_email    = 'https://github.com/pe2mbs/odbc2orm'
```

### Comparing `odbc2orm-1.0.6/odbc2orm.egg-info/PKG-INFO` & `odbc2orm-1.0.7/odbc2orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbc2orm
-Version: 1.0.6
+Version: 1.0.7
 Summary: Convert ODBC schema to ORM
 Home-page: https://github.com/pe2mbs/odbc2orm
 Author: Marc Bertens-Nguyen
 Author-email: m.bertens@pe2mbs.nl
 Project-URL: Source Public, https://github.com/pe2mbs/odbc2orm/
 Project-URL: Bug Reports, https://github.com/pe2mbs/odbc2orm/issues
 Project-URL: Say Thanks!, https://github.com/pe2mbs/odbc2orm/saythanks
```

### Comparing `odbc2orm-1.0.6/setup.py` & `odbc2orm-1.0.7/setup.py`

 * *Files identical despite different names*

