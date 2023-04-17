# Comparing `tmp/hdpws-0.4.2.tar.gz` & `tmp/hdpws-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdpws-0.4.2.tar", last modified: Tue Mar 21 11:24:36 2023, max compression
+gzip compressed data, was "hdpws-0.6.2.tar", last modified: Mon Apr 17 11:42:14 2023, max compression
```

## Comparing `hdpws-0.4.2.tar` & `hdpws-0.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 btharris (971688066) staff       (20)        0 2023-03-21 11:24:36.345137 hdpws-0.4.2/
--rw-------   0 btharris (971688066) staff       (20)    12589 2023-02-22 18:33:31.000000 hdpws-0.4.2/LICENSE
--rw-------   0 btharris (971688066) staff       (20)     3320 2023-03-21 11:24:36.344841 hdpws-0.4.2/PKG-INFO
--rw-------   0 btharris (971688066) staff       (20)     2334 2023-03-17 14:02:16.000000 hdpws-0.4.2/README.md
-drwx------   0 btharris (971688066) staff       (20)        0 2023-03-21 11:24:36.342683 hdpws-0.4.2/hdpws/
--rwx------   0 btharris (971688066) staff       (20)     2048 2023-03-21 11:04:26.000000 hdpws-0.4.2/hdpws/__init__.py
--rwx------   0 btharris (971688066) staff       (20)    12007 2023-03-21 11:17:36.000000 hdpws-0.4.2/hdpws/__main__.py
--rw-------   0 btharris (971688066) staff       (20)     4901 2023-02-27 14:08:19.000000 hdpws-0.4.2/hdpws/dateinterval.py
--rwx------   0 btharris (971688066) staff       (20)    28927 2023-03-21 11:08:19.000000 hdpws-0.4.2/hdpws/hdpws.py
--rwx------   0 btharris (971688066) staff       (20)     1745 2023-03-21 11:12:21.000000 hdpws-0.4.2/hdpws/resourcetype.py
-drwx------   0 btharris (971688066) staff       (20)        0 2023-03-21 11:24:36.344434 hdpws-0.4.2/hdpws.egg-info/
--rw-------   0 btharris (971688066) staff       (20)     3320 2023-03-21 11:24:36.000000 hdpws-0.4.2/hdpws.egg-info/PKG-INFO
--rw-------   0 btharris (971688066) staff       (20)      265 2023-03-21 11:24:36.000000 hdpws-0.4.2/hdpws.egg-info/SOURCES.txt
--rw-------   0 btharris (971688066) staff       (20)        1 2023-03-21 11:24:36.000000 hdpws-0.4.2/hdpws.egg-info/dependency_links.txt
--rw-------   0 btharris (971688066) staff       (20)       38 2023-03-21 11:24:36.000000 hdpws-0.4.2/hdpws.egg-info/requires.txt
--rw-------   0 btharris (971688066) staff       (20)        6 2023-03-21 11:24:36.000000 hdpws-0.4.2/hdpws.egg-info/top_level.txt
--rw-------   0 btharris (971688066) staff       (20)       38 2023-03-21 11:24:36.345232 hdpws-0.4.2/setup.cfg
--rw-------   0 btharris (971688066) staff       (20)     1742 2023-03-21 11:04:11.000000 hdpws-0.4.2/setup.py
+drwx------   0 btharris (971688066) staff       (20)        0 2023-04-17 11:42:14.664165 hdpws-0.6.2/
+-rw-------   0 btharris (971688066) staff       (20)    12589 2023-02-22 18:33:31.000000 hdpws-0.6.2/LICENSE
+-rw-------   0 btharris (971688066) staff       (20)     3320 2023-04-17 11:42:14.663821 hdpws-0.6.2/PKG-INFO
+-rw-------   0 btharris (971688066) staff       (20)     2334 2023-03-17 14:02:16.000000 hdpws-0.6.2/README.md
+drwx------   0 btharris (971688066) staff       (20)        0 2023-04-17 11:42:14.661248 hdpws-0.6.2/hdpws/
+-rwx------   0 btharris (971688066) staff       (20)     2048 2023-04-17 09:02:11.000000 hdpws-0.6.2/hdpws/__init__.py
+-rwx------   0 btharris (971688066) staff       (20)    12133 2023-04-05 17:30:02.000000 hdpws-0.6.2/hdpws/__main__.py
+-rw-------   0 btharris (971688066) staff       (20)     4901 2023-02-27 14:08:19.000000 hdpws-0.6.2/hdpws/dateinterval.py
+-rwx------   0 btharris (971688066) staff       (20)    29949 2023-04-05 17:30:51.000000 hdpws-0.6.2/hdpws/hdpws.py
+-rwx------   0 btharris (971688066) staff       (20)     1745 2023-03-21 11:12:21.000000 hdpws-0.6.2/hdpws/resourcetype.py
+drwx------   0 btharris (971688066) staff       (20)        0 2023-04-17 11:42:14.663372 hdpws-0.6.2/hdpws.egg-info/
+-rw-------   0 btharris (971688066) staff       (20)     3320 2023-04-17 11:42:14.000000 hdpws-0.6.2/hdpws.egg-info/PKG-INFO
+-rw-------   0 btharris (971688066) staff       (20)      265 2023-04-17 11:42:14.000000 hdpws-0.6.2/hdpws.egg-info/SOURCES.txt
+-rw-------   0 btharris (971688066) staff       (20)        1 2023-04-17 11:42:14.000000 hdpws-0.6.2/hdpws.egg-info/dependency_links.txt
+-rw-------   0 btharris (971688066) staff       (20)       38 2023-04-17 11:42:14.000000 hdpws-0.6.2/hdpws.egg-info/requires.txt
+-rw-------   0 btharris (971688066) staff       (20)        6 2023-04-17 11:42:14.000000 hdpws-0.6.2/hdpws.egg-info/top_level.txt
+-rw-------   0 btharris (971688066) staff       (20)       38 2023-04-17 11:42:14.664280 hdpws-0.6.2/setup.cfg
+-rw-------   0 btharris (971688066) staff       (20)     1742 2023-04-17 09:02:17.000000 hdpws-0.6.2/setup.py
```

### Comparing `hdpws-0.4.2/LICENSE` & `hdpws-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdpws-0.4.2/PKG-INFO` & `hdpws-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdpws
-Version: 0.4.2
+Version: 0.6.2
 Summary: NASA's Heliophysics Data Portal Web Service Client Library
 Home-page: https://heliophysicsdata.gsfc.nasa.gov/WebServices
 Author: Bernie Harris
 Author-email: NASA-SPDF-Support@nasa.onmicrosoft.com
 License: NOSA
 Keywords: heliophysics,spase,space physics,spdf,hdp
 Platform: UNKNOWN
```

### Comparing `hdpws-0.4.2/README.md` & `hdpws-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `hdpws-0.4.2/hdpws/__init__.py` & `hdpws-0.6.2/hdpws/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 Copyright &copy; 2023 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 
 """
 
 
-__version__ = "0.4.2"
+__version__ = "0.6.2"
 
 
 #
 # Limit on the number of times an HTTP request which returns a
 # 429 or 503 status with a Retry-After header will be retried.
 #
 #RETRY_LIMIT = 100
```

### Comparing `hdpws-0.4.2/hdpws/__main__.py` & `hdpws-0.6.2/hdpws/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 import logging.config
 from typing import Dict, List
 import xml.etree.ElementTree as ET  # pylint: disable=unused-import
 import urllib3
 
 
 from hdpws.hdpws import HdpWs
-from hdpws import NAMESPACES
+from hdpws import NAMESPACES as NS
 from hdpws.resourcetype import ResourceType as rt
 
 
 logging.basicConfig()
 LOGGING_CONFIG_FILE = 'logging_config.json'
 try:
     with open(LOGGING_CONFIG_FILE, 'r', encoding='utf-8') as fd:
@@ -211,27 +211,35 @@
         print('HDP Observed Regions:')
         for value in result['ObservedRegion'][0:5]:
             print(f'    {value}')
         print('    ...')
     else:
         print_error('hdp.get_observed_regions', result)
 
+    result = hdp.get_styles()
+    if result['HttpStatus'] == 200:
+        print('HDP Styles:')
+        for value in result['Style']:
+            print(f'    {value}')
+    else:
+        print_error('hdp.get_styles', result)
+
 
     resource_ids = [
         'spase://NASA/Collection/IRIS_AIA',
         'spase://SMWG/Service/CCMC/Models'
     ]
     result = hdp.get_spase(resource_ids)
     if result['HttpStatus'] == 200:
         #print('HDP Spase:')
         #print(ET.tostring(result['Result']))
         print('get_spase Result ResourceIDs:')
-        for spase in result['Result'].findall('.//Spase', namespaces=NAMESPACES):
-            print(spase.findall('.//ResourceID', namespaces=NAMESPACES)[0].text)
-            print('    ', spase.findall('.//ResourceName', namespaces=NAMESPACES)[0].text)
+        for spase in result['Result'].findall('.//Spase', namespaces=NS):
+            print(spase.findall('.//ResourceID', namespaces=NS)[0].text)
+            print('    ', spase.findall('.//ResourceName', namespaces=NS)[0].text)
     else:
         print_error('hdp.get_spase_data', result)
 
 
     query = {
         'ResourceID': ['spase://NASA/NumericalData/ACE/CRIS/L2/P1D',
             'spase://NASA/NumericalData/ACE/CRIS/L2/PT1H'
@@ -248,15 +256,15 @@
     time_range = ['2022-01-01', '2022-01-02']
 
     result = hdp.get_spase_data(types, query, time_range)
     if result['HttpStatus'] == 200:
         #print('HDP Spase:')
         #print(ET.tostring(result['Result']))
         print('get_spase_data Result ResourceIDs:')
-        for r_id in result['Result'].findall('.//ResourceID', namespaces=NAMESPACES):
+        for r_id in result['Result'].findall('.//ResourceID', namespaces=NS):
             print(r_id.text)
     else:
         print_error('hdp.get_spase_data', result)
 
 
     query = {
         'ResourceID': ['spase://NASA/NumericalData/ACE/MAG/L2/PT16S', 'bad']
@@ -278,17 +286,17 @@
     time_range = ['1999-01-01', '1999-01-02']
 
     result = hdp.get_spase_catalog(query, time_range)
     if result['HttpStatus'] == 200:
         #print('HDP Spase:')
         #print(ET.tostring(result['Result']))
         print('Result Catalogs:')
-        for catalog in result['Result'].findall('.//Catalog', namespaces=NAMESPACES):
-            print(catalog.findall('.//ResourceID', namespaces=NAMESPACES)[0].text)
-            print('    ', catalog.findall('.//ResourceName', namespaces=NAMESPACES)[0].text)
+        for catalog in result['Result'].findall('.//Catalog', namespaces=NS):
+            print(catalog.findall('.//ResourceID', namespaces=NS)[0].text)
+            print('    ', catalog.findall('.//ResourceName', namespaces=NS)[0].text)
             #ET.indent(catalog)
             #print(ET.tostring(catalog, encoding='unicode',
             #                  default_namespace=SPASE_NS))
     else:
         print_error('hdp.get_spase_catalog', result)
 
 
@@ -299,17 +307,17 @@
     }
 
     result = hdp.get_spase_collection(query)
     if result['HttpStatus'] == 200:
         #print('HDP Spase:')
         #print(ET.tostring(result['Result']))
         print('Result Collections:')
-        for collection in result['Result'].findall('.//Collection', namespaces=NAMESPACES):
-            print(collection.findall('.//ResourceID', namespaces=NAMESPACES)[0].text)
-            print('    ', collection.findall('.//ResourceName', namespaces=NAMESPACES)[0].text)
+        for collection in result['Result'].findall('.//Collection', namespaces=NS):
+            print(collection.findall('.//ResourceID', namespaces=NS)[0].text)
+            print('    ', collection.findall('.//ResourceName', namespaces=NS)[0].text)
             #ET.indent(collection)
             #print(ET.tostring(collection, encoding='unicode',
             #                  default_namespace=SPASE_NS))
     else:
         print_error('hdp.get_spase_collection', result)
 
 
@@ -320,17 +328,17 @@
     }
 
     result = hdp.get_spase_document(query)
     if result['HttpStatus'] == 200:
         #print('HDP Spase:')
         #print(ET.tostring(result['Result']))
         print('Result Documents:')
-        for document in result['Result'].findall('.//Document', namespaces=NAMESPACES):
-            print(document.findall('.//ResourceID', namespaces=NAMESPACES)[0].text)
-            print('    ', document.findall('.//ResourceName', namespaces=NAMESPACES)[0].text)
+        for document in result['Result'].findall('.//Document', namespaces=NS):
+            print(document.findall('.//ResourceID', namespaces=NS)[0].text)
+            print('    ', document.findall('.//ResourceName', namespaces=NS)[0].text)
             #ET.indent(document)
             #print(ET.tostring(document, encoding='unicode',
             #                  default_namespace=SPASE_NS))
     else:
         print_error('hdp.get_spase_document', result)
```

### Comparing `hdpws-0.4.2/hdpws/dateinterval.py` & `hdpws-0.6.2/hdpws/dateinterval.py`

 * *Files identical despite different names*

### Comparing `hdpws-0.4.2/hdpws/hdpws.py` & `hdpws-0.6.2/hdpws/hdpws.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 import platform
 import xml.etree.ElementTree as ET
 from xml.etree.ElementTree import ParseError
 import logging
 from typing import Dict, List, Union
 import requests
 
-from hdpws import __version__, NAMESPACES
+from hdpws import __version__, NAMESPACES as NS
 from hdpws.dateinterval import DateInterval
 from hdpws.resourcetype import ResourceType
 
 
 
 class HdpWs:
     """
@@ -229,14 +229,42 @@
             - ErrorDescription: value from HttpText.<br>
         """
         return self.__get_simple_resource('Spase/Repository/ResourceID',
                                           'ResourceID', 
                                           'RepositoryID')
 
 
+    def get_styles(
+            self
+        ) -> Dict:
+        """
+        Gets all /Spase/Style values available at HDP.
+
+        Returns
+        -------
+        Dict
+            Dictionary containing a 'Style' key with a value
+            of a List containing all /Spase/Style values
+            with the addition of the following key/values:<br>
+            - HttpStatus: with the value of the HTTP status code.
+              Successful == 200.<br>
+            When HttpStatus != 200:<br>
+            - HttpText: containing a string representation of the HTTP
+              entity body.<br>
+            When HttpText is a standard HDP WS error entity body the
+            following key/values (convenience to avoid parsing
+            HttpStatus):<br>
+            - ErrorMessage: value from HttpText.<br>
+            - ErrorDescription: value from HttpText.<br>
+        """
+        return self.__get_simple_resource('Spase/Style',
+                                          'Style', 
+                                          'Style')
+
+
     def get_measurement_types(
             self
         ) -> Dict:
         """
         Gets all /Spase/MeasurementType values available at HDP.
 
         Returns
@@ -672,15 +700,15 @@
         mt_response = ET.fromstring(response.text)
 
         result = {
             result_name: []
         }
 
         for value in mt_response.findall('.//hdp:' + name,
-                                         namespaces=NAMESPACES):
+                                         namespaces=NS):
 
             result[result_name].append(value.text)
 
         result.update(status)
         return result
 
 
@@ -784,15 +812,15 @@
         if response.status_code != 200:
 
             http_result['ErrorText'] = response.text
             try:
                 error_element = ET.fromstring(response.text)
                 http_result['ErrorMessage'] = error_element.findall(\
                     './/xhtml:p[@class="ErrorMessage"]/xhtml:b',
-                    namespaces=NAMESPACES)[0].tail
+                    namespaces=NS)[0].tail
                 http_result['ErrorDescription'] = error_element.findall(\
                     './/xhtml:p[@class="ErrorDescription"]/xhtml:b',
-                    namespaces=NAMESPACES)[0].tail
+                    namespaces=NS)[0].tail
             except ParseError:
                 pass  # ErrorText is the best we can do
 
         return http_result
```

### Comparing `hdpws-0.4.2/hdpws/resourcetype.py` & `hdpws-0.6.2/hdpws/resourcetype.py`

 * *Files identical despite different names*

### Comparing `hdpws-0.4.2/hdpws.egg-info/PKG-INFO` & `hdpws-0.6.2/hdpws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdpws
-Version: 0.4.2
+Version: 0.6.2
 Summary: NASA's Heliophysics Data Portal Web Service Client Library
 Home-page: https://heliophysicsdata.gsfc.nasa.gov/WebServices
 Author: Bernie Harris
 Author-email: NASA-SPDF-Support@nasa.onmicrosoft.com
 License: NOSA
 Keywords: heliophysics,spase,space physics,spdf,hdp
 Platform: UNKNOWN
```

### Comparing `hdpws-0.4.2/setup.py` & `hdpws-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="hdpws",
-    version="0.4.2",
+    version="0.6.2",
     description="NASA's Heliophysics Data Portal Web Service Client Library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://heliophysicsdata.gsfc.nasa.gov/WebServices",
     author="Bernie Harris",
     author_email="NASA-SPDF-Support@nasa.onmicrosoft.com",
     license="NOSA",
```

