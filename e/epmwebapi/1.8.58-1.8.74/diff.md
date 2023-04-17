# Comparing `tmp/epmwebapi-1.8.58.tar.gz` & `tmp/epmwebapi-1.8.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\epmwebapi-1.8.58.tar", last modified: Mon Oct 24 17:40:08 2022, max compression
+gzip compressed data, was "dist\epmwebapi-1.8.74.tar", last modified: Mon Apr 17 17:05:34 2023, max compression
```

## Comparing `epmwebapi-1.8.58.tar` & `epmwebapi-1.8.74.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2022-10-24 17:40:08.000000 epmwebapi-1.8.58/
-drwxrwxrwx   0        0        0        0 2022-10-24 17:40:08.000000 epmwebapi-1.8.58/epmwebapi/
--rw-rw-rw-   0        0        0     5663 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/aggregatedetails.py
--rw-rw-rw-   0        0        0     1160 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/annotationvaluejson.py
--rw-rw-rw-   0        0        0     6391 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/authorizationservice.py
--rw-rw-rw-   0        0        0      677 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/autostarttimer.py
--rw-rw-rw-   0        0        0    17437 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/basicvariable.py
--rw-rw-rw-   0        0        0      655 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/basicvariablepropertymask.py
--rw-rw-rw-   0        0        0      236 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/browsedirection.py
--rw-rw-rw-   0        0        0      892 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/browseitemmodeljson.py
--rw-rw-rw-   0        0        0      580 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/browsemodeljson.py
--rw-rw-rw-   0        0        0      493 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/browseresultitemmodeljson.py
--rw-rw-rw-   0        0        0      541 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/browseresultmodeljson.py
--rw-rw-rw-   0        0        0    10872 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/customtypedefinition.py
--rw-rw-rw-   0        0        0      490 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/dataobjectattributes.py
--rw-rw-rw-   0        0        0     1149 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/dataobjectsfilter.py
--rw-rw-rw-   0        0        0    22528 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/datasetconfig.py
--rw-rw-rw-   0        0        0    12946 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/datasetpen.py
--rw-rw-rw-   0        0        0     1522 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/datavaluejson.py
--rw-rw-rw-   0        0        0      395 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/diagnosticmodeljson.py
-drwxrwxrwx   0        0        0        0 2022-10-24 17:40:08.000000 epmwebapi-1.8.58/epmwebapi/dll_references/
--rw-rw-rw-   0        0        0   103424 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/dll_references/Elipse.Epm.AddressSpaceModel.dll
--rw-rw-rw-   0        0        0   419328 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/dll_references/EpmData.dll
--rw-rw-rw-   0        0        0      317 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/domainfilter.py
--rw-rw-rw-   0        0        0      327 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/downloadtype.py
--rw-rw-rw-   0        0        0    87052 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/epmconnection.py
--rw-rw-rw-   0        0        0     3567 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/epmconnectioncontext.py
--rw-rw-rw-   0        0        0    11086 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/epmdataobject.py
--rw-rw-rw-   0        0        0     1932 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/epmmodelobject.py
--rw-rw-rw-   0        0        0      545 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/epmnodeids.py
--rw-rw-rw-   0        0        0     2411 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/epmobject.py
--rw-rw-rw-   0        0        0      553 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/epmproperty.py
--rw-rw-rw-   0        0        0     3503 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/epmutils.py
--rw-rw-rw-   0        0        0     2829 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/epmvariable.py
--rw-rw-rw-   0        0        0      200 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/epmwebapi.py
--rw-rw-rw-   0        0        0     1039 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/folder.py
--rw-rw-rw-   0        0        0      985 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/historyprocessedmodeljson.py
--rw-rw-rw-   0        0        0      834 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/historyrawmodeljson.py
--rw-rw-rw-   0        0        0      434 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/historyresultitemmodeljson.py
--rw-rw-rw-   0        0        0      412 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/historyresultmodeljson.py
--rw-rw-rw-   0        0        0      875 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/historyupdatedataitemmodeljson.py
--rw-rw-rw-   0        0        0      518 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/historyupdatedatamodeljson.py
--rw-rw-rw-   0        0        0      436 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/historyupdateresultmodeljson.py
--rw-rw-rw-   0        0        0      338 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/historyupdatetype.py
--rw-rw-rw-   0        0        0      608 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/itempathandcontinuationpointjson.py
--rw-rw-rw-   0        0        0      913 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/itempathjson.py
--rw-rw-rw-   0        0        0     3869 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/mimetype.py
--rw-rw-rw-   0        0        0     2861 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/nodeattributes.py
--rw-rw-rw-   0        0        0     1092 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/nodeclassmask.py
--rw-rw-rw-   0        0        0     5363 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/numpyextras.py
--rw-rw-rw-   0        0        0      336 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/performupdatetype.py
--rw-rw-rw-   0        0        0      430 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/portalresources.py
--rw-rw-rw-   0        0        0      433 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/processorresources.py
--rw-rw-rw-   0        0        0     1281 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/querymodeljson.py
--rw-rw-rw-   0        0        0      639 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/queryperiod.py
--rw-rw-rw-   0        0        0      444 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/queryresultitemmodeljson.py
--rw-rw-rw-   0        0        0      371 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/queryresultmask.py
--rw-rw-rw-   0        0        0      741 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/queryresultmodeljson.py
--rw-rw-rw-   0        0        0      467 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/readitemmodeljson.py
--rw-rw-rw-   0        0        0      558 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/readmodeljson.py
--rw-rw-rw-   0        0        0      475 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/readresultitemmodeljson.py
--rw-rw-rw-   0        0        0      535 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/readresultmodeljson.py
--rw-rw-rw-   0        0        0      792 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/resource.py
--rw-rw-rw-   0        0        0     8938 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/resourcesmanager.py
--rw-rw-rw-   0        0        0    30888 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/statuscodes.py
--rw-rw-rw-   0        0        0      545 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/writeitemmodeljson.py
--rw-rw-rw-   0        0        0      444 2022-10-24 17:32:34.000000 epmwebapi-1.8.58/epmwebapi/writemodeljson.py
--rw-rw-rw-   0        0        0       24 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/_version.py
--rw-rw-rw-   0        0        0     1793 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/epmwebapi/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-24 17:40:08.000000 epmwebapi-1.8.58/epmwebapi.egg-info/
--rw-rw-rw-   0        0        0        1 2022-10-24 17:40:08.000000 epmwebapi-1.8.58/epmwebapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4768 2022-10-24 17:40:08.000000 epmwebapi-1.8.58/epmwebapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       46 2022-10-24 17:40:08.000000 epmwebapi-1.8.58/epmwebapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0     2229 2022-10-24 17:40:08.000000 epmwebapi-1.8.58/epmwebapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2022-10-24 17:40:08.000000 epmwebapi-1.8.58/epmwebapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/LICENSE.txt
--rw-rw-rw-   0        0        0     4768 2022-10-24 17:40:08.000000 epmwebapi-1.8.58/PKG-INFO
--rw-rw-rw-   0        0        0     3752 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/Readme.md
--rw-rw-rw-   0        0        0      114 2022-10-24 17:40:08.000000 epmwebapi-1.8.58/setup.cfg
--rw-rw-rw-   0        0        0     1497 2022-10-24 17:32:33.000000 epmwebapi-1.8.58/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/
+drwxrwxrwx   0        0        0        0 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/epmwebapi/
+-rw-rw-rw-   0        0        0     5663 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/aggregatedetails.py
+-rw-rw-rw-   0        0        0     1160 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/annotationvaluejson.py
+-rw-rw-rw-   0        0        0     6391 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/authorizationservice.py
+-rw-rw-rw-   0        0        0      677 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/autostarttimer.py
+-rw-rw-rw-   0        0        0    17437 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/basicvariable.py
+-rw-rw-rw-   0        0        0      655 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/basicvariablepropertymask.py
+-rw-rw-rw-   0        0        0      236 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/browsedirection.py
+-rw-rw-rw-   0        0        0      892 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/browseitemmodeljson.py
+-rw-rw-rw-   0        0        0      580 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/browsemodeljson.py
+-rw-rw-rw-   0        0        0      493 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/browseresultitemmodeljson.py
+-rw-rw-rw-   0        0        0      541 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/browseresultmodeljson.py
+-rw-rw-rw-   0        0        0    10872 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/customtypedefinition.py
+-rw-rw-rw-   0        0        0      490 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/dataobjectattributes.py
+-rw-rw-rw-   0        0        0     1149 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/dataobjectsfilter.py
+-rw-rw-rw-   0        0        0    22528 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/datasetconfig.py
+-rw-rw-rw-   0        0        0    12946 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/datasetpen.py
+-rw-rw-rw-   0        0        0     1522 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/datavaluejson.py
+-rw-rw-rw-   0        0        0      395 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/diagnosticmodeljson.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/epmwebapi/dll_references/
+-rw-rw-rw-   0        0        0   103424 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/dll_references/Elipse.Epm.AddressSpaceModel.dll
+-rw-rw-rw-   0        0        0   419328 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/dll_references/EpmData.dll
+-rw-rw-rw-   0        0        0      317 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/domainfilter.py
+-rw-rw-rw-   0        0        0      327 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/downloadtype.py
+-rw-rw-rw-   0        0        0    87052 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmconnection.py
+-rw-rw-rw-   0        0        0     3567 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmconnectioncontext.py
+-rw-rw-rw-   0        0        0    11086 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmdataobject.py
+-rw-rw-rw-   0        0        0     1932 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmmodelobject.py
+-rw-rw-rw-   0        0        0      545 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmnodeids.py
+-rw-rw-rw-   0        0        0     2411 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmobject.py
+-rw-rw-rw-   0        0        0      553 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmproperty.py
+-rw-rw-rw-   0        0        0     3503 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmutils.py
+-rw-rw-rw-   0        0        0     2829 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmvariable.py
+-rw-rw-rw-   0        0        0      200 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmwebapi.py
+-rw-rw-rw-   0        0        0     1039 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/folder.py
+-rw-rw-rw-   0        0        0      985 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyprocessedmodeljson.py
+-rw-rw-rw-   0        0        0      834 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyrawmodeljson.py
+-rw-rw-rw-   0        0        0      434 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyresultitemmodeljson.py
+-rw-rw-rw-   0        0        0      412 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyresultmodeljson.py
+-rw-rw-rw-   0        0        0      875 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyupdatedataitemmodeljson.py
+-rw-rw-rw-   0        0        0      518 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyupdatedatamodeljson.py
+-rw-rw-rw-   0        0        0      436 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyupdateresultmodeljson.py
+-rw-rw-rw-   0        0        0      338 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyupdatetype.py
+-rw-rw-rw-   0        0        0      608 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/itempathandcontinuationpointjson.py
+-rw-rw-rw-   0        0        0      913 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/itempathjson.py
+-rw-rw-rw-   0        0        0     3869 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/mimetype.py
+-rw-rw-rw-   0        0        0     2861 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/nodeattributes.py
+-rw-rw-rw-   0        0        0     1092 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/nodeclassmask.py
+-rw-rw-rw-   0        0        0     5363 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/numpyextras.py
+-rw-rw-rw-   0        0        0      336 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/performupdatetype.py
+-rw-rw-rw-   0        0        0      430 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/portalresources.py
+-rw-rw-rw-   0        0        0      433 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/processorresources.py
+-rw-rw-rw-   0        0        0     1281 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/querymodeljson.py
+-rw-rw-rw-   0        0        0      639 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/queryperiod.py
+-rw-rw-rw-   0        0        0      444 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/queryresultitemmodeljson.py
+-rw-rw-rw-   0        0        0      371 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/queryresultmask.py
+-rw-rw-rw-   0        0        0      741 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/queryresultmodeljson.py
+-rw-rw-rw-   0        0        0      467 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/readitemmodeljson.py
+-rw-rw-rw-   0        0        0      558 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/readmodeljson.py
+-rw-rw-rw-   0        0        0      475 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/readresultitemmodeljson.py
+-rw-rw-rw-   0        0        0      535 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/readresultmodeljson.py
+-rw-rw-rw-   0        0        0      792 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/resource.py
+-rw-rw-rw-   0        0        0     8938 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/resourcesmanager.py
+-rw-rw-rw-   0        0        0    30888 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/statuscodes.py
+-rw-rw-rw-   0        0        0      545 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/writeitemmodeljson.py
+-rw-rw-rw-   0        0        0      444 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/writemodeljson.py
+-rw-rw-rw-   0        0        0       24 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/_version.py
+-rw-rw-rw-   0        0        0     1793 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/epmwebapi.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-17 17:05:33.000000 epmwebapi-1.8.74/epmwebapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4768 2023-04-17 17:05:33.000000 epmwebapi-1.8.74/epmwebapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-04-17 17:05:33.000000 epmwebapi-1.8.74/epmwebapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     2229 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/epmwebapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 17:05:33.000000 epmwebapi-1.8.74/epmwebapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/LICENSE.txt
+-rw-rw-rw-   0        0        0     4768 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/PKG-INFO
+-rw-rw-rw-   0        0        0     3752 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/Readme.md
+-rw-rw-rw-   0        0        0      114 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/setup.cfg
+-rw-rw-rw-   0        0        0     1497 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/setup.py
```

### Comparing `epmwebapi-1.8.58/epmwebapi/aggregatedetails.py` & `epmwebapi-1.8.74/epmwebapi/aggregatedetails.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/annotationvaluejson.py` & `epmwebapi-1.8.74/epmwebapi/annotationvaluejson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/authorizationservice.py` & `epmwebapi-1.8.74/epmwebapi/authorizationservice.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/autostarttimer.py` & `epmwebapi-1.8.74/epmwebapi/autostarttimer.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/basicvariable.py` & `epmwebapi-1.8.74/epmwebapi/basicvariable.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/basicvariablepropertymask.py` & `epmwebapi-1.8.74/epmwebapi/basicvariablepropertymask.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/browseitemmodeljson.py` & `epmwebapi-1.8.74/epmwebapi/browseitemmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/browsemodeljson.py` & `epmwebapi-1.8.74/epmwebapi/browsemodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/browseresultmodeljson.py` & `epmwebapi-1.8.74/epmwebapi/browseresultmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/customtypedefinition.py` & `epmwebapi-1.8.74/epmwebapi/customtypedefinition.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/dataobjectsfilter.py` & `epmwebapi-1.8.74/epmwebapi/dataobjectsfilter.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/datasetconfig.py` & `epmwebapi-1.8.74/epmwebapi/datasetconfig.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/datasetpen.py` & `epmwebapi-1.8.74/epmwebapi/datasetpen.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/datavaluejson.py` & `epmwebapi-1.8.74/epmwebapi/datavaluejson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/dll_references/Elipse.Epm.AddressSpaceModel.dll` & `epmwebapi-1.8.74/epmwebapi/dll_references/Elipse.Epm.AddressSpaceModel.dll`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/dll_references/EpmData.dll` & `epmwebapi-1.8.74/epmwebapi/dll_references/EpmData.dll`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/epmconnection.py` & `epmwebapi-1.8.74/epmwebapi/epmconnection.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/epmconnectioncontext.py` & `epmwebapi-1.8.74/epmwebapi/epmconnectioncontext.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/epmdataobject.py` & `epmwebapi-1.8.74/epmwebapi/epmdataobject.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/epmmodelobject.py` & `epmwebapi-1.8.74/epmwebapi/epmmodelobject.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/epmnodeids.py` & `epmwebapi-1.8.74/epmwebapi/epmnodeids.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/epmobject.py` & `epmwebapi-1.8.74/epmwebapi/epmobject.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/epmproperty.py` & `epmwebapi-1.8.74/epmwebapi/epmproperty.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/epmutils.py` & `epmwebapi-1.8.74/epmwebapi/epmutils.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/epmvariable.py` & `epmwebapi-1.8.74/epmwebapi/epmvariable.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/folder.py` & `epmwebapi-1.8.74/epmwebapi/folder.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/historyprocessedmodeljson.py` & `epmwebapi-1.8.74/epmwebapi/historyprocessedmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/historyrawmodeljson.py` & `epmwebapi-1.8.74/epmwebapi/historyrawmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/historyupdatedataitemmodeljson.py` & `epmwebapi-1.8.74/epmwebapi/historyupdatedataitemmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/historyupdatedatamodeljson.py` & `epmwebapi-1.8.74/epmwebapi/historyupdatedatamodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/itempathandcontinuationpointjson.py` & `epmwebapi-1.8.74/epmwebapi/itempathandcontinuationpointjson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/itempathjson.py` & `epmwebapi-1.8.74/epmwebapi/itempathjson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/mimetype.py` & `epmwebapi-1.8.74/epmwebapi/mimetype.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/nodeattributes.py` & `epmwebapi-1.8.74/epmwebapi/nodeattributes.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/nodeclassmask.py` & `epmwebapi-1.8.74/epmwebapi/nodeclassmask.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/numpyextras.py` & `epmwebapi-1.8.74/epmwebapi/numpyextras.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/querymodeljson.py` & `epmwebapi-1.8.74/epmwebapi/querymodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/queryperiod.py` & `epmwebapi-1.8.74/epmwebapi/queryperiod.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/queryresultmodeljson.py` & `epmwebapi-1.8.74/epmwebapi/queryresultmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/readmodeljson.py` & `epmwebapi-1.8.74/epmwebapi/readmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/readresultmodeljson.py` & `epmwebapi-1.8.74/epmwebapi/readresultmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/resource.py` & `epmwebapi-1.8.74/epmwebapi/resource.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/resourcesmanager.py` & `epmwebapi-1.8.74/epmwebapi/resourcesmanager.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/statuscodes.py` & `epmwebapi-1.8.74/epmwebapi/statuscodes.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/writeitemmodeljson.py` & `epmwebapi-1.8.74/epmwebapi/writeitemmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi/__init__.py` & `epmwebapi-1.8.74/epmwebapi/__init__.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/epmwebapi.egg-info/PKG-INFO` & `epmwebapi-1.8.74/epmwebapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epmwebapi
-Version: 1.8.58
+Version: 1.8.74
 Summary: UNKNOWN
 Home-page: https://github.com/elipsesoftware/epmwebapi
 Author: Elipse Software Ltda
 License: UNKNOWN
 Description: # epmwebapi
         
         A biblioteca **Epmwebapi** desenvolvida pela **Elipse Software**, permite a interação com os dados da sua plataforma
```

### Comparing `epmwebapi-1.8.58/epmwebapi.egg-info/SOURCES.txt` & `epmwebapi-1.8.74/epmwebapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/LICENSE.txt` & `epmwebapi-1.8.74/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/PKG-INFO` & `epmwebapi-1.8.74/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epmwebapi
-Version: 1.8.58
+Version: 1.8.74
 Summary: UNKNOWN
 Home-page: https://github.com/elipsesoftware/epmwebapi
 Author: Elipse Software Ltda
 License: UNKNOWN
 Description: # epmwebapi
         
         A biblioteca **Epmwebapi** desenvolvida pela **Elipse Software**, permite a interação com os dados da sua plataforma
```

### Comparing `epmwebapi-1.8.58/Readme.md` & `epmwebapi-1.8.74/Readme.md`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.58/setup.py` & `epmwebapi-1.8.74/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name = 'epmwebapi', 
-      version = '1.8.58', 
+      version = '1.8.74', 
       author = 'Elipse Software Ltda', 
       packages = ['epmwebapi'], 
       include_package_data=True,
       description = '', 
       long_description = long_description, 
       long_description_content_type='text/markdown',
       url = 'https://github.com/elipsesoftware/epmwebapi',
```

