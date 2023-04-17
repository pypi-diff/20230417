# Comparing `tmp/mailchimp3-3.0.7.tar.gz` & `tmp/mailchimp3-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mailchimp3-3.0.7.tar", last modified: Thu Mar 28 11:33:11 2019, max compression
+gzip compressed data, was "dist/mailchimp3-3.0.9.tar", last modified: Tue Sep 10 06:35:44 2019, max compression
```

## Comparing `mailchimp3-3.0.7.tar` & `mailchimp3-3.0.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 charlesthk   (501) staff       (20)        0 2019-03-28 11:33:11.000000 mailchimp3-3.0.7/
--rw-r--r--   0 charlesthk   (501) staff       (20)    32418 2019-03-28 11:33:11.000000 mailchimp3-3.0.7/PKG-INFO
-drwxr-xr-x   0 charlesthk   (501) staff       (20)        0 2019-03-28 11:33:11.000000 mailchimp3-3.0.7/mailchimp3.egg-info/
--rw-r--r--   0 charlesthk   (501) staff       (20)    32418 2019-03-28 11:33:11.000000 mailchimp3-3.0.7/mailchimp3.egg-info/PKG-INFO
--rw-r--r--   0 charlesthk   (501) staff       (20)     3049 2019-03-28 11:33:11.000000 mailchimp3-3.0.7/mailchimp3.egg-info/SOURCES.txt
--rw-r--r--   0 charlesthk   (501) staff       (20)       16 2019-03-28 11:33:11.000000 mailchimp3-3.0.7/mailchimp3.egg-info/requires.txt
--rw-r--r--   0 charlesthk   (501) staff       (20)       11 2019-03-28 11:33:11.000000 mailchimp3-3.0.7/mailchimp3.egg-info/top_level.txt
--rw-r--r--   0 charlesthk   (501) staff       (20)        1 2019-03-28 11:33:11.000000 mailchimp3-3.0.7/mailchimp3.egg-info/dependency_links.txt
--rw-r--r--   0 charlesthk   (501) staff       (20)     1396 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/setup.py
--rw-r--r--   0 charlesthk   (501) staff       (20)       67 2019-03-28 11:33:11.000000 mailchimp3-3.0.7/setup.cfg
-drwxr-xr-x   0 charlesthk   (501) staff       (20)        0 2019-03-28 11:33:11.000000 mailchimp3-3.0.7/mailchimp3/
--rw-r--r--   0 charlesthk   (501) staff       (20)     2642 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/baseapi.py
--rwxr-xr-x   0 charlesthk   (501) staff       (20)     9536 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/__init__.py
--rw-r--r--   0 charlesthk   (501) staff       (20)    10313 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/mailchimpclient.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     3622 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/helpers.py
-drwxr-xr-x   0 charlesthk   (501) staff       (20)        0 2019-03-28 11:33:11.000000 mailchimp3-3.0.7/mailchimp3/entities/
--rw-r--r--   0 charlesthk   (501) staff       (20)     1307 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportsubreports.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1600 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/searchmembers.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     6144 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listmembernotes.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1850 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportcampaignabusereports.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     5458 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listinterestcategories.py
--rw-r--r--   0 charlesthk   (501) staff       (20)    12424 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/lists.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     5843 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/storecustomers.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2300 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listabusereports.py
--rwxr-xr-x   0 charlesthk   (501) staff       (20)     1622 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/campaigncontent.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1561 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listmembergoals.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1368 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/automationactions.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     4497 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/campaignfeedback.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2253 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/automationemailactions.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2776 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listmembertags.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     6253 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/storeproductvariants.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1473 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportlocations.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1302 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/segments.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     5847 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listinterestcategoryinterest.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1306 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listactivity.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     4116 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listmergefields.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1522 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listsignupforms.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2395 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportclickdetailreports.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     4344 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listsegmentmembers.py
--rw-r--r--   0 charlesthk   (501) staff       (20)        0 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/__init__.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2327 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/automationemails.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     4360 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/stores.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1248 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/searchcampaigns.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     3327 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/campaignfolders.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1277 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportcampaignadvice.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2505 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/authorizedapps.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     4888 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/storeproducts.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     5203 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listsegments.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2385 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportsentto.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2175 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/automationremovedsubscribers.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     8127 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listmembers.py
--rwxr-xr-x   0 charlesthk   (501) staff       (20)     8135 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/campaigns.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     3461 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/batchwebhooks.py
--rwxr-xr-x   0 charlesthk   (501) staff       (20)     3604 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/filemanagerfolders.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     5203 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/storecartlines.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     3945 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/templates.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2559 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportemailactivity.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     5290 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/storeorderlines.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     3493 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/conversationmessages.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2459 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/automations.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     3954 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/filemanagerfiles.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     3571 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/batchoperations.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1734 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportopendetails.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     3460 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reports.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2207 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listgrowthhistory.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1175 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reporteepurl.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     5664 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/storecarts.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     3628 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/automationemailqueues.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2211 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportgoogleanalytics.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1266 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/campaignsendchecklist.py
--rw-r--r--   0 charlesthk   (501) staff       (20)      982 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/root.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1253 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/templatedefaultcontent.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     6741 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/storeorders.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     4893 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/storepromorules.py
--rwxr-xr-x   0 charlesthk   (501) staff       (20)     5267 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/campaignactions.py
--rwxr-xr-x   0 charlesthk   (501) staff       (20)     3340 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/templatefolders.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     4947 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/storeproductimages.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2482 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportunsubscribes.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1165 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listclients.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     2227 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/conversations.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     3016 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportclickdetailmembers.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1618 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listmemberactivity.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     5300 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/storepromocodes.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     3461 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/listwebhooks.py
--rw-r--r--   0 charlesthk   (501) staff       (20)      685 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/ping.py
--rw-r--r--   0 charlesthk   (501) staff       (20)     1234 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/mailchimp3/entities/reportdomainperformance.py
--rw-r--r--   0 charlesthk   (501) staff       (20)    24115 2019-03-28 11:32:25.000000 mailchimp3-3.0.7/README.rst
+drwxr-xr-x   0 charlesthk   (501) staff       (20)        0 2019-09-10 06:35:44.000000 mailchimp3-3.0.9/
+-rw-r--r--   0 charlesthk   (501) staff       (20)    32453 2019-09-10 06:35:44.000000 mailchimp3-3.0.9/PKG-INFO
+drwxr-xr-x   0 charlesthk   (501) staff       (20)        0 2019-09-10 06:35:44.000000 mailchimp3-3.0.9/mailchimp3.egg-info/
+-rw-r--r--   0 charlesthk   (501) staff       (20)    32453 2019-09-10 06:35:44.000000 mailchimp3-3.0.9/mailchimp3.egg-info/PKG-INFO
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3049 2019-09-10 06:35:44.000000 mailchimp3-3.0.9/mailchimp3.egg-info/SOURCES.txt
+-rw-r--r--   0 charlesthk   (501) staff       (20)       16 2019-09-10 06:35:44.000000 mailchimp3-3.0.9/mailchimp3.egg-info/requires.txt
+-rw-r--r--   0 charlesthk   (501) staff       (20)       11 2019-09-10 06:35:44.000000 mailchimp3-3.0.9/mailchimp3.egg-info/top_level.txt
+-rw-r--r--   0 charlesthk   (501) staff       (20)        1 2019-09-10 06:35:44.000000 mailchimp3-3.0.9/mailchimp3.egg-info/dependency_links.txt
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1396 2019-09-10 06:32:01.000000 mailchimp3-3.0.9/setup.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)       67 2019-09-10 06:35:44.000000 mailchimp3-3.0.9/setup.cfg
+drwxr-xr-x   0 charlesthk   (501) staff       (20)        0 2019-09-10 06:35:44.000000 mailchimp3-3.0.9/mailchimp3/
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2881 2019-09-10 06:32:01.000000 mailchimp3-3.0.9/mailchimp3/baseapi.py
+-rwxr-xr-x   0 charlesthk   (501) staff       (20)     9536 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/__init__.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)    10067 2019-09-10 06:32:01.000000 mailchimp3-3.0.9/mailchimp3/mailchimpclient.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3622 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/helpers.py
+drwxr-xr-x   0 charlesthk   (501) staff       (20)        0 2019-09-10 06:35:44.000000 mailchimp3-3.0.9/mailchimp3/entities/
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1307 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportsubreports.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1600 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/searchmembers.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     6144 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listmembernotes.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1850 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportcampaignabusereports.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     5458 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listinterestcategories.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)    12424 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/lists.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     5843 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/storecustomers.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2300 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listabusereports.py
+-rwxr-xr-x   0 charlesthk   (501) staff       (20)     1622 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/campaigncontent.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1561 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listmembergoals.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1368 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/automationactions.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     4497 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/campaignfeedback.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2253 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/automationemailactions.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2776 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listmembertags.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     6253 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/storeproductvariants.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1473 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportlocations.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1302 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/segments.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     5847 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listinterestcategoryinterest.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1306 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listactivity.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     4116 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listmergefields.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1522 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listsignupforms.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2395 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportclickdetailreports.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     4344 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listsegmentmembers.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)        0 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/__init__.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2327 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/automationemails.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     4360 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/stores.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1248 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/searchcampaigns.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3327 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/campaignfolders.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1277 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportcampaignadvice.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2505 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/authorizedapps.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     4888 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/storeproducts.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     5203 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listsegments.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2385 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportsentto.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2175 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/automationremovedsubscribers.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     8127 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listmembers.py
+-rwxr-xr-x   0 charlesthk   (501) staff       (20)     8135 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/campaigns.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3461 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/batchwebhooks.py
+-rwxr-xr-x   0 charlesthk   (501) staff       (20)     3604 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/filemanagerfolders.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     5203 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/storecartlines.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3945 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/templates.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2559 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportemailactivity.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     5290 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/storeorderlines.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3493 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/conversationmessages.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2459 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/automations.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3954 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/filemanagerfiles.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3571 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/batchoperations.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1734 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportopendetails.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3460 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reports.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2207 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listgrowthhistory.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1175 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reporteepurl.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     5664 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/storecarts.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3628 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/automationemailqueues.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2211 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportgoogleanalytics.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1266 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/campaignsendchecklist.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)      982 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/root.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1253 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/templatedefaultcontent.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     6741 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/storeorders.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     4893 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/storepromorules.py
+-rwxr-xr-x   0 charlesthk   (501) staff       (20)     5267 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/campaignactions.py
+-rwxr-xr-x   0 charlesthk   (501) staff       (20)     3340 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/templatefolders.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     4947 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/storeproductimages.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2482 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportunsubscribes.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1165 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listclients.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     2227 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/conversations.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3016 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportclickdetailmembers.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1618 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listmemberactivity.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     5300 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/storepromocodes.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     3461 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/listwebhooks.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)      685 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/ping.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)     1234 2019-03-28 11:32:25.000000 mailchimp3-3.0.9/mailchimp3/entities/reportdomainperformance.py
+-rw-r--r--   0 charlesthk   (501) staff       (20)    24070 2019-09-10 06:34:47.000000 mailchimp3-3.0.9/README.rst
```

### Comparing `mailchimp3-3.0.7/PKG-INFO` & `mailchimp3-3.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: mailchimp3
-Version: 3.0.7
+Version: 3.0.9
 Summary: A python client for v3 of MailChimp API
 Home-page: https://github.com/charlesthk/python-mailchimp
 Author: Charles TISSIER
 Author-email: charles@vingtcinq.io
 License: MIT
-Description: |mailchimp3 v3.0.7 on PyPi| |MIT license| |Stable|
+Description: |mailchimp3 v3.0.9 on PyPi| |MIT license| |Stable|
         
         python-mailchimp-api
         ====================
         
         A straighforward python client for v3 of MailChimp API using requests >=
         2.7.0.
         
@@ -56,17 +56,17 @@
         
         Grab ``YOUR_API_KEY`` from your mailchimp account (Account > Extra > Api
         Keys). ``YOUR_USERNAME`` is the one you use to login on the website and
         is optional.
         
         ::
         
-            from mailchimp3 import MailChimp
+           from mailchimp3 import MailChimp
         
-            client = MailChimp(mc_api='YOUR_API_KEY', mc_user='YOUR_USERNAME')
+           client = MailChimp(mc_api='YOUR_API_KEY', mc_user='YOUR_USERNAME')
         
         OAuth Support
         ~~~~~~~~~~~~~
         
         In addition to HTTP Basic Authentication, MailChimp supports
         authentication through OAuth2. Information on obtaining the proper
         access key can be found
@@ -80,160 +80,162 @@
         skip. For endpoints that allow the pagination parameters, the all()
         method has an additional boolean ``get_all`` argument that will loop
         through all records until the API no longer returns any to get all
         records without manually performing an additional query. By default,
         count is 10 and offset is 0 for all endpoints that support it. The
         ``get_all`` parameter on the all() method on any endpoint defaults to
         false, which follows the values that are provided in the call, and using
-        ``get_all=True`` will ignore the provided count and offset to ensure
-        that all records are returned. When using get_all, the count will be
-        5000, to fetch large numbers of records without flooding the system with
-        requests. The large size of count should not impact calls which are
+        ``get_all=True`` will ignore the provided offset to ensure that all
+        records are returned. When using get_all, the count will be 500 unless
+        otherwise specified. It is strongly recommended to avoid small values
+        for ``count`` to fetch large numbers of records because this will flood
+        the system. A large ``count`` size should not impact calls which are
         expected to return a very small number of records, and should improve
-        performance for calls where fetching 5000 records would only provide a
+        performance for calls where fetching 500 records would only provide a
         fraction by preventing the delay of making a huge number of requests.
         
         ::
         
-            client.lists.members.all('123456', count=100, offset=0)
+           client.lists.members.all('123456', count=100, offset=0)
         
         Fields
         ~~~~~~
         
         Many endpoints allow you to select which fields will be returned out of
         all available fields (for example, only the email_address of a member).
         Simply add ``fields`` arguments in your function. The following only
         display email_address and id for each member in list 123456:
         
         ::
         
-            client.lists.members.all('123456', get_all=True, fields="members.email_address,members.id")
+           client.lists.members.all('123456', get_all=True, fields="members.email_address,members.id")
         
         Examples
         ~~~~~~~~
         
         ::
         
-            # returns all the lists (only name and id)
-            client.lists.all(get_all=True, fields="lists.name,lists.id")
+           # returns all the lists (only name and id)
+           client.lists.all(get_all=True, fields="lists.name,lists.id")
         
-            # returns all members inside list '123456'
-            client.lists.members.all('123456', get_all=True)
+           # returns all members inside list '123456'
+           client.lists.members.all('123456', get_all=True)
         
-            # return the first 100 member's email addresses for the list with id 123456
-            client.lists.members.all('123456', count=100, offset=0, fields="members.email_address")
+           # return the first 100 member's email addresses for the list with id 123456
+           client.lists.members.all('123456', count=100, offset=0, fields="members.email_address")
         
-            # returns the list matching id '123456'
-            client.lists.get('123456')
-        
-            # add John Doe with email john.doe@example.com to list matching id '123456'
-            client.lists.members.create('123456', {
-                'email_address': 'john.doe@example.com',
-                'status': 'subscribed',
-                'merge_fields': {
-                    'FNAME': 'John',
-                    'LNAME': 'Doe',
-                },
-            })
-        
-            # returns all the campaigns
-            client.campaigns.all(get_all=True)
-        
-            # You can also disable at runtime with the optional ``enabled`` parameter.
-            # Every API call will return None
-            client = MailChimp('YOUR SECRET KEY', enabled=False)
-        
-            # You are encouraged to specify a value in seconds for the ``timeout``
-            # parameter to avoid hanging requests.
-            client = MailChimp('YOUR SECRET KEY', timeout=10.0)
-        
-            # You are encouraged to specify a User-Agent for requests to the MailChimp
-            # API. Headers can be specified using the ``request_headers`` parameter.
-            headers = requests.utils.default_headers()
-            headers['User-Agent'] = 'Example (example@example.com)'
-            client = MailChimp('YOUR SECRET KEY', request_headers=headers)
+           # returns the list matching id '123456'
+           client.lists.get('123456')
+        
+           # add John Doe with email john.doe@example.com to list matching id '123456'
+           client.lists.members.create('123456', {
+               'email_address': 'john.doe@example.com',
+               'status': 'subscribed',
+               'merge_fields': {
+                   'FNAME': 'John',
+                   'LNAME': 'Doe',
+               },
+           })
+        
+           # returns all the campaigns
+           client.campaigns.all(get_all=True)
+        
+           # You can also disable at runtime with the optional ``enabled`` parameter.
+           # Every API call will return None
+           client = MailChimp('YOUR SECRET KEY', enabled=False)
+        
+           # You are encouraged to specify a value in seconds for the ``timeout``
+           # parameter to avoid hanging requests.
+           client = MailChimp('YOUR SECRET KEY', timeout=10.0)
+        
+           # You are encouraged to specify a User-Agent for requests to the MailChimp
+           # API. Headers can be specified using the ``request_headers`` parameter.
+           headers = requests.utils.default_headers()
+           headers['User-Agent'] = 'Example (example@example.com)'
+           client = MailChimp('YOUR SECRET KEY', request_headers=headers)
         
         API Structure
         -------------
         
         All endpoints follow the structure listed in the official MailChimp API
         v3 documentation. The structure will be listed below and then the
         individual methods available after.
         
         ::
         
-            MailChimp
-            +- Root
-            +- Authorized Apps
-            +- Automations
-            |  +- Actions
-            |  +- Emails
-            |  |  +- Actions
-            |  |  +- Queues
-            |  +- Removed Subscribers
-            +- Batch Operations
-            +- Batch Webhooks
-            +- Campaign Folders
-            +- Campaigns
-            |  +- Actions
-            |  +- Content
-            |  +- Feedback
-            |  +- Send Checklist
-            +- Conversations
-            |  +- Messages
-            +- Stores
-            |  +- Carts
-            |  |  +- Lines
-            |  +- Customers
-            |  +- Orders
-            |  |  +- Lines
-            |  +- Products
-            |     +- Images
-            |     +- Variants
-            |  +- Promo Rules
-            |     +- Promo Codes
-            +- File Manager Files
-            +- File Manager Folders
-            +- Lists
-            |  +- Abuse Reports
-            |  +- Activity
-            |  +- Clients
-            |  +- Growth History
-            |  +- Interest Categories
-            |  |  +- Interests
-            |  +- Members
-            |  |  +- Activity
-            |  |  +- Goals
-            |  |  +- Notes
-            |  +- Merge Fields
-            |  +- Segments
-            |  |  +- Segment Members
-            |  +- Signup Forms
-            |  +- Twitter Lead Generation Carts
-            |  +- Webhooks
-            +- Ping
-            +- Reports
-            |  +- Campaign Abuse
-            |  +- Campaign Advice
-            |  +- Campaign Open reports
-            |  +- Click Reports
-            |  |  +- Members
-            |  +- Domain Performance
-            |  +- EepURL Reports
-            |  +- Email Activity
-            |  +- Google Analytics
-            |  +- Location
-            |  +- Sent To
-            |  +- Sub-Reports
-            |  +- Unsubscribes
-            +- Seach Campaigns
-            +- Search Members
-            +- Template Folders
-            +- Templates
-               +- Default Content
+           MailChimp
+           +- Root
+           +- Authorized Apps
+           +- Automations
+           |  +- Actions
+           |  +- Emails
+           |  |  +- Actions
+           |  |  +- Queues
+           |  +- Removed Subscribers
+           +- Batch Operations
+           +- Batch Webhooks
+           +- Campaign Folders
+           +- Campaigns
+           |  +- Actions
+           |  +- Content
+           |  +- Feedback
+           |  +- Send Checklist
+           +- Conversations
+           |  +- Messages
+           +- Stores
+           |  +- Carts
+           |  |  +- Lines
+           |  +- Customers
+           |  +- Orders
+           |  |  +- Lines
+           |  +- Products
+           |     +- Images
+           |     +- Variants
+           |  +- Promo Rules
+           |     +- Promo Codes
+           +- File Manager Files
+           +- File Manager Folders
+           +- Lists
+           |  +- Abuse Reports
+           |  +- Activity
+           |  +- Clients
+           |  +- Growth History
+           |  +- Interest Categories
+           |  |  +- Interests
+           |  +- Members
+           |  |  +- Activity
+           |  |  +- Goals
+           |  |  +- Notes
+           |  |  +- Tags
+           |  +- Merge Fields
+           |  +- Segments
+           |  |  +- Segment Members
+           |  +- Signup Forms
+           |  +- Twitter Lead Generation Carts
+           |  +- Webhooks
+           +- Ping
+           +- Reports
+           |  +- Campaign Abuse
+           |  +- Campaign Advice
+           |  +- Campaign Open reports
+           |  +- Click Reports
+           |  |  +- Members
+           |  +- Domain Performance
+           |  +- EepURL Reports
+           |  +- Email Activity
+           |  +- Google Analytics
+           |  +- Location
+           |  +- Sent To
+           |  +- Sub-Reports
+           |  +- Unsubscribes
+           +- Seach Campaigns
+           +- Search Members
+           +- Template Folders
+           +- Templates
+              +- Default Content
         
         API Endpoints
         -------------
         
         Below is the list of all endpoints and the methods that can be called
         against them. Any endpoint that has a method that takes an ID argument
         (for example the app_id in the authorized_apps endpoint or the
@@ -252,682 +254,690 @@
         .. _root-1:
         
         Root
         ^^^^
         
         ::
         
-            client.root.get()
+           client.root.get()
         
         Authorized Apps
         ~~~~~~~~~~~~~~~
         
         .. _authorized-apps-1:
         
         Authorized Apps
         ^^^^^^^^^^^^^^^
         
         ::
         
-            client.authorized_apps.create(data={})
-            client.authorized_apps.all(get_all=False)
-            client.authorized_apps.get(app_id='')
+           client.authorized_apps.create(data={})
+           client.authorized_apps.all(get_all=False)
+           client.authorized_apps.get(app_id='')
         
         Automations
         ~~~~~~~~~~~
         
         .. _automations-1:
         
         Automations
         ^^^^^^^^^^^
         
         ::
         
-            client.automations.all(get_all=False)
-            client.automations.get(workflow_id='')
+           client.automations.all(get_all=False)
+           client.automations.get(workflow_id='')
         
         Automation Actions
         ^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.automations.actions.pause(workflow_id='')
-            client.automations.actions.start(workflow_id='')
+           client.automations.actions.pause(workflow_id='')
+           client.automations.actions.start(workflow_id='')
         
         Automation Emails
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.automations.emails.all(workflow_id='')
-            client.automations.emails.get(workflow_id='', email_id='')
+           client.automations.emails.all(workflow_id='')
+           client.automations.emails.get(workflow_id='', email_id='')
         
         Automation Email Actions
         ^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.automations.emails.actions.pause(workflow_id='', email_id='')
-            client.automations.emails.actions.start(workflow_id='', email_id='')
+           client.automations.emails.actions.pause(workflow_id='', email_id='')
+           client.automations.emails.actions.start(workflow_id='', email_id='')
         
         Automation Email Queues
         ^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.automations.emails.queues.create(workflow_id='', email_id='', data={})
-            client.automations.emails.queues.all(workflow_id='', email_id='')
-            client.automations.emails.queues.get(workflow_id='', email_id='', subscriber_hash='')
+           client.automations.emails.queues.create(workflow_id='', email_id='', data={})
+           client.automations.emails.queues.all(workflow_id='', email_id='')
+           client.automations.emails.queues.get(workflow_id='', email_id='', subscriber_hash='')
         
         Automation Removed Subscribers
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.automations.removed_subscribers.create(workflow_id='', data={})
-            client.automations.removed_subscribers.all(workflow_id='')
+           client.automations.removed_subscribers.create(workflow_id='', data={})
+           client.automations.removed_subscribers.all(workflow_id='')
         
         Batch Operations
         ~~~~~~~~~~~~~~~~
         
         .. _batch-operations-1:
         
         Batch Operations
         ^^^^^^^^^^^^^^^^
         
         ::
         
-            client.batch_operations.create(data={})
-            client.batch_operations.all(get_all=False)
-            client.batch_operations.get(batch_id='')
-            client.batch_operations.delete(batch_id='')
+           client.batch_operations.create(data={})
+           client.batch_operations.all(get_all=False)
+           client.batch_operations.get(batch_id='')
+           client.batch_operations.delete(batch_id='')
         
         Batch Webhooks
         ~~~~~~~~~~~~~~
         
         .. _batch-webhooks-1:
         
         Batch Webhooks
         ^^^^^^^^^^^^^^
         
         ::
         
-            client.batch_webhooks.create(data={})
-            client.batch_webhooks.all(get_all=False)
-            client.batch_webhooks.get(batch_webhook_id='')
-            client.batch_webhooks.update(batch_webhook_id='', data={})
-            client.batch_webhooks.delete(batch_webhook_id='')
+           client.batch_webhooks.create(data={})
+           client.batch_webhooks.all(get_all=False)
+           client.batch_webhooks.get(batch_webhook_id='')
+           client.batch_webhooks.update(batch_webhook_id='', data={})
+           client.batch_webhooks.delete(batch_webhook_id='')
         
         Campaigns
         ~~~~~~~~~
         
         Folders
         ^^^^^^^
         
         ::
         
-            client.campaign_folders.create(data={})
-            client.campaign_folders.all(get_all=False)
-            client.campaign_folders.get(folder_id='')
-            client.campaign_folders.update(folder_id='', data={})
-            client.campaign_folders.delete(folder_id='')
+           client.campaign_folders.create(data={})
+           client.campaign_folders.all(get_all=False)
+           client.campaign_folders.get(folder_id='')
+           client.campaign_folders.update(folder_id='', data={})
+           client.campaign_folders.delete(folder_id='')
         
         .. _campaigns-1:
         
         Campaigns
         ^^^^^^^^^
         
         ::
         
-            client.campaigns.create(data={})
-            client.campaigns.all(get_all=False)
-            client.campaigns.get(campaign_id='')
-            client.campaigns.update(campaign_id='')
-            client.campaigns.delete(campaign_id='')
+           client.campaigns.create(data={})
+           client.campaigns.all(get_all=False)
+           client.campaigns.get(campaign_id='')
+           client.campaigns.update(campaign_id='')
+           client.campaigns.delete(campaign_id='')
         
         Campaign Actions
         ^^^^^^^^^^^^^^^^
         
         ::
         
-            client.campaigns.actions.cancel(campaign_id='')
-            client.campaigns.actions.pause(campaign_id='')
-            client.campaigns.actions.replicate(campaign_id='')
-            client.campaigns.actions.resume(campaign_id='')
-            client.campaigns.actions.schedule(campaign_id='', data={})
-            client.campaigns.actions.send(campaign_id='')
-            client.campaigns.actions.test(campaign_id='', data={})
-            client.campaigns.actions.unschedule(campaign_id='')
+           client.campaigns.actions.cancel(campaign_id='')
+           client.campaigns.actions.pause(campaign_id='')
+           client.campaigns.actions.replicate(campaign_id='')
+           client.campaigns.actions.resume(campaign_id='')
+           client.campaigns.actions.schedule(campaign_id='', data={})
+           client.campaigns.actions.send(campaign_id='')
+           client.campaigns.actions.test(campaign_id='', data={})
+           client.campaigns.actions.unschedule(campaign_id='')
         
         Campaign Content
         ^^^^^^^^^^^^^^^^
         
         ::
         
-            client.campaigns.content.get(campaign_id='')
-            client.campaigns.content.update(campaign_id='', data={})
+           client.campaigns.content.get(campaign_id='')
+           client.campaigns.content.update(campaign_id='', data={})
         
         Campaign Feedback
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.campaigns.feedback.create(campaign_id='', data={})
-            client.campaigns.feedback.all(campaign_id='', get_all=False)
-            client.campaigns.feedback.get(campaign_id='', feedback_id='')
-            client.campaigns.feedback.update(campaign_id='', feedback_id='', data={})
-            client.campaigns.feedback.delete(campaign_id='', feedback_id='')
+           client.campaigns.feedback.create(campaign_id='', data={})
+           client.campaigns.feedback.all(campaign_id='', get_all=False)
+           client.campaigns.feedback.get(campaign_id='', feedback_id='')
+           client.campaigns.feedback.update(campaign_id='', feedback_id='', data={})
+           client.campaigns.feedback.delete(campaign_id='', feedback_id='')
         
         Campaign Send Checklist
         ^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.campaigns.send_checklist.get(campaign_id='')
+           client.campaigns.send_checklist.get(campaign_id='')
         
         Conversations
         ~~~~~~~~~~~~~
         
         .. _conversations-1:
         
         Conversations
         ^^^^^^^^^^^^^
         
         ::
         
-            client.conversations.all(get_all=False)
-            client.conversations.get(conversation_id='')
+           client.conversations.all(get_all=False)
+           client.conversations.get(conversation_id='')
         
         Conversation Messages
         ^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.conversations.messages.create(conversation_id='', data={})
-            client.conversations.messages.all(conversation_id='')
-            client.conversations.messages.get(conversation_id='', message_id='')
+           client.conversations.messages.create(conversation_id='', data={})
+           client.conversations.messages.all(conversation_id='')
+           client.conversations.messages.get(conversation_id='', message_id='')
         
         E-Commerce
         ~~~~~~~~~~
         
         Stores
         ^^^^^^
         
         ::
         
-            client.stores.create(data={})
-            client.stores.all(get_all=False)
-            client.stores.get(store_id='')
-            client.stores.update(store_id='', data={})
-            client.stores.delete(store_id='')
+           client.stores.create(data={})
+           client.stores.all(get_all=False)
+           client.stores.get(store_id='')
+           client.stores.update(store_id='', data={})
+           client.stores.delete(store_id='')
         
         Store Carts
         ^^^^^^^^^^^
         
         ::
         
-            client.stores.carts.create(store_id='', data={})
-            client.stores.carts.all(store_id='', get_all=False)
-            client.stores.carts.get(store_id='', cart_id='')
-            client.stores.carts.update(store_id='', cart_id='', data={})
-            client.stores.carts.delete(store_id='', cart_id='')
+           client.stores.carts.create(store_id='', data={})
+           client.stores.carts.all(store_id='', get_all=False)
+           client.stores.carts.get(store_id='', cart_id='')
+           client.stores.carts.update(store_id='', cart_id='', data={})
+           client.stores.carts.delete(store_id='', cart_id='')
         
         Store Cart Lines
         ^^^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.carts.lines.create(store_id='', cart_id='', data={})
-            client.stores.carts.lines.all(store_id='', cart_id='', get_all=False)
-            client.stores.carts.lines.get(store_id='', cart_id='', line_id='')
-            client.stores.carts.lines.update(store_id='', cart_id='', line_id='', data={})
-            client.stores.carts.lines.delete(store_id='', cart_id='', line_id='')
+           client.stores.carts.lines.create(store_id='', cart_id='', data={})
+           client.stores.carts.lines.all(store_id='', cart_id='', get_all=False)
+           client.stores.carts.lines.get(store_id='', cart_id='', line_id='')
+           client.stores.carts.lines.update(store_id='', cart_id='', line_id='', data={})
+           client.stores.carts.lines.delete(store_id='', cart_id='', line_id='')
         
         Store Customers
         ^^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.customers.create(store_id='', data={})
-            client.stores.customers.all(store_id='', get_all=False)
-            client.stores.customers.get(store_id='', customer_id='')
-            client.stores.customers.update(store_id='', customer_id='', data={})
-            client.stores.customers.create_or_update(store_id='', customer_id='', data={})
-            client.stores.customers.delete(store_id='', customer_id='')
+           client.stores.customers.create(store_id='', data={})
+           client.stores.customers.all(store_id='', get_all=False)
+           client.stores.customers.get(store_id='', customer_id='')
+           client.stores.customers.update(store_id='', customer_id='', data={})
+           client.stores.customers.create_or_update(store_id='', customer_id='', data={})
+           client.stores.customers.delete(store_id='', customer_id='')
         
         Store Orders
         ^^^^^^^^^^^^
         
         ::
         
-            client.stores.orders.create(store_id='', data={})
-            client.stores.orders.all(store_id='', get_all=False)
-            client.stores.orders.get(store_id='', order_id='')
-            client.stores.orders.update(store_id='', order_id='', data={})
-            client.stores.orders.delete(store_id='', order_id='')
+           client.stores.orders.create(store_id='', data={})
+           client.stores.orders.all(store_id='', get_all=False)
+           client.stores.orders.get(store_id='', order_id='')
+           client.stores.orders.update(store_id='', order_id='', data={})
+           client.stores.orders.delete(store_id='', order_id='')
         
         Store Order Lines
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.orders.lines.create(store_id='', order_id='', data={})
-            client.stores.orders.lines.all(store_id='', order_id='', get_all=False)
-            client.stores.orders.lines.get(store_id='', order_id='', line_id='')
-            client.stores.orders.lines.update(store_id='', order_id='', line_id='', data={})
-            client.stores.orders.lines.delete(store_id='', order_id='', line_id='')
+           client.stores.orders.lines.create(store_id='', order_id='', data={})
+           client.stores.orders.lines.all(store_id='', order_id='', get_all=False)
+           client.stores.orders.lines.get(store_id='', order_id='', line_id='')
+           client.stores.orders.lines.update(store_id='', order_id='', line_id='', data={})
+           client.stores.orders.lines.delete(store_id='', order_id='', line_id='')
         
         Store Products
         ^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.products.create(store_id='', data={})
-            client.stores.products.all(store_id='', get_all=False)
-            client.stores.products.get(store_id='', product_id='')
-            client.stores.products.update(store_id='', product_id='')
-            client.stores.products.delete(store_id='', product_id='')
+           client.stores.products.create(store_id='', data={})
+           client.stores.products.all(store_id='', get_all=False)
+           client.stores.products.get(store_id='', product_id='')
+           client.stores.products.update(store_id='', product_id='')
+           client.stores.products.delete(store_id='', product_id='')
         
         Store Product Images
         ^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.products.images.create(store_id='', product_id='', data={})
-            client.stores.products.images.all(store_id='', product_id='', get_all=False)
-            client.stores.products.images.get(store_id='', product_id='', image_id='')
-            client.stores.products.images.update(store_id='', product_id='', image_id='', data={})
-            client.stores.products.images.delete(store_id='', product_id='', image_id='')
+           client.stores.products.images.create(store_id='', product_id='', data={})
+           client.stores.products.images.all(store_id='', product_id='', get_all=False)
+           client.stores.products.images.get(store_id='', product_id='', image_id='')
+           client.stores.products.images.update(store_id='', product_id='', image_id='', data={})
+           client.stores.products.images.delete(store_id='', product_id='', image_id='')
         
         Store Product Variants
         ^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.products.variants.create(store_id='', product_id='', data={})
-            client.stores.products.variants.all(store_id='', product_id='', get_all=False)
-            client.stores.products.variants.get(store_id='', product_id='', variant_id='')
-            client.stores.products.variants.update(store_id='', product_id='', variant_id='', data={})
-            client.stores.products.variants.create_or_update(store_id='', product_id='', variant_id='', data={})
-            client.stores.products.variants.delete(store_id='', product_id='', variant_id='')
+           client.stores.products.variants.create(store_id='', product_id='', data={})
+           client.stores.products.variants.all(store_id='', product_id='', get_all=False)
+           client.stores.products.variants.get(store_id='', product_id='', variant_id='')
+           client.stores.products.variants.update(store_id='', product_id='', variant_id='', data={})
+           client.stores.products.variants.create_or_update(store_id='', product_id='', variant_id='', data={})
+           client.stores.products.variants.delete(store_id='', product_id='', variant_id='')
         
         File Manager
         ~~~~~~~~~~~~
         
         Files
         ^^^^^
         
         ::
         
-            client.files.create(data={})
-            client.files.all(get_all=False)
-            client.files.get(file_id='')
-            client.files.update(file_id='', data={})
-            client.files.delete(file_id='')
+           client.files.create(data={})
+           client.files.all(get_all=False)
+           client.files.get(file_id='')
+           client.files.update(file_id='', data={})
+           client.files.delete(file_id='')
         
         .. _folders-1:
         
         Folders
         ^^^^^^^
         
         ::
         
-            client.folders.create(data={})
-            client.folders.all(get_all=False)
-            client.folders.get(folder_id='')
-            client.folders.update(folder_id='', data={})
-            client.folders.delete(folder_id='')
+           client.folders.create(data={})
+           client.folders.all(get_all=False)
+           client.folders.get(folder_id='')
+           client.folders.update(folder_id='', data={})
+           client.folders.delete(folder_id='')
         
         Lists
         ~~~~~
         
         .. _lists-1:
         
         Lists
         ^^^^^
         
         ::
         
-            client.lists.create(data={})
-            client.lists.update_members(list_id='', data={})
-            client.lists.all(get_all=False)
-            client.lists.get(list_id='')
-            client.lists.update(list_id='', data={})
-            client.lists.delete(list_id='')
+           client.lists.create(data={})
+           client.lists.update_members(list_id='', data={})
+           client.lists.all(get_all=False)
+           client.lists.get(list_id='')
+           client.lists.update(list_id='', data={})
+           client.lists.delete(list_id='')
         
         List Abuse Reports
         ^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.abuse_reports.all(list_id='', get_all=False)
-            client.lists.abuse_reports.get(list_id='', report_id='')
+           client.lists.abuse_reports.all(list_id='', get_all=False)
+           client.lists.abuse_reports.get(list_id='', report_id='')
         
         List Activity
         ^^^^^^^^^^^^^
         
         ::
         
-            client.lists.activity.all(list_id='')
+           client.lists.activity.all(list_id='')
         
         List Clients
         ^^^^^^^^^^^^
         
         ::
         
-            client.lists.clients.all(list_id='')
+           client.lists.clients.all(list_id='')
         
         List Growth History
         ^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.growth_history.all(list_id='', get_all=False)
-            client.lists.growth_history.get(list_id='', month='')
+           client.lists.growth_history.all(list_id='', get_all=False)
+           client.lists.growth_history.get(list_id='', month='')
         
         List Interest Categories
         ^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.interest_categories.create(list_id='', data={})
-            client.lists.interest_categories.all(list_id='', get_all=False)
-            client.lists.interest_categories.get(list_id='', category_id='')
-            client.lists.interest_categories.update(list_id='', category_id='', data={})
-            client.lists.interest_categories.delete(list_id='', category_id='')
+           client.lists.interest_categories.create(list_id='', data={})
+           client.lists.interest_categories.all(list_id='', get_all=False)
+           client.lists.interest_categories.get(list_id='', category_id='')
+           client.lists.interest_categories.update(list_id='', category_id='', data={})
+           client.lists.interest_categories.delete(list_id='', category_id='')
         
         List Interest Category Interests
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.interest_categories.interests.create(list_id='', category_id='', data={})
-            client.lists.interest_categories.interests.all(list_id='', category_id='', get_all=False)
-            client.lists.interest_categories.interests.get(list_id='', category_id='', interest_id='')
-            client.lists.interest_categories.interests.update(list_id='', category_id='', interest_id='', data={})
-            client.lists.interest_categories.interests.delete(list_id='', category_id='', interest_id='')
+           client.lists.interest_categories.interests.create(list_id='', category_id='', data={})
+           client.lists.interest_categories.interests.all(list_id='', category_id='', get_all=False)
+           client.lists.interest_categories.interests.get(list_id='', category_id='', interest_id='')
+           client.lists.interest_categories.interests.update(list_id='', category_id='', interest_id='', data={})
+           client.lists.interest_categories.interests.delete(list_id='', category_id='', interest_id='')
         
         List Members
         ^^^^^^^^^^^^
         
         ::
         
-            client.lists.members.create(list_id='', data={})
-            client.lists.members.all(list_id='', get_all=False)
-            client.lists.members.get(list_id='', subscriber_hash='')
-            client.lists.members.update(list_id='', subscriber_hash='', data={})
-            client.lists.members.create_or_update(list_id='', subscriber_hash='', data={})
-            client.lists.members.delete(list_id='', subscriber_hash='')
-            client.lists.members.delete_permanent(list_id='', subscriber_hash='')
+           client.lists.members.create(list_id='', data={})
+           client.lists.members.all(list_id='', get_all=False)
+           client.lists.members.get(list_id='', subscriber_hash='')
+           client.lists.members.update(list_id='', subscriber_hash='', data={})
+           client.lists.members.create_or_update(list_id='', subscriber_hash='', data={})
+           client.lists.members.delete(list_id='', subscriber_hash='')
+           client.lists.members.delete_permanent(list_id='', subscriber_hash='')
         
         List Member Activity
         ^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.members.activity.all(list_id='', subscriber_hash='')
+           client.lists.members.activity.all(list_id='', subscriber_hash='')
         
         List Member Goals
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.members.goals.all(list_id='', subscriber_hash='')
+           client.lists.members.goals.all(list_id='', subscriber_hash='')
         
         List Member Notes
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.members.notes.create(list_id='', subscriber_hash='', data={})
-            client.lists.members.notes.all(list_id='', subscriber_hash='', get_all=False)
-            client.lists.members.notes.get(list_id='', subscriber_hash='', note_id='')
-            client.lists.members.notes.update(list_id='', subscriber_hash='', note_id='', data={})
-            client.lists.members.notes.delete(list_id='', subscriber_hash='', note_id='')
+           client.lists.members.notes.create(list_id='', subscriber_hash='', data={})
+           client.lists.members.notes.all(list_id='', subscriber_hash='', get_all=False)
+           client.lists.members.notes.get(list_id='', subscriber_hash='', note_id='')
+           client.lists.members.notes.update(list_id='', subscriber_hash='', note_id='', data={})
+           client.lists.members.notes.delete(list_id='', subscriber_hash='', note_id='')
+        
+        List Member Tags
+        ^^^^^^^^^^^^^^^^
+        
+        ::
+        
+           client.lists.members.tags.update(list_id='', subscriber_hash='', data={})
+           client.lists.members.tags.all(list_id='', subscriber_hash='')
         
         List Merge Fields
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.merge_fields.create(list_id='', data={})
-            client.lists.merge_fields.all(list_id='', get_all=False)
-            client.lists.merge_fields.get(list_id='', merge_id='')
-            client.lists.merge_fields.update(list_id='', merge_id='', data={})
-            client.lists.merge_fields.delete(list_id='', merge_id='')
+           client.lists.merge_fields.create(list_id='', data={})
+           client.lists.merge_fields.all(list_id='', get_all=False)
+           client.lists.merge_fields.get(list_id='', merge_id='')
+           client.lists.merge_fields.update(list_id='', merge_id='', data={})
+           client.lists.merge_fields.delete(list_id='', merge_id='')
         
         List Segments
         ^^^^^^^^^^^^^
         
         ::
         
-            client.lists.segments.create(list_id='', data={})
-            client.lists.segments.all(list_id='', get_all=False)
-            client.lists.segments.get(list_id='', segment_id='')
-            client.lists.segments.update(list_id='', segment_id='', data={})
-            client.lists.segments.update_members(list_id='', segment_id='', data={})
-            client.lists.segments.delete(list_id='', segment_id='')
+           client.lists.segments.create(list_id='', data={})
+           client.lists.segments.all(list_id='', get_all=False)
+           client.lists.segments.get(list_id='', segment_id='')
+           client.lists.segments.update(list_id='', segment_id='', data={})
+           client.lists.segments.update_members(list_id='', segment_id='', data={})
+           client.lists.segments.delete(list_id='', segment_id='')
         
         List Segment Members
         ^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.segments.members.create(list_id='', segment_id='', data={})
-            client.lists.segments.members.all(list_id='', segment_id='', get_all=False)
-            client.lists.segments.members.delete(list_id='', segment_id='', subscriber_hash='')
+           client.lists.segments.members.create(list_id='', segment_id='', data={})
+           client.lists.segments.members.all(list_id='', segment_id='', get_all=False)
+           client.lists.segments.members.delete(list_id='', segment_id='', subscriber_hash='')
         
         List Signup Forms
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.signup_forms.create(list_id='', data={})
-            client.lists.signup_forms.all(list_id='')
+           client.lists.signup_forms.create(list_id='', data={})
+           client.lists.signup_forms.all(list_id='')
         
         List Webhooks
         ^^^^^^^^^^^^^
         
         ::
         
-            client.lists.webhooks.create(list_id='', data={})
-            client.lists.webhooks.all(list_id='')
-            client.lists.webhooks.get(list_id='', webhook_id='')
-            client.lists.webhooks.update(list_id='', webhook_id='', data={})
-            client.lists.webhooks.delete(list_id='', webhook_id='')
+           client.lists.webhooks.create(list_id='', data={})
+           client.lists.webhooks.all(list_id='')
+           client.lists.webhooks.get(list_id='', webhook_id='')
+           client.lists.webhooks.update(list_id='', webhook_id='', data={})
+           client.lists.webhooks.delete(list_id='', webhook_id='')
         
         Reports
         ~~~~~~~
         
         .. _reports-1:
         
         Reports
         ^^^^^^^
         
         ::
         
-            client.reports.all(get_all=False)
-            client.reports.get(campaign_id='')
+           client.reports.all(get_all=False)
+           client.reports.get(campaign_id='')
         
         Campaign Abuse Reports
         ^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.abuse_reports.all(campaign_id='')
-            client.reports.abuse_reports.get(campaign_id='', report_id='')
+           client.reports.abuse_reports.all(campaign_id='')
+           client.reports.abuse_reports.get(campaign_id='', report_id='')
         
         Campaign Advice
         ^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.advice.all(campaign_id='')
+           client.reports.advice.all(campaign_id='')
         
         Click Details Report
         ^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.click_details.all(campaign_id='', get_all=False)
-            client.reports.click_details.get(campaign_id='', link_id='')
+           client.reports.click_details.all(campaign_id='', get_all=False)
+           client.reports.click_details.get(campaign_id='', link_id='')
         
         Click Details Report Members
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.click_details.members.all(campaign_id='', link_id='', get_all=False)
-            client.reports.click_details.members.get(campaign_id='', link_id='', subscriber_hash='')
+           client.reports.click_details.members.all(campaign_id='', link_id='', get_all=False)
+           client.reports.click_details.members.get(campaign_id='', link_id='', subscriber_hash='')
         
         Domain Performance Reports
         ^^^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.domain_performance.all(campaign_id='')
+           client.reports.domain_performance.all(campaign_id='')
         
         EepURL Reports
         ^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.eepurl.all(camnpaign_id='')
+           client.reports.eepurl.all(camnpaign_id='')
         
         Email Activity Reports
         ^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.email_activity.all(campaign_id='', get_all=False)
-            client.reports.email_activity.get(campaign_id='', subscriber_hash='')
+           client.reports.email_activity.all(campaign_id='', get_all=False)
+           client.reports.email_activity.get(campaign_id='', subscriber_hash='')
         
         Locations Report
         ^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.locations.all(campaign_id='', get_all=False)
+           client.reports.locations.all(campaign_id='', get_all=False)
         
         Sent To Reports
         ^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.sent_to.all(campaign_id='', get_all=False)
-            client.reports.sent_to.get(campaign_id='', subscriber_hash='')
+           client.reports.sent_to.all(campaign_id='', get_all=False)
+           client.reports.sent_to.get(campaign_id='', subscriber_hash='')
         
         Sub-Reports
         ^^^^^^^^^^^
         
         ::
         
-            client.reports.subreports.all(campaign_id='')
+           client.reports.subreports.all(campaign_id='')
         
         Unsubscribes
         ^^^^^^^^^^^^
         
         ::
         
-            client.reports.unsubscribes.all(campaign_id='', get_all=False)
-            client.reports.unsubscribes.get(campaign_id='', subscriber_hash='')
+           client.reports.unsubscribes.all(campaign_id='', get_all=False)
+           client.reports.unsubscribes.get(campaign_id='', subscriber_hash='')
         
         Search
         ~~~~~~
         
         .. _campaigns-2:
         
         Campaigns
         ^^^^^^^^^
         
         ::
         
-            client.search_campaigns.get()
+           client.search_campaigns.get()
         
         Members
         ^^^^^^^
         
         ::
         
-            client.search_members.get()
+           client.search_members.get()
         
         Templates
         ~~~~~~~~~
         
         .. _folders-2:
         
         Folders
         ^^^^^^^
         
         ::
         
-            client.template_folders.create(data={})
-            client.template_folders.all(get_all=False)
-            client.template_folders.get(folder_id='')
-            client.template_folders.update(folder_id='', data={})
-            client.template_folders.delete(folder_id='')
+           client.template_folders.create(data={})
+           client.template_folders.all(get_all=False)
+           client.template_folders.get(folder_id='')
+           client.template_folders.update(folder_id='', data={})
+           client.template_folders.delete(folder_id='')
         
         .. _templates-1:
         
         Templates
         ^^^^^^^^^
         
         ::
         
-            client.templates.create(data={})
-            client.templates.all(get_all=False)
-            client.templates.get(template_id='')
-            client.templates.update(template_id='', data={})
-            client.templates.delete(template_id='')
+           client.templates.create(data={})
+           client.templates.all(get_all=False)
+           client.templates.get(template_id='')
+           client.templates.update(template_id='', data={})
+           client.templates.delete(template_id='')
         
         Default Content
         ^^^^^^^^^^^^^^^
         
         ::
         
-            client.templates.default_content.all(template_id='')
+           client.templates.default_content.all(template_id='')
         
         Logging
         -------
         
         The MailChimp client will log request/response detail into the
         mailchimp3.client logging namespace. Consider the following snippet to
         get started with logging:
         
         .. code:: python
         
-            import logging
-            fh = logging.FileHandler('/path/to/some/log.log')
-            logger = logging.getLogger('mailchimp3.client')
-            logger.addHandler(fh)
+           import logging
+           fh = logging.FileHandler('/path/to/some/log.log')
+           logger = logging.getLogger('mailchimp3.client')
+           logger.addHandler(fh)
         
-            # use the client normally
-            client.lists.all(**{'fields': 'lists.date_created'})
+           # use the client normally
+           client.lists.all(**{'fields': 'lists.date_created'})
         
         request/response detail will be appended into /path/to/some/log.log:
         
         ::
         
-            GET Request: https://us15.api.mailchimp.com/3.0/lists?fields=lists.date_created
-            GET Response: 200 {"lists":[{"date_created":"2017-05-10T13:53:05+00:00"},{"date_created":"2017-08-22T20:27:56+00:00"},{"date_created":"2017-05-12T21:22:15+00:00"},{"date_created":"2017-04-27T17:42:04+00:00"},{"date_created":"2017-05-10T14:14:49+00:00"},{"date_created":"2017-05-10T13:52:37+00:00"},{"date_created":"2017-05-10T13:51:40+00:00"}]}
+           GET Request: https://us15.api.mailchimp.com/3.0/lists?fields=lists.date_created
+           GET Response: 200 {"lists":[{"date_created":"2017-05-10T13:53:05+00:00"},{"date_created":"2017-08-22T20:27:56+00:00"},{"date_created":"2017-05-12T21:22:15+00:00"},{"date_created":"2017-04-27T17:42:04+00:00"},{"date_created":"2017-05-10T14:14:49+00:00"},{"date_created":"2017-05-10T13:52:37+00:00"},{"date_created":"2017-05-10T13:51:40+00:00"}]}
         
         Check the `docs <https://docs.python.org/2/library/logging.html>`__ for
         more detail on the Python logging package.
         
         Support
         -------
         
         If you are having issues, please let us know or submit a pull request.
         
         License
         -------
         
         The project is licensed under the MIT License.
         
-        .. |mailchimp3 v3.0.7 on PyPi| image:: https://img.shields.io/pypi/v/mailchimp3.svg
+        .. |mailchimp3 v3.0.9 on PyPi| image:: https://img.shields.io/pypi/v/mailchimp3.svg
            :target: https://pypi.python.org/pypi/mailchimp3
         .. |MIT license| image:: https://img.shields.io/badge/licence-MIT-blue.svg
         .. |Stable| image:: https://img.shields.io/badge/status-stable-green.svg
         
         
 Keywords: mailchimp api v3 client wrapper
 Platform: UNKNOWN
```

### Comparing `mailchimp3-3.0.7/mailchimp3.egg-info/PKG-INFO` & `mailchimp3-3.0.9/mailchimp3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: mailchimp3
-Version: 3.0.7
+Version: 3.0.9
 Summary: A python client for v3 of MailChimp API
 Home-page: https://github.com/charlesthk/python-mailchimp
 Author: Charles TISSIER
 Author-email: charles@vingtcinq.io
 License: MIT
-Description: |mailchimp3 v3.0.7 on PyPi| |MIT license| |Stable|
+Description: |mailchimp3 v3.0.9 on PyPi| |MIT license| |Stable|
         
         python-mailchimp-api
         ====================
         
         A straighforward python client for v3 of MailChimp API using requests >=
         2.7.0.
         
@@ -56,17 +56,17 @@
         
         Grab ``YOUR_API_KEY`` from your mailchimp account (Account > Extra > Api
         Keys). ``YOUR_USERNAME`` is the one you use to login on the website and
         is optional.
         
         ::
         
-            from mailchimp3 import MailChimp
+           from mailchimp3 import MailChimp
         
-            client = MailChimp(mc_api='YOUR_API_KEY', mc_user='YOUR_USERNAME')
+           client = MailChimp(mc_api='YOUR_API_KEY', mc_user='YOUR_USERNAME')
         
         OAuth Support
         ~~~~~~~~~~~~~
         
         In addition to HTTP Basic Authentication, MailChimp supports
         authentication through OAuth2. Information on obtaining the proper
         access key can be found
@@ -80,160 +80,162 @@
         skip. For endpoints that allow the pagination parameters, the all()
         method has an additional boolean ``get_all`` argument that will loop
         through all records until the API no longer returns any to get all
         records without manually performing an additional query. By default,
         count is 10 and offset is 0 for all endpoints that support it. The
         ``get_all`` parameter on the all() method on any endpoint defaults to
         false, which follows the values that are provided in the call, and using
-        ``get_all=True`` will ignore the provided count and offset to ensure
-        that all records are returned. When using get_all, the count will be
-        5000, to fetch large numbers of records without flooding the system with
-        requests. The large size of count should not impact calls which are
+        ``get_all=True`` will ignore the provided offset to ensure that all
+        records are returned. When using get_all, the count will be 500 unless
+        otherwise specified. It is strongly recommended to avoid small values
+        for ``count`` to fetch large numbers of records because this will flood
+        the system. A large ``count`` size should not impact calls which are
         expected to return a very small number of records, and should improve
-        performance for calls where fetching 5000 records would only provide a
+        performance for calls where fetching 500 records would only provide a
         fraction by preventing the delay of making a huge number of requests.
         
         ::
         
-            client.lists.members.all('123456', count=100, offset=0)
+           client.lists.members.all('123456', count=100, offset=0)
         
         Fields
         ~~~~~~
         
         Many endpoints allow you to select which fields will be returned out of
         all available fields (for example, only the email_address of a member).
         Simply add ``fields`` arguments in your function. The following only
         display email_address and id for each member in list 123456:
         
         ::
         
-            client.lists.members.all('123456', get_all=True, fields="members.email_address,members.id")
+           client.lists.members.all('123456', get_all=True, fields="members.email_address,members.id")
         
         Examples
         ~~~~~~~~
         
         ::
         
-            # returns all the lists (only name and id)
-            client.lists.all(get_all=True, fields="lists.name,lists.id")
+           # returns all the lists (only name and id)
+           client.lists.all(get_all=True, fields="lists.name,lists.id")
         
-            # returns all members inside list '123456'
-            client.lists.members.all('123456', get_all=True)
+           # returns all members inside list '123456'
+           client.lists.members.all('123456', get_all=True)
         
-            # return the first 100 member's email addresses for the list with id 123456
-            client.lists.members.all('123456', count=100, offset=0, fields="members.email_address")
+           # return the first 100 member's email addresses for the list with id 123456
+           client.lists.members.all('123456', count=100, offset=0, fields="members.email_address")
         
-            # returns the list matching id '123456'
-            client.lists.get('123456')
-        
-            # add John Doe with email john.doe@example.com to list matching id '123456'
-            client.lists.members.create('123456', {
-                'email_address': 'john.doe@example.com',
-                'status': 'subscribed',
-                'merge_fields': {
-                    'FNAME': 'John',
-                    'LNAME': 'Doe',
-                },
-            })
-        
-            # returns all the campaigns
-            client.campaigns.all(get_all=True)
-        
-            # You can also disable at runtime with the optional ``enabled`` parameter.
-            # Every API call will return None
-            client = MailChimp('YOUR SECRET KEY', enabled=False)
-        
-            # You are encouraged to specify a value in seconds for the ``timeout``
-            # parameter to avoid hanging requests.
-            client = MailChimp('YOUR SECRET KEY', timeout=10.0)
-        
-            # You are encouraged to specify a User-Agent for requests to the MailChimp
-            # API. Headers can be specified using the ``request_headers`` parameter.
-            headers = requests.utils.default_headers()
-            headers['User-Agent'] = 'Example (example@example.com)'
-            client = MailChimp('YOUR SECRET KEY', request_headers=headers)
+           # returns the list matching id '123456'
+           client.lists.get('123456')
+        
+           # add John Doe with email john.doe@example.com to list matching id '123456'
+           client.lists.members.create('123456', {
+               'email_address': 'john.doe@example.com',
+               'status': 'subscribed',
+               'merge_fields': {
+                   'FNAME': 'John',
+                   'LNAME': 'Doe',
+               },
+           })
+        
+           # returns all the campaigns
+           client.campaigns.all(get_all=True)
+        
+           # You can also disable at runtime with the optional ``enabled`` parameter.
+           # Every API call will return None
+           client = MailChimp('YOUR SECRET KEY', enabled=False)
+        
+           # You are encouraged to specify a value in seconds for the ``timeout``
+           # parameter to avoid hanging requests.
+           client = MailChimp('YOUR SECRET KEY', timeout=10.0)
+        
+           # You are encouraged to specify a User-Agent for requests to the MailChimp
+           # API. Headers can be specified using the ``request_headers`` parameter.
+           headers = requests.utils.default_headers()
+           headers['User-Agent'] = 'Example (example@example.com)'
+           client = MailChimp('YOUR SECRET KEY', request_headers=headers)
         
         API Structure
         -------------
         
         All endpoints follow the structure listed in the official MailChimp API
         v3 documentation. The structure will be listed below and then the
         individual methods available after.
         
         ::
         
-            MailChimp
-            +- Root
-            +- Authorized Apps
-            +- Automations
-            |  +- Actions
-            |  +- Emails
-            |  |  +- Actions
-            |  |  +- Queues
-            |  +- Removed Subscribers
-            +- Batch Operations
-            +- Batch Webhooks
-            +- Campaign Folders
-            +- Campaigns
-            |  +- Actions
-            |  +- Content
-            |  +- Feedback
-            |  +- Send Checklist
-            +- Conversations
-            |  +- Messages
-            +- Stores
-            |  +- Carts
-            |  |  +- Lines
-            |  +- Customers
-            |  +- Orders
-            |  |  +- Lines
-            |  +- Products
-            |     +- Images
-            |     +- Variants
-            |  +- Promo Rules
-            |     +- Promo Codes
-            +- File Manager Files
-            +- File Manager Folders
-            +- Lists
-            |  +- Abuse Reports
-            |  +- Activity
-            |  +- Clients
-            |  +- Growth History
-            |  +- Interest Categories
-            |  |  +- Interests
-            |  +- Members
-            |  |  +- Activity
-            |  |  +- Goals
-            |  |  +- Notes
-            |  +- Merge Fields
-            |  +- Segments
-            |  |  +- Segment Members
-            |  +- Signup Forms
-            |  +- Twitter Lead Generation Carts
-            |  +- Webhooks
-            +- Ping
-            +- Reports
-            |  +- Campaign Abuse
-            |  +- Campaign Advice
-            |  +- Campaign Open reports
-            |  +- Click Reports
-            |  |  +- Members
-            |  +- Domain Performance
-            |  +- EepURL Reports
-            |  +- Email Activity
-            |  +- Google Analytics
-            |  +- Location
-            |  +- Sent To
-            |  +- Sub-Reports
-            |  +- Unsubscribes
-            +- Seach Campaigns
-            +- Search Members
-            +- Template Folders
-            +- Templates
-               +- Default Content
+           MailChimp
+           +- Root
+           +- Authorized Apps
+           +- Automations
+           |  +- Actions
+           |  +- Emails
+           |  |  +- Actions
+           |  |  +- Queues
+           |  +- Removed Subscribers
+           +- Batch Operations
+           +- Batch Webhooks
+           +- Campaign Folders
+           +- Campaigns
+           |  +- Actions
+           |  +- Content
+           |  +- Feedback
+           |  +- Send Checklist
+           +- Conversations
+           |  +- Messages
+           +- Stores
+           |  +- Carts
+           |  |  +- Lines
+           |  +- Customers
+           |  +- Orders
+           |  |  +- Lines
+           |  +- Products
+           |     +- Images
+           |     +- Variants
+           |  +- Promo Rules
+           |     +- Promo Codes
+           +- File Manager Files
+           +- File Manager Folders
+           +- Lists
+           |  +- Abuse Reports
+           |  +- Activity
+           |  +- Clients
+           |  +- Growth History
+           |  +- Interest Categories
+           |  |  +- Interests
+           |  +- Members
+           |  |  +- Activity
+           |  |  +- Goals
+           |  |  +- Notes
+           |  |  +- Tags
+           |  +- Merge Fields
+           |  +- Segments
+           |  |  +- Segment Members
+           |  +- Signup Forms
+           |  +- Twitter Lead Generation Carts
+           |  +- Webhooks
+           +- Ping
+           +- Reports
+           |  +- Campaign Abuse
+           |  +- Campaign Advice
+           |  +- Campaign Open reports
+           |  +- Click Reports
+           |  |  +- Members
+           |  +- Domain Performance
+           |  +- EepURL Reports
+           |  +- Email Activity
+           |  +- Google Analytics
+           |  +- Location
+           |  +- Sent To
+           |  +- Sub-Reports
+           |  +- Unsubscribes
+           +- Seach Campaigns
+           +- Search Members
+           +- Template Folders
+           +- Templates
+              +- Default Content
         
         API Endpoints
         -------------
         
         Below is the list of all endpoints and the methods that can be called
         against them. Any endpoint that has a method that takes an ID argument
         (for example the app_id in the authorized_apps endpoint or the
@@ -252,682 +254,690 @@
         .. _root-1:
         
         Root
         ^^^^
         
         ::
         
-            client.root.get()
+           client.root.get()
         
         Authorized Apps
         ~~~~~~~~~~~~~~~
         
         .. _authorized-apps-1:
         
         Authorized Apps
         ^^^^^^^^^^^^^^^
         
         ::
         
-            client.authorized_apps.create(data={})
-            client.authorized_apps.all(get_all=False)
-            client.authorized_apps.get(app_id='')
+           client.authorized_apps.create(data={})
+           client.authorized_apps.all(get_all=False)
+           client.authorized_apps.get(app_id='')
         
         Automations
         ~~~~~~~~~~~
         
         .. _automations-1:
         
         Automations
         ^^^^^^^^^^^
         
         ::
         
-            client.automations.all(get_all=False)
-            client.automations.get(workflow_id='')
+           client.automations.all(get_all=False)
+           client.automations.get(workflow_id='')
         
         Automation Actions
         ^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.automations.actions.pause(workflow_id='')
-            client.automations.actions.start(workflow_id='')
+           client.automations.actions.pause(workflow_id='')
+           client.automations.actions.start(workflow_id='')
         
         Automation Emails
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.automations.emails.all(workflow_id='')
-            client.automations.emails.get(workflow_id='', email_id='')
+           client.automations.emails.all(workflow_id='')
+           client.automations.emails.get(workflow_id='', email_id='')
         
         Automation Email Actions
         ^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.automations.emails.actions.pause(workflow_id='', email_id='')
-            client.automations.emails.actions.start(workflow_id='', email_id='')
+           client.automations.emails.actions.pause(workflow_id='', email_id='')
+           client.automations.emails.actions.start(workflow_id='', email_id='')
         
         Automation Email Queues
         ^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.automations.emails.queues.create(workflow_id='', email_id='', data={})
-            client.automations.emails.queues.all(workflow_id='', email_id='')
-            client.automations.emails.queues.get(workflow_id='', email_id='', subscriber_hash='')
+           client.automations.emails.queues.create(workflow_id='', email_id='', data={})
+           client.automations.emails.queues.all(workflow_id='', email_id='')
+           client.automations.emails.queues.get(workflow_id='', email_id='', subscriber_hash='')
         
         Automation Removed Subscribers
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.automations.removed_subscribers.create(workflow_id='', data={})
-            client.automations.removed_subscribers.all(workflow_id='')
+           client.automations.removed_subscribers.create(workflow_id='', data={})
+           client.automations.removed_subscribers.all(workflow_id='')
         
         Batch Operations
         ~~~~~~~~~~~~~~~~
         
         .. _batch-operations-1:
         
         Batch Operations
         ^^^^^^^^^^^^^^^^
         
         ::
         
-            client.batch_operations.create(data={})
-            client.batch_operations.all(get_all=False)
-            client.batch_operations.get(batch_id='')
-            client.batch_operations.delete(batch_id='')
+           client.batch_operations.create(data={})
+           client.batch_operations.all(get_all=False)
+           client.batch_operations.get(batch_id='')
+           client.batch_operations.delete(batch_id='')
         
         Batch Webhooks
         ~~~~~~~~~~~~~~
         
         .. _batch-webhooks-1:
         
         Batch Webhooks
         ^^^^^^^^^^^^^^
         
         ::
         
-            client.batch_webhooks.create(data={})
-            client.batch_webhooks.all(get_all=False)
-            client.batch_webhooks.get(batch_webhook_id='')
-            client.batch_webhooks.update(batch_webhook_id='', data={})
-            client.batch_webhooks.delete(batch_webhook_id='')
+           client.batch_webhooks.create(data={})
+           client.batch_webhooks.all(get_all=False)
+           client.batch_webhooks.get(batch_webhook_id='')
+           client.batch_webhooks.update(batch_webhook_id='', data={})
+           client.batch_webhooks.delete(batch_webhook_id='')
         
         Campaigns
         ~~~~~~~~~
         
         Folders
         ^^^^^^^
         
         ::
         
-            client.campaign_folders.create(data={})
-            client.campaign_folders.all(get_all=False)
-            client.campaign_folders.get(folder_id='')
-            client.campaign_folders.update(folder_id='', data={})
-            client.campaign_folders.delete(folder_id='')
+           client.campaign_folders.create(data={})
+           client.campaign_folders.all(get_all=False)
+           client.campaign_folders.get(folder_id='')
+           client.campaign_folders.update(folder_id='', data={})
+           client.campaign_folders.delete(folder_id='')
         
         .. _campaigns-1:
         
         Campaigns
         ^^^^^^^^^
         
         ::
         
-            client.campaigns.create(data={})
-            client.campaigns.all(get_all=False)
-            client.campaigns.get(campaign_id='')
-            client.campaigns.update(campaign_id='')
-            client.campaigns.delete(campaign_id='')
+           client.campaigns.create(data={})
+           client.campaigns.all(get_all=False)
+           client.campaigns.get(campaign_id='')
+           client.campaigns.update(campaign_id='')
+           client.campaigns.delete(campaign_id='')
         
         Campaign Actions
         ^^^^^^^^^^^^^^^^
         
         ::
         
-            client.campaigns.actions.cancel(campaign_id='')
-            client.campaigns.actions.pause(campaign_id='')
-            client.campaigns.actions.replicate(campaign_id='')
-            client.campaigns.actions.resume(campaign_id='')
-            client.campaigns.actions.schedule(campaign_id='', data={})
-            client.campaigns.actions.send(campaign_id='')
-            client.campaigns.actions.test(campaign_id='', data={})
-            client.campaigns.actions.unschedule(campaign_id='')
+           client.campaigns.actions.cancel(campaign_id='')
+           client.campaigns.actions.pause(campaign_id='')
+           client.campaigns.actions.replicate(campaign_id='')
+           client.campaigns.actions.resume(campaign_id='')
+           client.campaigns.actions.schedule(campaign_id='', data={})
+           client.campaigns.actions.send(campaign_id='')
+           client.campaigns.actions.test(campaign_id='', data={})
+           client.campaigns.actions.unschedule(campaign_id='')
         
         Campaign Content
         ^^^^^^^^^^^^^^^^
         
         ::
         
-            client.campaigns.content.get(campaign_id='')
-            client.campaigns.content.update(campaign_id='', data={})
+           client.campaigns.content.get(campaign_id='')
+           client.campaigns.content.update(campaign_id='', data={})
         
         Campaign Feedback
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.campaigns.feedback.create(campaign_id='', data={})
-            client.campaigns.feedback.all(campaign_id='', get_all=False)
-            client.campaigns.feedback.get(campaign_id='', feedback_id='')
-            client.campaigns.feedback.update(campaign_id='', feedback_id='', data={})
-            client.campaigns.feedback.delete(campaign_id='', feedback_id='')
+           client.campaigns.feedback.create(campaign_id='', data={})
+           client.campaigns.feedback.all(campaign_id='', get_all=False)
+           client.campaigns.feedback.get(campaign_id='', feedback_id='')
+           client.campaigns.feedback.update(campaign_id='', feedback_id='', data={})
+           client.campaigns.feedback.delete(campaign_id='', feedback_id='')
         
         Campaign Send Checklist
         ^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.campaigns.send_checklist.get(campaign_id='')
+           client.campaigns.send_checklist.get(campaign_id='')
         
         Conversations
         ~~~~~~~~~~~~~
         
         .. _conversations-1:
         
         Conversations
         ^^^^^^^^^^^^^
         
         ::
         
-            client.conversations.all(get_all=False)
-            client.conversations.get(conversation_id='')
+           client.conversations.all(get_all=False)
+           client.conversations.get(conversation_id='')
         
         Conversation Messages
         ^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.conversations.messages.create(conversation_id='', data={})
-            client.conversations.messages.all(conversation_id='')
-            client.conversations.messages.get(conversation_id='', message_id='')
+           client.conversations.messages.create(conversation_id='', data={})
+           client.conversations.messages.all(conversation_id='')
+           client.conversations.messages.get(conversation_id='', message_id='')
         
         E-Commerce
         ~~~~~~~~~~
         
         Stores
         ^^^^^^
         
         ::
         
-            client.stores.create(data={})
-            client.stores.all(get_all=False)
-            client.stores.get(store_id='')
-            client.stores.update(store_id='', data={})
-            client.stores.delete(store_id='')
+           client.stores.create(data={})
+           client.stores.all(get_all=False)
+           client.stores.get(store_id='')
+           client.stores.update(store_id='', data={})
+           client.stores.delete(store_id='')
         
         Store Carts
         ^^^^^^^^^^^
         
         ::
         
-            client.stores.carts.create(store_id='', data={})
-            client.stores.carts.all(store_id='', get_all=False)
-            client.stores.carts.get(store_id='', cart_id='')
-            client.stores.carts.update(store_id='', cart_id='', data={})
-            client.stores.carts.delete(store_id='', cart_id='')
+           client.stores.carts.create(store_id='', data={})
+           client.stores.carts.all(store_id='', get_all=False)
+           client.stores.carts.get(store_id='', cart_id='')
+           client.stores.carts.update(store_id='', cart_id='', data={})
+           client.stores.carts.delete(store_id='', cart_id='')
         
         Store Cart Lines
         ^^^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.carts.lines.create(store_id='', cart_id='', data={})
-            client.stores.carts.lines.all(store_id='', cart_id='', get_all=False)
-            client.stores.carts.lines.get(store_id='', cart_id='', line_id='')
-            client.stores.carts.lines.update(store_id='', cart_id='', line_id='', data={})
-            client.stores.carts.lines.delete(store_id='', cart_id='', line_id='')
+           client.stores.carts.lines.create(store_id='', cart_id='', data={})
+           client.stores.carts.lines.all(store_id='', cart_id='', get_all=False)
+           client.stores.carts.lines.get(store_id='', cart_id='', line_id='')
+           client.stores.carts.lines.update(store_id='', cart_id='', line_id='', data={})
+           client.stores.carts.lines.delete(store_id='', cart_id='', line_id='')
         
         Store Customers
         ^^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.customers.create(store_id='', data={})
-            client.stores.customers.all(store_id='', get_all=False)
-            client.stores.customers.get(store_id='', customer_id='')
-            client.stores.customers.update(store_id='', customer_id='', data={})
-            client.stores.customers.create_or_update(store_id='', customer_id='', data={})
-            client.stores.customers.delete(store_id='', customer_id='')
+           client.stores.customers.create(store_id='', data={})
+           client.stores.customers.all(store_id='', get_all=False)
+           client.stores.customers.get(store_id='', customer_id='')
+           client.stores.customers.update(store_id='', customer_id='', data={})
+           client.stores.customers.create_or_update(store_id='', customer_id='', data={})
+           client.stores.customers.delete(store_id='', customer_id='')
         
         Store Orders
         ^^^^^^^^^^^^
         
         ::
         
-            client.stores.orders.create(store_id='', data={})
-            client.stores.orders.all(store_id='', get_all=False)
-            client.stores.orders.get(store_id='', order_id='')
-            client.stores.orders.update(store_id='', order_id='', data={})
-            client.stores.orders.delete(store_id='', order_id='')
+           client.stores.orders.create(store_id='', data={})
+           client.stores.orders.all(store_id='', get_all=False)
+           client.stores.orders.get(store_id='', order_id='')
+           client.stores.orders.update(store_id='', order_id='', data={})
+           client.stores.orders.delete(store_id='', order_id='')
         
         Store Order Lines
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.orders.lines.create(store_id='', order_id='', data={})
-            client.stores.orders.lines.all(store_id='', order_id='', get_all=False)
-            client.stores.orders.lines.get(store_id='', order_id='', line_id='')
-            client.stores.orders.lines.update(store_id='', order_id='', line_id='', data={})
-            client.stores.orders.lines.delete(store_id='', order_id='', line_id='')
+           client.stores.orders.lines.create(store_id='', order_id='', data={})
+           client.stores.orders.lines.all(store_id='', order_id='', get_all=False)
+           client.stores.orders.lines.get(store_id='', order_id='', line_id='')
+           client.stores.orders.lines.update(store_id='', order_id='', line_id='', data={})
+           client.stores.orders.lines.delete(store_id='', order_id='', line_id='')
         
         Store Products
         ^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.products.create(store_id='', data={})
-            client.stores.products.all(store_id='', get_all=False)
-            client.stores.products.get(store_id='', product_id='')
-            client.stores.products.update(store_id='', product_id='')
-            client.stores.products.delete(store_id='', product_id='')
+           client.stores.products.create(store_id='', data={})
+           client.stores.products.all(store_id='', get_all=False)
+           client.stores.products.get(store_id='', product_id='')
+           client.stores.products.update(store_id='', product_id='')
+           client.stores.products.delete(store_id='', product_id='')
         
         Store Product Images
         ^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.products.images.create(store_id='', product_id='', data={})
-            client.stores.products.images.all(store_id='', product_id='', get_all=False)
-            client.stores.products.images.get(store_id='', product_id='', image_id='')
-            client.stores.products.images.update(store_id='', product_id='', image_id='', data={})
-            client.stores.products.images.delete(store_id='', product_id='', image_id='')
+           client.stores.products.images.create(store_id='', product_id='', data={})
+           client.stores.products.images.all(store_id='', product_id='', get_all=False)
+           client.stores.products.images.get(store_id='', product_id='', image_id='')
+           client.stores.products.images.update(store_id='', product_id='', image_id='', data={})
+           client.stores.products.images.delete(store_id='', product_id='', image_id='')
         
         Store Product Variants
         ^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.stores.products.variants.create(store_id='', product_id='', data={})
-            client.stores.products.variants.all(store_id='', product_id='', get_all=False)
-            client.stores.products.variants.get(store_id='', product_id='', variant_id='')
-            client.stores.products.variants.update(store_id='', product_id='', variant_id='', data={})
-            client.stores.products.variants.create_or_update(store_id='', product_id='', variant_id='', data={})
-            client.stores.products.variants.delete(store_id='', product_id='', variant_id='')
+           client.stores.products.variants.create(store_id='', product_id='', data={})
+           client.stores.products.variants.all(store_id='', product_id='', get_all=False)
+           client.stores.products.variants.get(store_id='', product_id='', variant_id='')
+           client.stores.products.variants.update(store_id='', product_id='', variant_id='', data={})
+           client.stores.products.variants.create_or_update(store_id='', product_id='', variant_id='', data={})
+           client.stores.products.variants.delete(store_id='', product_id='', variant_id='')
         
         File Manager
         ~~~~~~~~~~~~
         
         Files
         ^^^^^
         
         ::
         
-            client.files.create(data={})
-            client.files.all(get_all=False)
-            client.files.get(file_id='')
-            client.files.update(file_id='', data={})
-            client.files.delete(file_id='')
+           client.files.create(data={})
+           client.files.all(get_all=False)
+           client.files.get(file_id='')
+           client.files.update(file_id='', data={})
+           client.files.delete(file_id='')
         
         .. _folders-1:
         
         Folders
         ^^^^^^^
         
         ::
         
-            client.folders.create(data={})
-            client.folders.all(get_all=False)
-            client.folders.get(folder_id='')
-            client.folders.update(folder_id='', data={})
-            client.folders.delete(folder_id='')
+           client.folders.create(data={})
+           client.folders.all(get_all=False)
+           client.folders.get(folder_id='')
+           client.folders.update(folder_id='', data={})
+           client.folders.delete(folder_id='')
         
         Lists
         ~~~~~
         
         .. _lists-1:
         
         Lists
         ^^^^^
         
         ::
         
-            client.lists.create(data={})
-            client.lists.update_members(list_id='', data={})
-            client.lists.all(get_all=False)
-            client.lists.get(list_id='')
-            client.lists.update(list_id='', data={})
-            client.lists.delete(list_id='')
+           client.lists.create(data={})
+           client.lists.update_members(list_id='', data={})
+           client.lists.all(get_all=False)
+           client.lists.get(list_id='')
+           client.lists.update(list_id='', data={})
+           client.lists.delete(list_id='')
         
         List Abuse Reports
         ^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.abuse_reports.all(list_id='', get_all=False)
-            client.lists.abuse_reports.get(list_id='', report_id='')
+           client.lists.abuse_reports.all(list_id='', get_all=False)
+           client.lists.abuse_reports.get(list_id='', report_id='')
         
         List Activity
         ^^^^^^^^^^^^^
         
         ::
         
-            client.lists.activity.all(list_id='')
+           client.lists.activity.all(list_id='')
         
         List Clients
         ^^^^^^^^^^^^
         
         ::
         
-            client.lists.clients.all(list_id='')
+           client.lists.clients.all(list_id='')
         
         List Growth History
         ^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.growth_history.all(list_id='', get_all=False)
-            client.lists.growth_history.get(list_id='', month='')
+           client.lists.growth_history.all(list_id='', get_all=False)
+           client.lists.growth_history.get(list_id='', month='')
         
         List Interest Categories
         ^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.interest_categories.create(list_id='', data={})
-            client.lists.interest_categories.all(list_id='', get_all=False)
-            client.lists.interest_categories.get(list_id='', category_id='')
-            client.lists.interest_categories.update(list_id='', category_id='', data={})
-            client.lists.interest_categories.delete(list_id='', category_id='')
+           client.lists.interest_categories.create(list_id='', data={})
+           client.lists.interest_categories.all(list_id='', get_all=False)
+           client.lists.interest_categories.get(list_id='', category_id='')
+           client.lists.interest_categories.update(list_id='', category_id='', data={})
+           client.lists.interest_categories.delete(list_id='', category_id='')
         
         List Interest Category Interests
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.interest_categories.interests.create(list_id='', category_id='', data={})
-            client.lists.interest_categories.interests.all(list_id='', category_id='', get_all=False)
-            client.lists.interest_categories.interests.get(list_id='', category_id='', interest_id='')
-            client.lists.interest_categories.interests.update(list_id='', category_id='', interest_id='', data={})
-            client.lists.interest_categories.interests.delete(list_id='', category_id='', interest_id='')
+           client.lists.interest_categories.interests.create(list_id='', category_id='', data={})
+           client.lists.interest_categories.interests.all(list_id='', category_id='', get_all=False)
+           client.lists.interest_categories.interests.get(list_id='', category_id='', interest_id='')
+           client.lists.interest_categories.interests.update(list_id='', category_id='', interest_id='', data={})
+           client.lists.interest_categories.interests.delete(list_id='', category_id='', interest_id='')
         
         List Members
         ^^^^^^^^^^^^
         
         ::
         
-            client.lists.members.create(list_id='', data={})
-            client.lists.members.all(list_id='', get_all=False)
-            client.lists.members.get(list_id='', subscriber_hash='')
-            client.lists.members.update(list_id='', subscriber_hash='', data={})
-            client.lists.members.create_or_update(list_id='', subscriber_hash='', data={})
-            client.lists.members.delete(list_id='', subscriber_hash='')
-            client.lists.members.delete_permanent(list_id='', subscriber_hash='')
+           client.lists.members.create(list_id='', data={})
+           client.lists.members.all(list_id='', get_all=False)
+           client.lists.members.get(list_id='', subscriber_hash='')
+           client.lists.members.update(list_id='', subscriber_hash='', data={})
+           client.lists.members.create_or_update(list_id='', subscriber_hash='', data={})
+           client.lists.members.delete(list_id='', subscriber_hash='')
+           client.lists.members.delete_permanent(list_id='', subscriber_hash='')
         
         List Member Activity
         ^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.members.activity.all(list_id='', subscriber_hash='')
+           client.lists.members.activity.all(list_id='', subscriber_hash='')
         
         List Member Goals
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.members.goals.all(list_id='', subscriber_hash='')
+           client.lists.members.goals.all(list_id='', subscriber_hash='')
         
         List Member Notes
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.members.notes.create(list_id='', subscriber_hash='', data={})
-            client.lists.members.notes.all(list_id='', subscriber_hash='', get_all=False)
-            client.lists.members.notes.get(list_id='', subscriber_hash='', note_id='')
-            client.lists.members.notes.update(list_id='', subscriber_hash='', note_id='', data={})
-            client.lists.members.notes.delete(list_id='', subscriber_hash='', note_id='')
+           client.lists.members.notes.create(list_id='', subscriber_hash='', data={})
+           client.lists.members.notes.all(list_id='', subscriber_hash='', get_all=False)
+           client.lists.members.notes.get(list_id='', subscriber_hash='', note_id='')
+           client.lists.members.notes.update(list_id='', subscriber_hash='', note_id='', data={})
+           client.lists.members.notes.delete(list_id='', subscriber_hash='', note_id='')
+        
+        List Member Tags
+        ^^^^^^^^^^^^^^^^
+        
+        ::
+        
+           client.lists.members.tags.update(list_id='', subscriber_hash='', data={})
+           client.lists.members.tags.all(list_id='', subscriber_hash='')
         
         List Merge Fields
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.merge_fields.create(list_id='', data={})
-            client.lists.merge_fields.all(list_id='', get_all=False)
-            client.lists.merge_fields.get(list_id='', merge_id='')
-            client.lists.merge_fields.update(list_id='', merge_id='', data={})
-            client.lists.merge_fields.delete(list_id='', merge_id='')
+           client.lists.merge_fields.create(list_id='', data={})
+           client.lists.merge_fields.all(list_id='', get_all=False)
+           client.lists.merge_fields.get(list_id='', merge_id='')
+           client.lists.merge_fields.update(list_id='', merge_id='', data={})
+           client.lists.merge_fields.delete(list_id='', merge_id='')
         
         List Segments
         ^^^^^^^^^^^^^
         
         ::
         
-            client.lists.segments.create(list_id='', data={})
-            client.lists.segments.all(list_id='', get_all=False)
-            client.lists.segments.get(list_id='', segment_id='')
-            client.lists.segments.update(list_id='', segment_id='', data={})
-            client.lists.segments.update_members(list_id='', segment_id='', data={})
-            client.lists.segments.delete(list_id='', segment_id='')
+           client.lists.segments.create(list_id='', data={})
+           client.lists.segments.all(list_id='', get_all=False)
+           client.lists.segments.get(list_id='', segment_id='')
+           client.lists.segments.update(list_id='', segment_id='', data={})
+           client.lists.segments.update_members(list_id='', segment_id='', data={})
+           client.lists.segments.delete(list_id='', segment_id='')
         
         List Segment Members
         ^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.segments.members.create(list_id='', segment_id='', data={})
-            client.lists.segments.members.all(list_id='', segment_id='', get_all=False)
-            client.lists.segments.members.delete(list_id='', segment_id='', subscriber_hash='')
+           client.lists.segments.members.create(list_id='', segment_id='', data={})
+           client.lists.segments.members.all(list_id='', segment_id='', get_all=False)
+           client.lists.segments.members.delete(list_id='', segment_id='', subscriber_hash='')
         
         List Signup Forms
         ^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.lists.signup_forms.create(list_id='', data={})
-            client.lists.signup_forms.all(list_id='')
+           client.lists.signup_forms.create(list_id='', data={})
+           client.lists.signup_forms.all(list_id='')
         
         List Webhooks
         ^^^^^^^^^^^^^
         
         ::
         
-            client.lists.webhooks.create(list_id='', data={})
-            client.lists.webhooks.all(list_id='')
-            client.lists.webhooks.get(list_id='', webhook_id='')
-            client.lists.webhooks.update(list_id='', webhook_id='', data={})
-            client.lists.webhooks.delete(list_id='', webhook_id='')
+           client.lists.webhooks.create(list_id='', data={})
+           client.lists.webhooks.all(list_id='')
+           client.lists.webhooks.get(list_id='', webhook_id='')
+           client.lists.webhooks.update(list_id='', webhook_id='', data={})
+           client.lists.webhooks.delete(list_id='', webhook_id='')
         
         Reports
         ~~~~~~~
         
         .. _reports-1:
         
         Reports
         ^^^^^^^
         
         ::
         
-            client.reports.all(get_all=False)
-            client.reports.get(campaign_id='')
+           client.reports.all(get_all=False)
+           client.reports.get(campaign_id='')
         
         Campaign Abuse Reports
         ^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.abuse_reports.all(campaign_id='')
-            client.reports.abuse_reports.get(campaign_id='', report_id='')
+           client.reports.abuse_reports.all(campaign_id='')
+           client.reports.abuse_reports.get(campaign_id='', report_id='')
         
         Campaign Advice
         ^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.advice.all(campaign_id='')
+           client.reports.advice.all(campaign_id='')
         
         Click Details Report
         ^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.click_details.all(campaign_id='', get_all=False)
-            client.reports.click_details.get(campaign_id='', link_id='')
+           client.reports.click_details.all(campaign_id='', get_all=False)
+           client.reports.click_details.get(campaign_id='', link_id='')
         
         Click Details Report Members
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.click_details.members.all(campaign_id='', link_id='', get_all=False)
-            client.reports.click_details.members.get(campaign_id='', link_id='', subscriber_hash='')
+           client.reports.click_details.members.all(campaign_id='', link_id='', get_all=False)
+           client.reports.click_details.members.get(campaign_id='', link_id='', subscriber_hash='')
         
         Domain Performance Reports
         ^^^^^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.domain_performance.all(campaign_id='')
+           client.reports.domain_performance.all(campaign_id='')
         
         EepURL Reports
         ^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.eepurl.all(camnpaign_id='')
+           client.reports.eepurl.all(camnpaign_id='')
         
         Email Activity Reports
         ^^^^^^^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.email_activity.all(campaign_id='', get_all=False)
-            client.reports.email_activity.get(campaign_id='', subscriber_hash='')
+           client.reports.email_activity.all(campaign_id='', get_all=False)
+           client.reports.email_activity.get(campaign_id='', subscriber_hash='')
         
         Locations Report
         ^^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.locations.all(campaign_id='', get_all=False)
+           client.reports.locations.all(campaign_id='', get_all=False)
         
         Sent To Reports
         ^^^^^^^^^^^^^^^
         
         ::
         
-            client.reports.sent_to.all(campaign_id='', get_all=False)
-            client.reports.sent_to.get(campaign_id='', subscriber_hash='')
+           client.reports.sent_to.all(campaign_id='', get_all=False)
+           client.reports.sent_to.get(campaign_id='', subscriber_hash='')
         
         Sub-Reports
         ^^^^^^^^^^^
         
         ::
         
-            client.reports.subreports.all(campaign_id='')
+           client.reports.subreports.all(campaign_id='')
         
         Unsubscribes
         ^^^^^^^^^^^^
         
         ::
         
-            client.reports.unsubscribes.all(campaign_id='', get_all=False)
-            client.reports.unsubscribes.get(campaign_id='', subscriber_hash='')
+           client.reports.unsubscribes.all(campaign_id='', get_all=False)
+           client.reports.unsubscribes.get(campaign_id='', subscriber_hash='')
         
         Search
         ~~~~~~
         
         .. _campaigns-2:
         
         Campaigns
         ^^^^^^^^^
         
         ::
         
-            client.search_campaigns.get()
+           client.search_campaigns.get()
         
         Members
         ^^^^^^^
         
         ::
         
-            client.search_members.get()
+           client.search_members.get()
         
         Templates
         ~~~~~~~~~
         
         .. _folders-2:
         
         Folders
         ^^^^^^^
         
         ::
         
-            client.template_folders.create(data={})
-            client.template_folders.all(get_all=False)
-            client.template_folders.get(folder_id='')
-            client.template_folders.update(folder_id='', data={})
-            client.template_folders.delete(folder_id='')
+           client.template_folders.create(data={})
+           client.template_folders.all(get_all=False)
+           client.template_folders.get(folder_id='')
+           client.template_folders.update(folder_id='', data={})
+           client.template_folders.delete(folder_id='')
         
         .. _templates-1:
         
         Templates
         ^^^^^^^^^
         
         ::
         
-            client.templates.create(data={})
-            client.templates.all(get_all=False)
-            client.templates.get(template_id='')
-            client.templates.update(template_id='', data={})
-            client.templates.delete(template_id='')
+           client.templates.create(data={})
+           client.templates.all(get_all=False)
+           client.templates.get(template_id='')
+           client.templates.update(template_id='', data={})
+           client.templates.delete(template_id='')
         
         Default Content
         ^^^^^^^^^^^^^^^
         
         ::
         
-            client.templates.default_content.all(template_id='')
+           client.templates.default_content.all(template_id='')
         
         Logging
         -------
         
         The MailChimp client will log request/response detail into the
         mailchimp3.client logging namespace. Consider the following snippet to
         get started with logging:
         
         .. code:: python
         
-            import logging
-            fh = logging.FileHandler('/path/to/some/log.log')
-            logger = logging.getLogger('mailchimp3.client')
-            logger.addHandler(fh)
+           import logging
+           fh = logging.FileHandler('/path/to/some/log.log')
+           logger = logging.getLogger('mailchimp3.client')
+           logger.addHandler(fh)
         
-            # use the client normally
-            client.lists.all(**{'fields': 'lists.date_created'})
+           # use the client normally
+           client.lists.all(**{'fields': 'lists.date_created'})
         
         request/response detail will be appended into /path/to/some/log.log:
         
         ::
         
-            GET Request: https://us15.api.mailchimp.com/3.0/lists?fields=lists.date_created
-            GET Response: 200 {"lists":[{"date_created":"2017-05-10T13:53:05+00:00"},{"date_created":"2017-08-22T20:27:56+00:00"},{"date_created":"2017-05-12T21:22:15+00:00"},{"date_created":"2017-04-27T17:42:04+00:00"},{"date_created":"2017-05-10T14:14:49+00:00"},{"date_created":"2017-05-10T13:52:37+00:00"},{"date_created":"2017-05-10T13:51:40+00:00"}]}
+           GET Request: https://us15.api.mailchimp.com/3.0/lists?fields=lists.date_created
+           GET Response: 200 {"lists":[{"date_created":"2017-05-10T13:53:05+00:00"},{"date_created":"2017-08-22T20:27:56+00:00"},{"date_created":"2017-05-12T21:22:15+00:00"},{"date_created":"2017-04-27T17:42:04+00:00"},{"date_created":"2017-05-10T14:14:49+00:00"},{"date_created":"2017-05-10T13:52:37+00:00"},{"date_created":"2017-05-10T13:51:40+00:00"}]}
         
         Check the `docs <https://docs.python.org/2/library/logging.html>`__ for
         more detail on the Python logging package.
         
         Support
         -------
         
         If you are having issues, please let us know or submit a pull request.
         
         License
         -------
         
         The project is licensed under the MIT License.
         
-        .. |mailchimp3 v3.0.7 on PyPi| image:: https://img.shields.io/pypi/v/mailchimp3.svg
+        .. |mailchimp3 v3.0.9 on PyPi| image:: https://img.shields.io/pypi/v/mailchimp3.svg
            :target: https://pypi.python.org/pypi/mailchimp3
         .. |MIT license| image:: https://img.shields.io/badge/licence-MIT-blue.svg
         .. |Stable| image:: https://img.shields.io/badge/status-stable-green.svg
         
         
 Keywords: mailchimp api v3 client wrapper
 Platform: UNKNOWN
```

### Comparing `mailchimp3-3.0.7/mailchimp3.egg-info/SOURCES.txt` & `mailchimp3-3.0.9/mailchimp3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/setup.py` & `mailchimp3-3.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         long_description = file.read()
 except Exception:
     long_description = ''
 
 
 setup(
     name='mailchimp3',
-    version='3.0.7',
+    version='3.0.9',
     description='A python client for v3 of MailChimp API',
     long_description=long_description,
     url='https://github.com/charlesthk/python-mailchimp',
     author='Charles TISSIER',
     author_email='charles@vingtcinq.io',
     license='MIT',
     classifiers=[
```

### Comparing `mailchimp3-3.0.7/mailchimp3/baseapi.py` & `mailchimp3-3.0.9/mailchimp3/baseapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,26 +48,30 @@
         # fields as a query string parameter should be a string with
         # comma-separated substring values to pass along to
         # self._mc_client._get(). It should also contain total_items whenever
         # the parameter is employed, which is forced here.
         if 'fields' in queryparams:
             if 'total_items' not in queryparams['fields'].split(','):
                 queryparams['fields'] += ',total_items'
-        # Remove offset and count if provided in queryparams
-        # to avoid 'multiple values for keyword argument' TypeError
+        # Remove offset if provided in queryparams to avoid 'multiple values
+        # for keyword argument' TypeError
         queryparams.pop("offset", None)
-        queryparams.pop("count", None)
-        # Fetch results from mailchimp, up to first 1000
-        result = self._mc_client._get(url=url, offset=0, count=1000, **queryparams)
+
+        # Fetch results from mailchimp, up to first count. If count is not
+        # provided, return a count of 500. The maximum value supported by the
+        # api is 1000, but such a large request can cause 504 errors. See:
+        # https://github.com/VingtCinq/python-mailchimp/pull/207
+        count = queryparams.pop("count", 500)
+        result = self._mc_client._get(url=url, offset=0, count=count, **queryparams)
         total = result['total_items']
         # Fetch further results if necessary
-        if total > 1000:
-            for offset in range(1, int(total / 1000) + 1):
+        if total > count:
+            for offset in range(1, int(total / count) + 1):
                 result = merge_results(result, self._mc_client._get(
                     url=url,
-                    offset=int(offset * 1000),
-                    count=1000,
+                    offset=int(offset * count),
+                    count=count,
                     **queryparams
                 ))
             return result
         else:  # Further results not necessary
             return result
```

### Comparing `mailchimp3-3.0.7/mailchimp3/__init__.py` & `mailchimp3-3.0.9/mailchimp3/__init__.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/mailchimpclient.py` & `mailchimp3-3.0.9/mailchimp3/mailchimpclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,23 @@
     return wrapper
 
 
 class MailChimpError(Exception):
     pass
 
 
+def _raise_response_error(r):
+    # in case of a 500 error, the response might not be a JSON
+    try:
+        error_data = r.json()
+    except ValueError:
+        error_data = { "response": r }
+    raise MailChimpError(error_data)
+
+
 class MailChimpClient(object):
     """
     MailChimp class to communicate with the v3 API
     """
     def __init__(self, mc_api=None, mc_user='python-mailchimp', access_token=None, enabled=True, timeout=None,
                  request_hooks=None, request_headers=None):
         """
@@ -119,20 +128,16 @@
                 hooks=self.request_hooks,
                 headers=self.request_headers
             ))
         except requests.exceptions.RequestException as e:
             raise e
         else:
             if r.status_code >= 400:
-                # in case of a 500 error, the response might not be a JSON
-                try:
-                    error_data = r.json()
-                except ValueError:
-                    error_data = { "response": r }
-                raise MailChimpError(error_data)
+                _raise_response_error(r)
+
             if r.status_code == 204:
                 return None
             return r.json()
 
 
     @_enabled_or_noop
     def _get(self, url, **queryparams):
@@ -156,15 +161,15 @@
                 hooks=self.request_hooks,
                 headers=self.request_headers
             ))
         except requests.exceptions.RequestException as e:
             raise e
         else:
             if r.status_code >= 400:
-                raise MailChimpError(r.json())
+                _raise_response_error(r)
             return r.json()
 
 
     @_enabled_or_noop
     def _delete(self, url):
         """
         Handle authenticated DELETE requests
@@ -183,15 +188,15 @@
                 hooks=self.request_hooks,
                 headers=self.request_headers
             ))
         except requests.exceptions.RequestException as e:
             raise e
         else:
             if r.status_code >= 400:
-                raise MailChimpError(r.json())
+                _raise_response_error(r)
             if r.status_code == 204:
                 return
             return r.json()
 
 
     @_enabled_or_noop
     def _patch(self, url, data=None):
@@ -215,15 +220,15 @@
                 hooks=self.request_hooks,
                 headers=self.request_headers
             ))
         except requests.exceptions.RequestException as e:
             raise e
         else:
             if r.status_code >= 400:
-                raise MailChimpError(r.json())
+                _raise_response_error(r)
             return r.json()
 
 
     @_enabled_or_noop
     def _put(self, url, data=None):
         """
         Handle authenticated PUT requests
@@ -245,20 +250,15 @@
                 hooks=self.request_hooks,
                 headers=self.request_headers
             ))
         except requests.exceptions.RequestException as e:
             raise e
         else:
             if r.status_code >= 400:
-                # in case of 500 error, the response might not be a JSON
-                try:
-                    error_data = r.json()
-                except ValueError:
-                    error_data = { "response": r }
-                raise MailChimpError(error_data)
+                _raise_response_error(r)
             return r.json()
 
 
 class MailChimpOAuth(requests.auth.AuthBase):
     """
     Authentication class for authentication with OAuth2. Acquiring an OAuth2
     for MailChimp can be done by following the instructions in the
```

### Comparing `mailchimp3-3.0.7/mailchimp3/helpers.py` & `mailchimp3-3.0.9/mailchimp3/helpers.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportsubreports.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportsubreports.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/searchmembers.py` & `mailchimp3-3.0.9/mailchimp3/entities/searchmembers.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listmembernotes.py` & `mailchimp3-3.0.9/mailchimp3/entities/listmembernotes.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportcampaignabusereports.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportcampaignabusereports.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listinterestcategories.py` & `mailchimp3-3.0.9/mailchimp3/entities/listinterestcategories.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/lists.py` & `mailchimp3-3.0.9/mailchimp3/entities/lists.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/storecustomers.py` & `mailchimp3-3.0.9/mailchimp3/entities/storecustomers.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listabusereports.py` & `mailchimp3-3.0.9/mailchimp3/entities/listabusereports.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/campaigncontent.py` & `mailchimp3-3.0.9/mailchimp3/entities/campaigncontent.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listmembergoals.py` & `mailchimp3-3.0.9/mailchimp3/entities/listmembergoals.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/automationactions.py` & `mailchimp3-3.0.9/mailchimp3/entities/automationactions.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/campaignfeedback.py` & `mailchimp3-3.0.9/mailchimp3/entities/campaignfeedback.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/automationemailactions.py` & `mailchimp3-3.0.9/mailchimp3/entities/automationemailactions.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listmembertags.py` & `mailchimp3-3.0.9/mailchimp3/entities/listmembertags.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/storeproductvariants.py` & `mailchimp3-3.0.9/mailchimp3/entities/storeproductvariants.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportlocations.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportlocations.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/segments.py` & `mailchimp3-3.0.9/mailchimp3/entities/segments.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listinterestcategoryinterest.py` & `mailchimp3-3.0.9/mailchimp3/entities/listinterestcategoryinterest.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listactivity.py` & `mailchimp3-3.0.9/mailchimp3/entities/listactivity.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listmergefields.py` & `mailchimp3-3.0.9/mailchimp3/entities/listmergefields.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listsignupforms.py` & `mailchimp3-3.0.9/mailchimp3/entities/listsignupforms.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportclickdetailreports.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportclickdetailreports.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listsegmentmembers.py` & `mailchimp3-3.0.9/mailchimp3/entities/listsegmentmembers.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/automationemails.py` & `mailchimp3-3.0.9/mailchimp3/entities/automationemails.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/stores.py` & `mailchimp3-3.0.9/mailchimp3/entities/stores.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/searchcampaigns.py` & `mailchimp3-3.0.9/mailchimp3/entities/searchcampaigns.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/campaignfolders.py` & `mailchimp3-3.0.9/mailchimp3/entities/campaignfolders.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportcampaignadvice.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportcampaignadvice.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/authorizedapps.py` & `mailchimp3-3.0.9/mailchimp3/entities/authorizedapps.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/storeproducts.py` & `mailchimp3-3.0.9/mailchimp3/entities/storeproducts.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listsegments.py` & `mailchimp3-3.0.9/mailchimp3/entities/listsegments.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportsentto.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportsentto.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/automationremovedsubscribers.py` & `mailchimp3-3.0.9/mailchimp3/entities/automationremovedsubscribers.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listmembers.py` & `mailchimp3-3.0.9/mailchimp3/entities/listmembers.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/campaigns.py` & `mailchimp3-3.0.9/mailchimp3/entities/campaigns.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/batchwebhooks.py` & `mailchimp3-3.0.9/mailchimp3/entities/batchwebhooks.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/filemanagerfolders.py` & `mailchimp3-3.0.9/mailchimp3/entities/filemanagerfolders.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/storecartlines.py` & `mailchimp3-3.0.9/mailchimp3/entities/storecartlines.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/templates.py` & `mailchimp3-3.0.9/mailchimp3/entities/templates.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportemailactivity.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportemailactivity.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/storeorderlines.py` & `mailchimp3-3.0.9/mailchimp3/entities/storeorderlines.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/conversationmessages.py` & `mailchimp3-3.0.9/mailchimp3/entities/conversationmessages.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/automations.py` & `mailchimp3-3.0.9/mailchimp3/entities/automations.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/filemanagerfiles.py` & `mailchimp3-3.0.9/mailchimp3/entities/filemanagerfiles.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/batchoperations.py` & `mailchimp3-3.0.9/mailchimp3/entities/batchoperations.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportopendetails.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportopendetails.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reports.py` & `mailchimp3-3.0.9/mailchimp3/entities/reports.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listgrowthhistory.py` & `mailchimp3-3.0.9/mailchimp3/entities/listgrowthhistory.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reporteepurl.py` & `mailchimp3-3.0.9/mailchimp3/entities/reporteepurl.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/storecarts.py` & `mailchimp3-3.0.9/mailchimp3/entities/storecarts.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/automationemailqueues.py` & `mailchimp3-3.0.9/mailchimp3/entities/automationemailqueues.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportgoogleanalytics.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportgoogleanalytics.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/campaignsendchecklist.py` & `mailchimp3-3.0.9/mailchimp3/entities/campaignsendchecklist.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/root.py` & `mailchimp3-3.0.9/mailchimp3/entities/root.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/templatedefaultcontent.py` & `mailchimp3-3.0.9/mailchimp3/entities/templatedefaultcontent.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/storeorders.py` & `mailchimp3-3.0.9/mailchimp3/entities/storeorders.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/storepromorules.py` & `mailchimp3-3.0.9/mailchimp3/entities/storepromorules.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/campaignactions.py` & `mailchimp3-3.0.9/mailchimp3/entities/campaignactions.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/templatefolders.py` & `mailchimp3-3.0.9/mailchimp3/entities/templatefolders.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/storeproductimages.py` & `mailchimp3-3.0.9/mailchimp3/entities/storeproductimages.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportunsubscribes.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportunsubscribes.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listclients.py` & `mailchimp3-3.0.9/mailchimp3/entities/listclients.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/conversations.py` & `mailchimp3-3.0.9/mailchimp3/entities/conversations.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportclickdetailmembers.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportclickdetailmembers.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listmemberactivity.py` & `mailchimp3-3.0.9/mailchimp3/entities/listmemberactivity.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/storepromocodes.py` & `mailchimp3-3.0.9/mailchimp3/entities/storepromocodes.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/listwebhooks.py` & `mailchimp3-3.0.9/mailchimp3/entities/listwebhooks.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/ping.py` & `mailchimp3-3.0.9/mailchimp3/entities/ping.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/mailchimp3/entities/reportdomainperformance.py` & `mailchimp3-3.0.9/mailchimp3/entities/reportdomainperformance.py`

 * *Files identical despite different names*

### Comparing `mailchimp3-3.0.7/README.rst` & `mailchimp3-3.0.9/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-|mailchimp3 v3.0.7 on PyPi| |MIT license| |Stable|
+|mailchimp3 v3.0.9 on PyPi| |MIT license| |Stable|
 
 python-mailchimp-api
 ====================
 
 A straighforward python client for v3 of MailChimp API using requests >=
 2.7.0.
 
@@ -48,17 +48,17 @@
 
 Grab ``YOUR_API_KEY`` from your mailchimp account (Account > Extra > Api
 Keys). ``YOUR_USERNAME`` is the one you use to login on the website and
 is optional.
 
 ::
 
-    from mailchimp3 import MailChimp
+   from mailchimp3 import MailChimp
 
-    client = MailChimp(mc_api='YOUR_API_KEY', mc_user='YOUR_USERNAME')
+   client = MailChimp(mc_api='YOUR_API_KEY', mc_user='YOUR_USERNAME')
 
 OAuth Support
 ~~~~~~~~~~~~~
 
 In addition to HTTP Basic Authentication, MailChimp supports
 authentication through OAuth2. Information on obtaining the proper
 access key can be found
@@ -72,160 +72,162 @@
 skip. For endpoints that allow the pagination parameters, the all()
 method has an additional boolean ``get_all`` argument that will loop
 through all records until the API no longer returns any to get all
 records without manually performing an additional query. By default,
 count is 10 and offset is 0 for all endpoints that support it. The
 ``get_all`` parameter on the all() method on any endpoint defaults to
 false, which follows the values that are provided in the call, and using
-``get_all=True`` will ignore the provided count and offset to ensure
-that all records are returned. When using get_all, the count will be
-5000, to fetch large numbers of records without flooding the system with
-requests. The large size of count should not impact calls which are
+``get_all=True`` will ignore the provided offset to ensure that all
+records are returned. When using get_all, the count will be 500 unless
+otherwise specified. It is strongly recommended to avoid small values
+for ``count`` to fetch large numbers of records because this will flood
+the system. A large ``count`` size should not impact calls which are
 expected to return a very small number of records, and should improve
-performance for calls where fetching 5000 records would only provide a
+performance for calls where fetching 500 records would only provide a
 fraction by preventing the delay of making a huge number of requests.
 
 ::
 
-    client.lists.members.all('123456', count=100, offset=0)
+   client.lists.members.all('123456', count=100, offset=0)
 
 Fields
 ~~~~~~
 
 Many endpoints allow you to select which fields will be returned out of
 all available fields (for example, only the email_address of a member).
 Simply add ``fields`` arguments in your function. The following only
 display email_address and id for each member in list 123456:
 
 ::
 
-    client.lists.members.all('123456', get_all=True, fields="members.email_address,members.id")
+   client.lists.members.all('123456', get_all=True, fields="members.email_address,members.id")
 
 Examples
 ~~~~~~~~
 
 ::
 
-    # returns all the lists (only name and id)
-    client.lists.all(get_all=True, fields="lists.name,lists.id")
+   # returns all the lists (only name and id)
+   client.lists.all(get_all=True, fields="lists.name,lists.id")
 
-    # returns all members inside list '123456'
-    client.lists.members.all('123456', get_all=True)
+   # returns all members inside list '123456'
+   client.lists.members.all('123456', get_all=True)
 
-    # return the first 100 member's email addresses for the list with id 123456
-    client.lists.members.all('123456', count=100, offset=0, fields="members.email_address")
+   # return the first 100 member's email addresses for the list with id 123456
+   client.lists.members.all('123456', count=100, offset=0, fields="members.email_address")
 
-    # returns the list matching id '123456'
-    client.lists.get('123456')
-
-    # add John Doe with email john.doe@example.com to list matching id '123456'
-    client.lists.members.create('123456', {
-        'email_address': 'john.doe@example.com',
-        'status': 'subscribed',
-        'merge_fields': {
-            'FNAME': 'John',
-            'LNAME': 'Doe',
-        },
-    })
-
-    # returns all the campaigns
-    client.campaigns.all(get_all=True)
-
-    # You can also disable at runtime with the optional ``enabled`` parameter.
-    # Every API call will return None
-    client = MailChimp('YOUR SECRET KEY', enabled=False)
-
-    # You are encouraged to specify a value in seconds for the ``timeout``
-    # parameter to avoid hanging requests.
-    client = MailChimp('YOUR SECRET KEY', timeout=10.0)
-
-    # You are encouraged to specify a User-Agent for requests to the MailChimp
-    # API. Headers can be specified using the ``request_headers`` parameter.
-    headers = requests.utils.default_headers()
-    headers['User-Agent'] = 'Example (example@example.com)'
-    client = MailChimp('YOUR SECRET KEY', request_headers=headers)
+   # returns the list matching id '123456'
+   client.lists.get('123456')
+
+   # add John Doe with email john.doe@example.com to list matching id '123456'
+   client.lists.members.create('123456', {
+       'email_address': 'john.doe@example.com',
+       'status': 'subscribed',
+       'merge_fields': {
+           'FNAME': 'John',
+           'LNAME': 'Doe',
+       },
+   })
+
+   # returns all the campaigns
+   client.campaigns.all(get_all=True)
+
+   # You can also disable at runtime with the optional ``enabled`` parameter.
+   # Every API call will return None
+   client = MailChimp('YOUR SECRET KEY', enabled=False)
+
+   # You are encouraged to specify a value in seconds for the ``timeout``
+   # parameter to avoid hanging requests.
+   client = MailChimp('YOUR SECRET KEY', timeout=10.0)
+
+   # You are encouraged to specify a User-Agent for requests to the MailChimp
+   # API. Headers can be specified using the ``request_headers`` parameter.
+   headers = requests.utils.default_headers()
+   headers['User-Agent'] = 'Example (example@example.com)'
+   client = MailChimp('YOUR SECRET KEY', request_headers=headers)
 
 API Structure
 -------------
 
 All endpoints follow the structure listed in the official MailChimp API
 v3 documentation. The structure will be listed below and then the
 individual methods available after.
 
 ::
 
-    MailChimp
-    +- Root
-    +- Authorized Apps
-    +- Automations
-    |  +- Actions
-    |  +- Emails
-    |  |  +- Actions
-    |  |  +- Queues
-    |  +- Removed Subscribers
-    +- Batch Operations
-    +- Batch Webhooks
-    +- Campaign Folders
-    +- Campaigns
-    |  +- Actions
-    |  +- Content
-    |  +- Feedback
-    |  +- Send Checklist
-    +- Conversations
-    |  +- Messages
-    +- Stores
-    |  +- Carts
-    |  |  +- Lines
-    |  +- Customers
-    |  +- Orders
-    |  |  +- Lines
-    |  +- Products
-    |     +- Images
-    |     +- Variants
-    |  +- Promo Rules
-    |     +- Promo Codes
-    +- File Manager Files
-    +- File Manager Folders
-    +- Lists
-    |  +- Abuse Reports
-    |  +- Activity
-    |  +- Clients
-    |  +- Growth History
-    |  +- Interest Categories
-    |  |  +- Interests
-    |  +- Members
-    |  |  +- Activity
-    |  |  +- Goals
-    |  |  +- Notes
-    |  +- Merge Fields
-    |  +- Segments
-    |  |  +- Segment Members
-    |  +- Signup Forms
-    |  +- Twitter Lead Generation Carts
-    |  +- Webhooks
-    +- Ping
-    +- Reports
-    |  +- Campaign Abuse
-    |  +- Campaign Advice
-    |  +- Campaign Open reports
-    |  +- Click Reports
-    |  |  +- Members
-    |  +- Domain Performance
-    |  +- EepURL Reports
-    |  +- Email Activity
-    |  +- Google Analytics
-    |  +- Location
-    |  +- Sent To
-    |  +- Sub-Reports
-    |  +- Unsubscribes
-    +- Seach Campaigns
-    +- Search Members
-    +- Template Folders
-    +- Templates
-       +- Default Content
+   MailChimp
+   +- Root
+   +- Authorized Apps
+   +- Automations
+   |  +- Actions
+   |  +- Emails
+   |  |  +- Actions
+   |  |  +- Queues
+   |  +- Removed Subscribers
+   +- Batch Operations
+   +- Batch Webhooks
+   +- Campaign Folders
+   +- Campaigns
+   |  +- Actions
+   |  +- Content
+   |  +- Feedback
+   |  +- Send Checklist
+   +- Conversations
+   |  +- Messages
+   +- Stores
+   |  +- Carts
+   |  |  +- Lines
+   |  +- Customers
+   |  +- Orders
+   |  |  +- Lines
+   |  +- Products
+   |     +- Images
+   |     +- Variants
+   |  +- Promo Rules
+   |     +- Promo Codes
+   +- File Manager Files
+   +- File Manager Folders
+   +- Lists
+   |  +- Abuse Reports
+   |  +- Activity
+   |  +- Clients
+   |  +- Growth History
+   |  +- Interest Categories
+   |  |  +- Interests
+   |  +- Members
+   |  |  +- Activity
+   |  |  +- Goals
+   |  |  +- Notes
+   |  |  +- Tags
+   |  +- Merge Fields
+   |  +- Segments
+   |  |  +- Segment Members
+   |  +- Signup Forms
+   |  +- Twitter Lead Generation Carts
+   |  +- Webhooks
+   +- Ping
+   +- Reports
+   |  +- Campaign Abuse
+   |  +- Campaign Advice
+   |  +- Campaign Open reports
+   |  +- Click Reports
+   |  |  +- Members
+   |  +- Domain Performance
+   |  +- EepURL Reports
+   |  +- Email Activity
+   |  +- Google Analytics
+   |  +- Location
+   |  +- Sent To
+   |  +- Sub-Reports
+   |  +- Unsubscribes
+   +- Seach Campaigns
+   +- Search Members
+   +- Template Folders
+   +- Templates
+      +- Default Content
 
 API Endpoints
 -------------
 
 Below is the list of all endpoints and the methods that can be called
 against them. Any endpoint that has a method that takes an ID argument
 (for example the app_id in the authorized_apps endpoint or the
@@ -244,679 +246,687 @@
 .. _root-1:
 
 Root
 ^^^^
 
 ::
 
-    client.root.get()
+   client.root.get()
 
 Authorized Apps
 ~~~~~~~~~~~~~~~
 
 .. _authorized-apps-1:
 
 Authorized Apps
 ^^^^^^^^^^^^^^^
 
 ::
 
-    client.authorized_apps.create(data={})
-    client.authorized_apps.all(get_all=False)
-    client.authorized_apps.get(app_id='')
+   client.authorized_apps.create(data={})
+   client.authorized_apps.all(get_all=False)
+   client.authorized_apps.get(app_id='')
 
 Automations
 ~~~~~~~~~~~
 
 .. _automations-1:
 
 Automations
 ^^^^^^^^^^^
 
 ::
 
-    client.automations.all(get_all=False)
-    client.automations.get(workflow_id='')
+   client.automations.all(get_all=False)
+   client.automations.get(workflow_id='')
 
 Automation Actions
 ^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.automations.actions.pause(workflow_id='')
-    client.automations.actions.start(workflow_id='')
+   client.automations.actions.pause(workflow_id='')
+   client.automations.actions.start(workflow_id='')
 
 Automation Emails
 ^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.automations.emails.all(workflow_id='')
-    client.automations.emails.get(workflow_id='', email_id='')
+   client.automations.emails.all(workflow_id='')
+   client.automations.emails.get(workflow_id='', email_id='')
 
 Automation Email Actions
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.automations.emails.actions.pause(workflow_id='', email_id='')
-    client.automations.emails.actions.start(workflow_id='', email_id='')
+   client.automations.emails.actions.pause(workflow_id='', email_id='')
+   client.automations.emails.actions.start(workflow_id='', email_id='')
 
 Automation Email Queues
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.automations.emails.queues.create(workflow_id='', email_id='', data={})
-    client.automations.emails.queues.all(workflow_id='', email_id='')
-    client.automations.emails.queues.get(workflow_id='', email_id='', subscriber_hash='')
+   client.automations.emails.queues.create(workflow_id='', email_id='', data={})
+   client.automations.emails.queues.all(workflow_id='', email_id='')
+   client.automations.emails.queues.get(workflow_id='', email_id='', subscriber_hash='')
 
 Automation Removed Subscribers
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.automations.removed_subscribers.create(workflow_id='', data={})
-    client.automations.removed_subscribers.all(workflow_id='')
+   client.automations.removed_subscribers.create(workflow_id='', data={})
+   client.automations.removed_subscribers.all(workflow_id='')
 
 Batch Operations
 ~~~~~~~~~~~~~~~~
 
 .. _batch-operations-1:
 
 Batch Operations
 ^^^^^^^^^^^^^^^^
 
 ::
 
-    client.batch_operations.create(data={})
-    client.batch_operations.all(get_all=False)
-    client.batch_operations.get(batch_id='')
-    client.batch_operations.delete(batch_id='')
+   client.batch_operations.create(data={})
+   client.batch_operations.all(get_all=False)
+   client.batch_operations.get(batch_id='')
+   client.batch_operations.delete(batch_id='')
 
 Batch Webhooks
 ~~~~~~~~~~~~~~
 
 .. _batch-webhooks-1:
 
 Batch Webhooks
 ^^^^^^^^^^^^^^
 
 ::
 
-    client.batch_webhooks.create(data={})
-    client.batch_webhooks.all(get_all=False)
-    client.batch_webhooks.get(batch_webhook_id='')
-    client.batch_webhooks.update(batch_webhook_id='', data={})
-    client.batch_webhooks.delete(batch_webhook_id='')
+   client.batch_webhooks.create(data={})
+   client.batch_webhooks.all(get_all=False)
+   client.batch_webhooks.get(batch_webhook_id='')
+   client.batch_webhooks.update(batch_webhook_id='', data={})
+   client.batch_webhooks.delete(batch_webhook_id='')
 
 Campaigns
 ~~~~~~~~~
 
 Folders
 ^^^^^^^
 
 ::
 
-    client.campaign_folders.create(data={})
-    client.campaign_folders.all(get_all=False)
-    client.campaign_folders.get(folder_id='')
-    client.campaign_folders.update(folder_id='', data={})
-    client.campaign_folders.delete(folder_id='')
+   client.campaign_folders.create(data={})
+   client.campaign_folders.all(get_all=False)
+   client.campaign_folders.get(folder_id='')
+   client.campaign_folders.update(folder_id='', data={})
+   client.campaign_folders.delete(folder_id='')
 
 .. _campaigns-1:
 
 Campaigns
 ^^^^^^^^^
 
 ::
 
-    client.campaigns.create(data={})
-    client.campaigns.all(get_all=False)
-    client.campaigns.get(campaign_id='')
-    client.campaigns.update(campaign_id='')
-    client.campaigns.delete(campaign_id='')
+   client.campaigns.create(data={})
+   client.campaigns.all(get_all=False)
+   client.campaigns.get(campaign_id='')
+   client.campaigns.update(campaign_id='')
+   client.campaigns.delete(campaign_id='')
 
 Campaign Actions
 ^^^^^^^^^^^^^^^^
 
 ::
 
-    client.campaigns.actions.cancel(campaign_id='')
-    client.campaigns.actions.pause(campaign_id='')
-    client.campaigns.actions.replicate(campaign_id='')
-    client.campaigns.actions.resume(campaign_id='')
-    client.campaigns.actions.schedule(campaign_id='', data={})
-    client.campaigns.actions.send(campaign_id='')
-    client.campaigns.actions.test(campaign_id='', data={})
-    client.campaigns.actions.unschedule(campaign_id='')
+   client.campaigns.actions.cancel(campaign_id='')
+   client.campaigns.actions.pause(campaign_id='')
+   client.campaigns.actions.replicate(campaign_id='')
+   client.campaigns.actions.resume(campaign_id='')
+   client.campaigns.actions.schedule(campaign_id='', data={})
+   client.campaigns.actions.send(campaign_id='')
+   client.campaigns.actions.test(campaign_id='', data={})
+   client.campaigns.actions.unschedule(campaign_id='')
 
 Campaign Content
 ^^^^^^^^^^^^^^^^
 
 ::
 
-    client.campaigns.content.get(campaign_id='')
-    client.campaigns.content.update(campaign_id='', data={})
+   client.campaigns.content.get(campaign_id='')
+   client.campaigns.content.update(campaign_id='', data={})
 
 Campaign Feedback
 ^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.campaigns.feedback.create(campaign_id='', data={})
-    client.campaigns.feedback.all(campaign_id='', get_all=False)
-    client.campaigns.feedback.get(campaign_id='', feedback_id='')
-    client.campaigns.feedback.update(campaign_id='', feedback_id='', data={})
-    client.campaigns.feedback.delete(campaign_id='', feedback_id='')
+   client.campaigns.feedback.create(campaign_id='', data={})
+   client.campaigns.feedback.all(campaign_id='', get_all=False)
+   client.campaigns.feedback.get(campaign_id='', feedback_id='')
+   client.campaigns.feedback.update(campaign_id='', feedback_id='', data={})
+   client.campaigns.feedback.delete(campaign_id='', feedback_id='')
 
 Campaign Send Checklist
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.campaigns.send_checklist.get(campaign_id='')
+   client.campaigns.send_checklist.get(campaign_id='')
 
 Conversations
 ~~~~~~~~~~~~~
 
 .. _conversations-1:
 
 Conversations
 ^^^^^^^^^^^^^
 
 ::
 
-    client.conversations.all(get_all=False)
-    client.conversations.get(conversation_id='')
+   client.conversations.all(get_all=False)
+   client.conversations.get(conversation_id='')
 
 Conversation Messages
 ^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.conversations.messages.create(conversation_id='', data={})
-    client.conversations.messages.all(conversation_id='')
-    client.conversations.messages.get(conversation_id='', message_id='')
+   client.conversations.messages.create(conversation_id='', data={})
+   client.conversations.messages.all(conversation_id='')
+   client.conversations.messages.get(conversation_id='', message_id='')
 
 E-Commerce
 ~~~~~~~~~~
 
 Stores
 ^^^^^^
 
 ::
 
-    client.stores.create(data={})
-    client.stores.all(get_all=False)
-    client.stores.get(store_id='')
-    client.stores.update(store_id='', data={})
-    client.stores.delete(store_id='')
+   client.stores.create(data={})
+   client.stores.all(get_all=False)
+   client.stores.get(store_id='')
+   client.stores.update(store_id='', data={})
+   client.stores.delete(store_id='')
 
 Store Carts
 ^^^^^^^^^^^
 
 ::
 
-    client.stores.carts.create(store_id='', data={})
-    client.stores.carts.all(store_id='', get_all=False)
-    client.stores.carts.get(store_id='', cart_id='')
-    client.stores.carts.update(store_id='', cart_id='', data={})
-    client.stores.carts.delete(store_id='', cart_id='')
+   client.stores.carts.create(store_id='', data={})
+   client.stores.carts.all(store_id='', get_all=False)
+   client.stores.carts.get(store_id='', cart_id='')
+   client.stores.carts.update(store_id='', cart_id='', data={})
+   client.stores.carts.delete(store_id='', cart_id='')
 
 Store Cart Lines
 ^^^^^^^^^^^^^^^^
 
 ::
 
-    client.stores.carts.lines.create(store_id='', cart_id='', data={})
-    client.stores.carts.lines.all(store_id='', cart_id='', get_all=False)
-    client.stores.carts.lines.get(store_id='', cart_id='', line_id='')
-    client.stores.carts.lines.update(store_id='', cart_id='', line_id='', data={})
-    client.stores.carts.lines.delete(store_id='', cart_id='', line_id='')
+   client.stores.carts.lines.create(store_id='', cart_id='', data={})
+   client.stores.carts.lines.all(store_id='', cart_id='', get_all=False)
+   client.stores.carts.lines.get(store_id='', cart_id='', line_id='')
+   client.stores.carts.lines.update(store_id='', cart_id='', line_id='', data={})
+   client.stores.carts.lines.delete(store_id='', cart_id='', line_id='')
 
 Store Customers
 ^^^^^^^^^^^^^^^
 
 ::
 
-    client.stores.customers.create(store_id='', data={})
-    client.stores.customers.all(store_id='', get_all=False)
-    client.stores.customers.get(store_id='', customer_id='')
-    client.stores.customers.update(store_id='', customer_id='', data={})
-    client.stores.customers.create_or_update(store_id='', customer_id='', data={})
-    client.stores.customers.delete(store_id='', customer_id='')
+   client.stores.customers.create(store_id='', data={})
+   client.stores.customers.all(store_id='', get_all=False)
+   client.stores.customers.get(store_id='', customer_id='')
+   client.stores.customers.update(store_id='', customer_id='', data={})
+   client.stores.customers.create_or_update(store_id='', customer_id='', data={})
+   client.stores.customers.delete(store_id='', customer_id='')
 
 Store Orders
 ^^^^^^^^^^^^
 
 ::
 
-    client.stores.orders.create(store_id='', data={})
-    client.stores.orders.all(store_id='', get_all=False)
-    client.stores.orders.get(store_id='', order_id='')
-    client.stores.orders.update(store_id='', order_id='', data={})
-    client.stores.orders.delete(store_id='', order_id='')
+   client.stores.orders.create(store_id='', data={})
+   client.stores.orders.all(store_id='', get_all=False)
+   client.stores.orders.get(store_id='', order_id='')
+   client.stores.orders.update(store_id='', order_id='', data={})
+   client.stores.orders.delete(store_id='', order_id='')
 
 Store Order Lines
 ^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.stores.orders.lines.create(store_id='', order_id='', data={})
-    client.stores.orders.lines.all(store_id='', order_id='', get_all=False)
-    client.stores.orders.lines.get(store_id='', order_id='', line_id='')
-    client.stores.orders.lines.update(store_id='', order_id='', line_id='', data={})
-    client.stores.orders.lines.delete(store_id='', order_id='', line_id='')
+   client.stores.orders.lines.create(store_id='', order_id='', data={})
+   client.stores.orders.lines.all(store_id='', order_id='', get_all=False)
+   client.stores.orders.lines.get(store_id='', order_id='', line_id='')
+   client.stores.orders.lines.update(store_id='', order_id='', line_id='', data={})
+   client.stores.orders.lines.delete(store_id='', order_id='', line_id='')
 
 Store Products
 ^^^^^^^^^^^^^^
 
 ::
 
-    client.stores.products.create(store_id='', data={})
-    client.stores.products.all(store_id='', get_all=False)
-    client.stores.products.get(store_id='', product_id='')
-    client.stores.products.update(store_id='', product_id='')
-    client.stores.products.delete(store_id='', product_id='')
+   client.stores.products.create(store_id='', data={})
+   client.stores.products.all(store_id='', get_all=False)
+   client.stores.products.get(store_id='', product_id='')
+   client.stores.products.update(store_id='', product_id='')
+   client.stores.products.delete(store_id='', product_id='')
 
 Store Product Images
 ^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.stores.products.images.create(store_id='', product_id='', data={})
-    client.stores.products.images.all(store_id='', product_id='', get_all=False)
-    client.stores.products.images.get(store_id='', product_id='', image_id='')
-    client.stores.products.images.update(store_id='', product_id='', image_id='', data={})
-    client.stores.products.images.delete(store_id='', product_id='', image_id='')
+   client.stores.products.images.create(store_id='', product_id='', data={})
+   client.stores.products.images.all(store_id='', product_id='', get_all=False)
+   client.stores.products.images.get(store_id='', product_id='', image_id='')
+   client.stores.products.images.update(store_id='', product_id='', image_id='', data={})
+   client.stores.products.images.delete(store_id='', product_id='', image_id='')
 
 Store Product Variants
 ^^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.stores.products.variants.create(store_id='', product_id='', data={})
-    client.stores.products.variants.all(store_id='', product_id='', get_all=False)
-    client.stores.products.variants.get(store_id='', product_id='', variant_id='')
-    client.stores.products.variants.update(store_id='', product_id='', variant_id='', data={})
-    client.stores.products.variants.create_or_update(store_id='', product_id='', variant_id='', data={})
-    client.stores.products.variants.delete(store_id='', product_id='', variant_id='')
+   client.stores.products.variants.create(store_id='', product_id='', data={})
+   client.stores.products.variants.all(store_id='', product_id='', get_all=False)
+   client.stores.products.variants.get(store_id='', product_id='', variant_id='')
+   client.stores.products.variants.update(store_id='', product_id='', variant_id='', data={})
+   client.stores.products.variants.create_or_update(store_id='', product_id='', variant_id='', data={})
+   client.stores.products.variants.delete(store_id='', product_id='', variant_id='')
 
 File Manager
 ~~~~~~~~~~~~
 
 Files
 ^^^^^
 
 ::
 
-    client.files.create(data={})
-    client.files.all(get_all=False)
-    client.files.get(file_id='')
-    client.files.update(file_id='', data={})
-    client.files.delete(file_id='')
+   client.files.create(data={})
+   client.files.all(get_all=False)
+   client.files.get(file_id='')
+   client.files.update(file_id='', data={})
+   client.files.delete(file_id='')
 
 .. _folders-1:
 
 Folders
 ^^^^^^^
 
 ::
 
-    client.folders.create(data={})
-    client.folders.all(get_all=False)
-    client.folders.get(folder_id='')
-    client.folders.update(folder_id='', data={})
-    client.folders.delete(folder_id='')
+   client.folders.create(data={})
+   client.folders.all(get_all=False)
+   client.folders.get(folder_id='')
+   client.folders.update(folder_id='', data={})
+   client.folders.delete(folder_id='')
 
 Lists
 ~~~~~
 
 .. _lists-1:
 
 Lists
 ^^^^^
 
 ::
 
-    client.lists.create(data={})
-    client.lists.update_members(list_id='', data={})
-    client.lists.all(get_all=False)
-    client.lists.get(list_id='')
-    client.lists.update(list_id='', data={})
-    client.lists.delete(list_id='')
+   client.lists.create(data={})
+   client.lists.update_members(list_id='', data={})
+   client.lists.all(get_all=False)
+   client.lists.get(list_id='')
+   client.lists.update(list_id='', data={})
+   client.lists.delete(list_id='')
 
 List Abuse Reports
 ^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.lists.abuse_reports.all(list_id='', get_all=False)
-    client.lists.abuse_reports.get(list_id='', report_id='')
+   client.lists.abuse_reports.all(list_id='', get_all=False)
+   client.lists.abuse_reports.get(list_id='', report_id='')
 
 List Activity
 ^^^^^^^^^^^^^
 
 ::
 
-    client.lists.activity.all(list_id='')
+   client.lists.activity.all(list_id='')
 
 List Clients
 ^^^^^^^^^^^^
 
 ::
 
-    client.lists.clients.all(list_id='')
+   client.lists.clients.all(list_id='')
 
 List Growth History
 ^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.lists.growth_history.all(list_id='', get_all=False)
-    client.lists.growth_history.get(list_id='', month='')
+   client.lists.growth_history.all(list_id='', get_all=False)
+   client.lists.growth_history.get(list_id='', month='')
 
 List Interest Categories
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.lists.interest_categories.create(list_id='', data={})
-    client.lists.interest_categories.all(list_id='', get_all=False)
-    client.lists.interest_categories.get(list_id='', category_id='')
-    client.lists.interest_categories.update(list_id='', category_id='', data={})
-    client.lists.interest_categories.delete(list_id='', category_id='')
+   client.lists.interest_categories.create(list_id='', data={})
+   client.lists.interest_categories.all(list_id='', get_all=False)
+   client.lists.interest_categories.get(list_id='', category_id='')
+   client.lists.interest_categories.update(list_id='', category_id='', data={})
+   client.lists.interest_categories.delete(list_id='', category_id='')
 
 List Interest Category Interests
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.lists.interest_categories.interests.create(list_id='', category_id='', data={})
-    client.lists.interest_categories.interests.all(list_id='', category_id='', get_all=False)
-    client.lists.interest_categories.interests.get(list_id='', category_id='', interest_id='')
-    client.lists.interest_categories.interests.update(list_id='', category_id='', interest_id='', data={})
-    client.lists.interest_categories.interests.delete(list_id='', category_id='', interest_id='')
+   client.lists.interest_categories.interests.create(list_id='', category_id='', data={})
+   client.lists.interest_categories.interests.all(list_id='', category_id='', get_all=False)
+   client.lists.interest_categories.interests.get(list_id='', category_id='', interest_id='')
+   client.lists.interest_categories.interests.update(list_id='', category_id='', interest_id='', data={})
+   client.lists.interest_categories.interests.delete(list_id='', category_id='', interest_id='')
 
 List Members
 ^^^^^^^^^^^^
 
 ::
 
-    client.lists.members.create(list_id='', data={})
-    client.lists.members.all(list_id='', get_all=False)
-    client.lists.members.get(list_id='', subscriber_hash='')
-    client.lists.members.update(list_id='', subscriber_hash='', data={})
-    client.lists.members.create_or_update(list_id='', subscriber_hash='', data={})
-    client.lists.members.delete(list_id='', subscriber_hash='')
-    client.lists.members.delete_permanent(list_id='', subscriber_hash='')
+   client.lists.members.create(list_id='', data={})
+   client.lists.members.all(list_id='', get_all=False)
+   client.lists.members.get(list_id='', subscriber_hash='')
+   client.lists.members.update(list_id='', subscriber_hash='', data={})
+   client.lists.members.create_or_update(list_id='', subscriber_hash='', data={})
+   client.lists.members.delete(list_id='', subscriber_hash='')
+   client.lists.members.delete_permanent(list_id='', subscriber_hash='')
 
 List Member Activity
 ^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.lists.members.activity.all(list_id='', subscriber_hash='')
+   client.lists.members.activity.all(list_id='', subscriber_hash='')
 
 List Member Goals
 ^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.lists.members.goals.all(list_id='', subscriber_hash='')
+   client.lists.members.goals.all(list_id='', subscriber_hash='')
 
 List Member Notes
 ^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.lists.members.notes.create(list_id='', subscriber_hash='', data={})
-    client.lists.members.notes.all(list_id='', subscriber_hash='', get_all=False)
-    client.lists.members.notes.get(list_id='', subscriber_hash='', note_id='')
-    client.lists.members.notes.update(list_id='', subscriber_hash='', note_id='', data={})
-    client.lists.members.notes.delete(list_id='', subscriber_hash='', note_id='')
+   client.lists.members.notes.create(list_id='', subscriber_hash='', data={})
+   client.lists.members.notes.all(list_id='', subscriber_hash='', get_all=False)
+   client.lists.members.notes.get(list_id='', subscriber_hash='', note_id='')
+   client.lists.members.notes.update(list_id='', subscriber_hash='', note_id='', data={})
+   client.lists.members.notes.delete(list_id='', subscriber_hash='', note_id='')
+
+List Member Tags
+^^^^^^^^^^^^^^^^
+
+::
+
+   client.lists.members.tags.update(list_id='', subscriber_hash='', data={})
+   client.lists.members.tags.all(list_id='', subscriber_hash='')
 
 List Merge Fields
 ^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.lists.merge_fields.create(list_id='', data={})
-    client.lists.merge_fields.all(list_id='', get_all=False)
-    client.lists.merge_fields.get(list_id='', merge_id='')
-    client.lists.merge_fields.update(list_id='', merge_id='', data={})
-    client.lists.merge_fields.delete(list_id='', merge_id='')
+   client.lists.merge_fields.create(list_id='', data={})
+   client.lists.merge_fields.all(list_id='', get_all=False)
+   client.lists.merge_fields.get(list_id='', merge_id='')
+   client.lists.merge_fields.update(list_id='', merge_id='', data={})
+   client.lists.merge_fields.delete(list_id='', merge_id='')
 
 List Segments
 ^^^^^^^^^^^^^
 
 ::
 
-    client.lists.segments.create(list_id='', data={})
-    client.lists.segments.all(list_id='', get_all=False)
-    client.lists.segments.get(list_id='', segment_id='')
-    client.lists.segments.update(list_id='', segment_id='', data={})
-    client.lists.segments.update_members(list_id='', segment_id='', data={})
-    client.lists.segments.delete(list_id='', segment_id='')
+   client.lists.segments.create(list_id='', data={})
+   client.lists.segments.all(list_id='', get_all=False)
+   client.lists.segments.get(list_id='', segment_id='')
+   client.lists.segments.update(list_id='', segment_id='', data={})
+   client.lists.segments.update_members(list_id='', segment_id='', data={})
+   client.lists.segments.delete(list_id='', segment_id='')
 
 List Segment Members
 ^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.lists.segments.members.create(list_id='', segment_id='', data={})
-    client.lists.segments.members.all(list_id='', segment_id='', get_all=False)
-    client.lists.segments.members.delete(list_id='', segment_id='', subscriber_hash='')
+   client.lists.segments.members.create(list_id='', segment_id='', data={})
+   client.lists.segments.members.all(list_id='', segment_id='', get_all=False)
+   client.lists.segments.members.delete(list_id='', segment_id='', subscriber_hash='')
 
 List Signup Forms
 ^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.lists.signup_forms.create(list_id='', data={})
-    client.lists.signup_forms.all(list_id='')
+   client.lists.signup_forms.create(list_id='', data={})
+   client.lists.signup_forms.all(list_id='')
 
 List Webhooks
 ^^^^^^^^^^^^^
 
 ::
 
-    client.lists.webhooks.create(list_id='', data={})
-    client.lists.webhooks.all(list_id='')
-    client.lists.webhooks.get(list_id='', webhook_id='')
-    client.lists.webhooks.update(list_id='', webhook_id='', data={})
-    client.lists.webhooks.delete(list_id='', webhook_id='')
+   client.lists.webhooks.create(list_id='', data={})
+   client.lists.webhooks.all(list_id='')
+   client.lists.webhooks.get(list_id='', webhook_id='')
+   client.lists.webhooks.update(list_id='', webhook_id='', data={})
+   client.lists.webhooks.delete(list_id='', webhook_id='')
 
 Reports
 ~~~~~~~
 
 .. _reports-1:
 
 Reports
 ^^^^^^^
 
 ::
 
-    client.reports.all(get_all=False)
-    client.reports.get(campaign_id='')
+   client.reports.all(get_all=False)
+   client.reports.get(campaign_id='')
 
 Campaign Abuse Reports
 ^^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.reports.abuse_reports.all(campaign_id='')
-    client.reports.abuse_reports.get(campaign_id='', report_id='')
+   client.reports.abuse_reports.all(campaign_id='')
+   client.reports.abuse_reports.get(campaign_id='', report_id='')
 
 Campaign Advice
 ^^^^^^^^^^^^^^^
 
 ::
 
-    client.reports.advice.all(campaign_id='')
+   client.reports.advice.all(campaign_id='')
 
 Click Details Report
 ^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.reports.click_details.all(campaign_id='', get_all=False)
-    client.reports.click_details.get(campaign_id='', link_id='')
+   client.reports.click_details.all(campaign_id='', get_all=False)
+   client.reports.click_details.get(campaign_id='', link_id='')
 
 Click Details Report Members
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.reports.click_details.members.all(campaign_id='', link_id='', get_all=False)
-    client.reports.click_details.members.get(campaign_id='', link_id='', subscriber_hash='')
+   client.reports.click_details.members.all(campaign_id='', link_id='', get_all=False)
+   client.reports.click_details.members.get(campaign_id='', link_id='', subscriber_hash='')
 
 Domain Performance Reports
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.reports.domain_performance.all(campaign_id='')
+   client.reports.domain_performance.all(campaign_id='')
 
 EepURL Reports
 ^^^^^^^^^^^^^^
 
 ::
 
-    client.reports.eepurl.all(camnpaign_id='')
+   client.reports.eepurl.all(camnpaign_id='')
 
 Email Activity Reports
 ^^^^^^^^^^^^^^^^^^^^^^
 
 ::
 
-    client.reports.email_activity.all(campaign_id='', get_all=False)
-    client.reports.email_activity.get(campaign_id='', subscriber_hash='')
+   client.reports.email_activity.all(campaign_id='', get_all=False)
+   client.reports.email_activity.get(campaign_id='', subscriber_hash='')
 
 Locations Report
 ^^^^^^^^^^^^^^^^
 
 ::
 
-    client.reports.locations.all(campaign_id='', get_all=False)
+   client.reports.locations.all(campaign_id='', get_all=False)
 
 Sent To Reports
 ^^^^^^^^^^^^^^^
 
 ::
 
-    client.reports.sent_to.all(campaign_id='', get_all=False)
-    client.reports.sent_to.get(campaign_id='', subscriber_hash='')
+   client.reports.sent_to.all(campaign_id='', get_all=False)
+   client.reports.sent_to.get(campaign_id='', subscriber_hash='')
 
 Sub-Reports
 ^^^^^^^^^^^
 
 ::
 
-    client.reports.subreports.all(campaign_id='')
+   client.reports.subreports.all(campaign_id='')
 
 Unsubscribes
 ^^^^^^^^^^^^
 
 ::
 
-    client.reports.unsubscribes.all(campaign_id='', get_all=False)
-    client.reports.unsubscribes.get(campaign_id='', subscriber_hash='')
+   client.reports.unsubscribes.all(campaign_id='', get_all=False)
+   client.reports.unsubscribes.get(campaign_id='', subscriber_hash='')
 
 Search
 ~~~~~~
 
 .. _campaigns-2:
 
 Campaigns
 ^^^^^^^^^
 
 ::
 
-    client.search_campaigns.get()
+   client.search_campaigns.get()
 
 Members
 ^^^^^^^
 
 ::
 
-    client.search_members.get()
+   client.search_members.get()
 
 Templates
 ~~~~~~~~~
 
 .. _folders-2:
 
 Folders
 ^^^^^^^
 
 ::
 
-    client.template_folders.create(data={})
-    client.template_folders.all(get_all=False)
-    client.template_folders.get(folder_id='')
-    client.template_folders.update(folder_id='', data={})
-    client.template_folders.delete(folder_id='')
+   client.template_folders.create(data={})
+   client.template_folders.all(get_all=False)
+   client.template_folders.get(folder_id='')
+   client.template_folders.update(folder_id='', data={})
+   client.template_folders.delete(folder_id='')
 
 .. _templates-1:
 
 Templates
 ^^^^^^^^^
 
 ::
 
-    client.templates.create(data={})
-    client.templates.all(get_all=False)
-    client.templates.get(template_id='')
-    client.templates.update(template_id='', data={})
-    client.templates.delete(template_id='')
+   client.templates.create(data={})
+   client.templates.all(get_all=False)
+   client.templates.get(template_id='')
+   client.templates.update(template_id='', data={})
+   client.templates.delete(template_id='')
 
 Default Content
 ^^^^^^^^^^^^^^^
 
 ::
 
-    client.templates.default_content.all(template_id='')
+   client.templates.default_content.all(template_id='')
 
 Logging
 -------
 
 The MailChimp client will log request/response detail into the
 mailchimp3.client logging namespace. Consider the following snippet to
 get started with logging:
 
 .. code:: python
 
-    import logging
-    fh = logging.FileHandler('/path/to/some/log.log')
-    logger = logging.getLogger('mailchimp3.client')
-    logger.addHandler(fh)
+   import logging
+   fh = logging.FileHandler('/path/to/some/log.log')
+   logger = logging.getLogger('mailchimp3.client')
+   logger.addHandler(fh)
 
-    # use the client normally
-    client.lists.all(**{'fields': 'lists.date_created'})
+   # use the client normally
+   client.lists.all(**{'fields': 'lists.date_created'})
 
 request/response detail will be appended into /path/to/some/log.log:
 
 ::
 
-    GET Request: https://us15.api.mailchimp.com/3.0/lists?fields=lists.date_created
-    GET Response: 200 {"lists":[{"date_created":"2017-05-10T13:53:05+00:00"},{"date_created":"2017-08-22T20:27:56+00:00"},{"date_created":"2017-05-12T21:22:15+00:00"},{"date_created":"2017-04-27T17:42:04+00:00"},{"date_created":"2017-05-10T14:14:49+00:00"},{"date_created":"2017-05-10T13:52:37+00:00"},{"date_created":"2017-05-10T13:51:40+00:00"}]}
+   GET Request: https://us15.api.mailchimp.com/3.0/lists?fields=lists.date_created
+   GET Response: 200 {"lists":[{"date_created":"2017-05-10T13:53:05+00:00"},{"date_created":"2017-08-22T20:27:56+00:00"},{"date_created":"2017-05-12T21:22:15+00:00"},{"date_created":"2017-04-27T17:42:04+00:00"},{"date_created":"2017-05-10T14:14:49+00:00"},{"date_created":"2017-05-10T13:52:37+00:00"},{"date_created":"2017-05-10T13:51:40+00:00"}]}
 
 Check the `docs <https://docs.python.org/2/library/logging.html>`__ for
 more detail on the Python logging package.
 
 Support
 -------
 
 If you are having issues, please let us know or submit a pull request.
 
 License
 -------
 
 The project is licensed under the MIT License.
 
-.. |mailchimp3 v3.0.7 on PyPi| image:: https://img.shields.io/pypi/v/mailchimp3.svg
+.. |mailchimp3 v3.0.9 on PyPi| image:: https://img.shields.io/pypi/v/mailchimp3.svg
    :target: https://pypi.python.org/pypi/mailchimp3
 .. |MIT license| image:: https://img.shields.io/badge/licence-MIT-blue.svg
 .. |Stable| image:: https://img.shields.io/badge/status-stable-green.svg
```

