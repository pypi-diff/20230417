# Comparing `tmp/pymediawikidocker-0.9.8.tar.gz` & `tmp/pymediawikidocker-0.9.9.tar.gz`

## Comparing `pymediawikidocker-0.9.8.tar` & `pymediawikidocker-0.9.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/.pydevproject
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/.DS_Store
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/__init__.py
--rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/config.py
--rw-r--r--   0        0        0    23216 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/docker.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/html_table.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/logger.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/mariadb.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/mw.py
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/mwcluster.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/version.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/webscrape.py
--rw-r--r--   0        0        0    11798 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/extensions.json
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/addCronTabEntry.sh
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/addSysopUser.sh
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/initdb.sh
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/installExtensions.sh
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/lang.sh
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwCompose.yml
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwDockerfile
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings.php
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings127.php
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings131.php
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings135.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings136.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings137.php
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings138.php
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings139.php
--rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki127.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki131.sql
--rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki135.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki136.sql
--rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki137.sql
--rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki138.sql
--rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki139.sql
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/phpinfo.php
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/plantuml.sh
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/startRunJobs.sh
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/update.sh
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/mwdocker/resources/templates/upload.ini
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/scripts/install
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/basetest.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/test_config.py
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/test_extensions.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/test_html_tables.py
--rw-r--r--   0        0        0    11260 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/tests/test_install.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/LICENSE
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/README.md
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/.pydevproject
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/.DS_Store
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/__init__.py
+-rw-r--r--   0        0        0    11080 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/config.py
+-rw-r--r--   0        0        0    24283 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/docker.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/html_table.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/logger.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/mariadb.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/mw.py
+-rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/mwcluster.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/version.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/webscrape.py
+-rw-r--r--   0        0        0    11798 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/extensions.json
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/addCronTabEntry.sh
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/addSysopUser.sh
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/initdb.sh
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/installExtensions.sh
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/lang.sh
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwCompose.yml
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwDockerfile
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings.php
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings127.php
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings131.php
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings135.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings136.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings137.php
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings138.php
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings139.php
+-rw-r--r--   0        0        0    56849 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki127.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki131.sql
+-rw-r--r--   0        0        0    64022 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki135.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki136.sql
+-rw-r--r--   0        0        0    63586 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki137.sql
+-rw-r--r--   0        0        0    66990 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki138.sql
+-rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki139.sql
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/phpinfo.php
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/plantuml.sh
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/startRunJobs.sh
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/update.sh
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/mwdocker/resources/templates/upload.ini
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/scripts/install
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/tests/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/tests/basetest.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/tests/test_config.py
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/tests/test_extensions.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/tests/test_html_tables.py
+-rw-r--r--   0        0        0    11260 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/tests/test_install.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/LICENSE
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/README.md
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pymediawikidocker-0.9.9/PKG-INFO
```

### Comparing `pymediawikidocker-0.9.8/.github/workflows/build.yml` & `pymediawikidocker-0.9.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/.github/workflows/upload-to-pypi.yml` & `pymediawikidocker-0.9.9/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/.DS_Store` & `pymediawikidocker-0.9.9/mwdocker/.DS_Store`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/config.py` & `pymediawikidocker-0.9.9/mwdocker/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     version:str="1.39.3"
     smwVersion:str=None
     extensionNameList:Optional[List[str]]=field(default_factory=lambda: ["Admin Links","Header Tabs","SyntaxHighlight","Variables"])
     extensionJsonFile:str=None
     user:str="Sysop"
     prefix:str="mw"
     password_length:int = 15
+    random_password:bool=False
     password:str="sysop-1234!"
     mySQLRootPassword:str=None
     mySQLPassword:str=None
     logo:str="$wgResourceBasePath/resources/assets/wiki.png"
     port:int=9080
     sqlPort:int=9306
     prot:str="http"
@@ -114,15 +115,15 @@
         Returns:
             str: the short version string
         '''
         versionMatch=re.match("(?P<major>[0-9]+)\.(?P<minor>[0-9]+)",self.version)
         shortVersion=f"{versionMatch.group('major')}{separator}{versionMatch.group('minor')}"
         return shortVersion
     
-    def random_password(self,length:int = 15)->str:
+    def create_random_password(self,length:int = 15)->str:
         """
         create a random password
 
         Args:
             length(int): the length of the password
 
         Returns:
@@ -192,21 +193,24 @@
         self.forceRebuild=args.forceRebuild
         self.host=args.host
         self.logo=args.logo
         self.mariaDBVersion=args.mariaDBVersion
         # passwords
         self.mySQLRootPassword=args.mysqlPassword
         if not self.mySQLRootPassword:
-            self.mySQLRootPassword=self.random_password(self.password_length)
-        self.mySQLPassword=self.random_password(self.password_length)    
+            self.mySQLRootPassword=self.create_random_password(self.password_length)
+        self.mySQLPassword=self.create_random_password(self.password_length)    
         self.prot=args.prot
         self.script_path=args.script_path
         self.versions=args.versions
         self.user=args.user
+        self.random_password=args.randomPassword
+        self.force_user=args.forceUser
         self.password=args.password
+        self.password_length=args.passwordLength
         self.basePort=args.basePort
         self.sqlPort=args.sqlPort
         self.smwVersion=args.smwVersion
         self.verbose=not args.quiet
         self.debug=args.debug
         self.getExtensionMap(self.extensionNameList, self.extensionJsonFile)
    
@@ -215,21 +219,23 @@
         add Arguments to the given parser
         """
         parser.add_argument('-cn','--container_name',default=self.container_base_name,help="set container name (only valid and recommended for single version call)")
         parser.add_argument("-d", "--debug", dest="debug",   action="store_true", help="enable debug mode [default: %(default)s]")
         parser.add_argument('-el', '--extensionList', dest='extensionNameList', nargs="*",default=self.extensionNameList,help="list of extensions to be installed [default: %(default)s]")
         parser.add_argument('-ej', '--extensionJson',dest='extensionJsonFile',default=self.extensionJsonFile,help="additional extension descriptions default: [default: %(default)s]")
         parser.add_argument("-f", "--forceRebuild", action="store_true", help="force rebuilding  [default: %(default)s]")
+        parser.add_argument("-fu","--forceUser",action="store_true",help="force overwrite of wikiuser")
         parser.add_argument("--host", default=Host.get_default_host(),
                             help="the host to serve / listen from [default: %(default)s]")
         parser.add_argument("-dp","--dockerPath", default=self.default_docker_path(),
                             help="the base directory to store docker and jinja template files [default: %(default)s]")
         parser.add_argument("--logo", default=self.logo, help="set Logo [default: %(default)s]")
         parser.add_argument('-mv', '--mariaDBVersion', dest='mariaDBVersion',default=self.mariaDBVersion,help="mariaDB Version to be installed [default: %(default)s]")
         parser.add_argument('--mysqlPassword',default=self.mySQLRootPassword, help="set sqlRootPassword [default: %(default)s] - random password if None")
+        parser.add_argument("-rp", "--randomPassword", action="store_true", help="create random password and create wikiuser while at it")
         parser.add_argument('-p','--password',dest='password',default=self.password, help="set password for initial user [default: %(default)s] ")
         parser.add_argument('-pl','--passwordLength',default=self.password_length, help="set the password length for random passwords[default: %(default)s] ")
         parser.add_argument("--prefix",default=self.prefix,help="the container name prefix to use [default: %(default)s]")
         parser.add_argument("--prot",default=self.prot,help="change to https in case [default: %(default)s]")
         parser.add_argument("--script_path",default=self.script_path,help="change to any script_path you might need to set [default: %(default)s]")
         parser.add_argument('-sp', '--sqlBasePort',dest='sqlPort',type=int,default=self.sqlPort,help="set base mySql port 3306 to be exposed - incrementing by one for each version [default: %(default)s]")
         parser.add_argument('-smw','--smwVersion',dest='smwVersion',default=self.smwVersion,help="set SemanticMediaWiki Version to be installed default is None - no installation of SMW")
```

### Comparing `pymediawikidocker-0.9.8/mwdocker/docker.py` & `pymediawikidocker-0.9.9/mwdocker/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,14 +294,32 @@
             "password": f"{self.config.password}"
         }
         wikiUser=WikiUser.ofDict(userDict,encrypted=False)
         if store:
             wikiUser.save()
         return wikiUser
     
+    def createOrModifyWikiUser(self,wikiId,force_overwrite:bool=False)->WikiUser:
+        """
+        create or modify the WikiUser for this DockerApplication
+        
+        Args:
+            wikiId(str): the wikiId to create or modify a wiki user for
+            force_overwrite(bool): if True overwrite the wikuser info
+        """
+        wikiUsers=WikiUser.getWikiUsers(lenient=True)
+        if wikiId in wikiUsers and not force_overwrite:
+            wikiUser=wikiUsers[wikiId]          
+            if self.config.password != wikiUser.getPassword():
+                raise Exception(f"wikiUser for wiki {wikiId} already exists but with different password")
+            pass
+        else:
+            wikiUser=self.createWikiUser(wikiId,store=True)
+        return wikiUser
+    
     def execute(self,command_str:str):
         '''
         execute the given command string
         
         Args:
             command_str: str - a command string to be executed ...
         '''
@@ -501,14 +519,18 @@
         Args:
             overwrite(bool): if True overwrite the existing files
         '''
         self.generate("mwDockerfile",f"{self.dockerPath}/Dockerfile",composerVersion=self.composerVersion,overwrite=overwrite)
         self.generate("mwCompose.yml",f"{self.dockerPath}/docker-compose.yml",mySQLRootPassword=self.config.mySQLRootPassword,mySQLPassword=self.config.mySQLPassword,container_base_name=self.config.container_base_name,overwrite=overwrite)
         self.generate(f"mwLocalSettings{self.config.shortVersion}.php",f"{self.dockerPath}/LocalSettings.php",mySQLPassword=self.config.mySQLPassword,hostname=self.config.host,extensions=self.config.extensionMap.values(),mwShortVersion=self.config.shortVersion,logo=self.config.logo,overwrite=overwrite)
         self.generate(f"mwWiki{self.config.shortVersion}.sql",f"{self.dockerPath}/wiki.sql",overwrite=overwrite)
+        if self.config.random_password:
+            self.config.password=self.config.create_random_password(lenght=self.config.password_length)
+            if self.config.wikiId:
+                self.createOrModifyWikiUser(self.config.wikiId, force_overwrite=self.config.force_user)
         self.generate(f"addSysopUser.sh",f"{self.dockerPath}/addSysopUser.sh",user=self.config.user,password=self.config.password,overwrite=overwrite)
         self.generate(f"installExtensions.sh",f"{self.dockerPath}/installExtensions.sh",extensions=self.config.extensionMap.values(),branch=self.branch,overwrite=overwrite)
         self.genComposerRequire(f"{self.dockerPath}/composer.local.json",overwrite=overwrite)
         for fileName in ["addCronTabEntry.sh","startRunJobs.sh","initdb.sh","update.sh","phpinfo.php","upload.ini","lang.sh","plantuml.sh"]:
             self.generate(f"{fileName}",f"{self.dockerPath}/{fileName}",overwrite=overwrite)
         
     def down(self,forceRebuild:bool=False):
```

### Comparing `pymediawikidocker-0.9.8/mwdocker/html_table.py` & `pymediawikidocker-0.9.9/mwdocker/html_table.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/logger.py` & `pymediawikidocker-0.9.9/mwdocker/logger.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/mariadb.py` & `pymediawikidocker-0.9.9/mwdocker/mariadb.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/mw.py` & `pymediawikidocker-0.9.9/mwdocker/mw.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/mwcluster.py` & `pymediawikidocker-0.9.9/mwdocker/mwcluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         Returns:
             dict(str): a dict of apps by version
         '''  
         app_count=len(self.config.versions)
         for i,version in enumerate(self.config.versions):
             mwApp=self.getDockerApplication(i,app_count,version)
             if withGenerate:
-                mwApp.generateAll(overwrite=self.config.forceRebuild)
+                mwApp.generateAll(overwrite=self.config.forceRebuild)     
             self.apps[version]=mwApp    
         return self.apps
         
     def checkDocker(self)->int: 
         """
         check the Docker environment
```

### Comparing `pymediawikidocker-0.9.8/mwdocker/version.py` & `pymediawikidocker-0.9.9/mwdocker/version.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/webscrape.py` & `pymediawikidocker-0.9.9/mwdocker/webscrape.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/extensions.json` & `pymediawikidocker-0.9.9/mwdocker/resources/extensions.json`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/lang.sh` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/lang.sh`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwCompose.yml` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwCompose.yml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwDockerfile` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwDockerfile`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings.php` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings127.php` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings127.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings131.php` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings131.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings135.php` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings135.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings136.php` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings136.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings137.php` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings137.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings138.php` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings138.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwLocalSettings139.php` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwLocalSettings139.php`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki127.sql` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki127.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki131.sql` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki131.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki135.sql` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki135.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki136.sql` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki136.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki137.sql` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki137.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki138.sql` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki138.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/mwWiki139.sql` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/mwWiki139.sql`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/mwdocker/resources/templates/plantuml.sh` & `pymediawikidocker-0.9.9/mwdocker/resources/templates/plantuml.sh`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/tests/basetest.py` & `pymediawikidocker-0.9.9/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/tests/test_config.py` & `pymediawikidocker-0.9.9/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,12 +56,12 @@
         
     def test_random_password(self):
         """
         test the random password generation
         """
         config=MwClusterConfig()
         for length,chars in [(11,15),(13,18),(15,20)]:
-            rp=config.random_password(length)
+            rp=config.create_random_password(length)
             debug=self.debug
             if debug:
                 print(f"{length} bytes:{len(rp)} chars:{rp}")
             self.assertEqual(chars,len(rp))
```

### Comparing `pymediawikidocker-0.9.8/tests/test_extensions.py` & `pymediawikidocker-0.9.9/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/tests/test_html_tables.py` & `pymediawikidocker-0.9.9/tests/test_html_tables.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/tests/test_install.py` & `pymediawikidocker-0.9.9/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/.gitignore` & `pymediawikidocker-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/LICENSE` & `pymediawikidocker-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/README.md` & `pymediawikidocker-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/pyproject.toml` & `pymediawikidocker-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymediawikidocker-0.9.8/PKG-INFO` & `pymediawikidocker-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymediawikidocker
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python controlled (semantic) mediawiki docker application cluster installation
 Project-URL: Home, https://github.com/WolfgangFahl/pymediawikidocker
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/pymediawikidocker
 Project-URL: Source, https://github.com/WolfgangFahl/pymediawikidocker
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License: Apache-2.0
```

