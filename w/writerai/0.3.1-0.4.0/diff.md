# Comparing `tmp/writerai-0.3.1.tar.gz` & `tmp/writerai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "writerai-0.3.1.tar", last modified: Wed Mar 15 16:17:39 2023, max compression
+gzip compressed data, was "writerai-0.4.0.tar", last modified: Mon Apr 17 12:53:39 2023, max compression
```

## Comparing `writerai-0.3.1.tar` & `writerai-0.4.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:17:39.324544 writerai-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-03-15 16:17:39.320544 writerai-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-03-15 16:17:30.000000 writerai-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 16:17:39.324544 writerai-0.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1009 2023-03-15 16:17:30.000000 writerai-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:17:39.312544 writerai-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:17:39.312544 writerai-0.3.1/src/writer/
--rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2602 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/ai_content_detector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2125 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/billing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4520 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/completions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4398 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/content.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3996 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/cowrite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2316 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/download_the_customized_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6394 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6865 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/modelcustomization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:17:39.312544 writerai-0.3.1/src/writer/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:17:39.316544 writerai-0.3.1/src/writer/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2471 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1326 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/addterms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/contentcheck.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1469 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/contentcorrect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1332 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/createcompletion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1394 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/createmodelcustomization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/createmodelcustomizationcompletion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1030 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/deletefile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/deletemodelcustomization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/deletesnippets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/deleteterms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1256 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/detectcontent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/fetchcustomizedmodelfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2530 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/findsnippets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2946 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/findterms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/generate_content.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1053 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/getfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1273 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/getmodelcustomization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/getsubscriptiondetails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      976 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/listfiles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/listmodelcustomizations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1008 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/listmodels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/listpages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1271 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/listtemplates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/listusers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      966 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/pagedetails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1485 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/updatesnippets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1490 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/updateterms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1176 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/operations/uploadfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:17:39.320544 writerai-0.3.1/src/writer/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4097 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/approvedtermextension.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      635 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/approvedtermextensioncreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      736 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/completiongenerationchoice.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/completiongenerationchoicelogprobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2185 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/completionrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/completionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/contentdetectorrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      612 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/contentdetectorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2431 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/contentissue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/contentrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2525 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/contentsettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/correctionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1977 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/createcustomizationrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/createtermsrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/createtermsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/customizationsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/deleteresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1930 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/draft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      608 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/failmessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/failresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1586 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/fulllinkedterm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4299 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/fulltermwithuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/generatetemplaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      732 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/generationmodelinforesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      590 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/generationmodelsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/hyperparameters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1933 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/input.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/linkedtermcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      553 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/magicrequestinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2917 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/modelcustomization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1156 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/modelfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/modelfilesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/pagepublicapiresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2269 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/pagewithsectionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      888 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/paginatedresult_fulltermwithuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      913 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/paginatedresult_pagepublicapiresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/paginatedresult_snippetwithuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/paginatedresult_userpublicresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/pagination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      526 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/processedcontent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      565 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/sectioninfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      250 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/simpleuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      340 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/snippettagv2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/snippetupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2116 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/snippetwithuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/subscriptionpublicresponseapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/templatedetailsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3104 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/termcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1013 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/termexample.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      590 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/termexamplecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      720 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/terminologyuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/termmistake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1036 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/termmistakecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/termtagcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      702 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/termtagresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3034 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/termupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/updatetermsrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/uploadmodelfilerequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/usage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      457 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/usageitem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2454 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models/shared/userpublicresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2165 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/models_.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5782 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5463 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/snippet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3532 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/styleguide.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7239 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/terminology.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2195 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:17:39.320544 writerai-0.3.1/src/writer/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24723 2023-03-15 16:17:30.000000 writerai-0.3.1/src/writer/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:17:39.320544 writerai-0.3.1/src/writerai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-03-15 16:17:39.000000 writerai-0.3.1/src/writerai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-03-15 16:17:39.000000 writerai-0.3.1/src/writerai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 16:17:39.000000 writerai-0.3.1/src/writerai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-15 16:17:39.000000 writerai-0.3.1/src/writerai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-15 16:17:39.000000 writerai-0.3.1/src/writerai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.080897 writerai-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-17 12:53:39.080897 writerai-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-17 12:53:29.000000 writerai-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:53:39.080897 writerai-0.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-04-17 12:53:29.000000 writerai-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.068897 writerai-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.072897 writerai-0.4.0/src/writer/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2710 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/ai_content_detector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2221 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/billing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4602 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/completions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4476 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/content.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4074 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/cowrite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2434 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/download_the_customized_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6434 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6919 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/modelcustomization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.072897 writerai-0.4.0/src/writer/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.072897 writerai-0.4.0/src/writer/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2547 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1453 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/addterms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/contentcheck.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/contentcorrect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1459 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/createcompletion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1521 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/createmodelcustomization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/createmodelcustomizationcompletion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/deletefile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/deletemodelcustomization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/deletesnippets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1521 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/deleteterms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1381 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/detectcontent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/fetchcustomizedmodelfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/findsnippets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3087 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/findterms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/generate_content.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1178 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/getfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/getmodelcustomization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/getsubscriptiondetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listfiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1277 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listmodelcustomizations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listmodels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listpages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listtemplates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2131 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/listusers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1089 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/pagedetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1614 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/updatesnippets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/updateterms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/operations/uploadfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.080897 writerai-0.4.0/src/writer/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4173 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/approvedtermextension.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/approvedtermextensioncreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/completiongenerationchoice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1135 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/completiongenerationchoicelogprobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2288 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/completionrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      669 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/completionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      437 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/contentdetectorrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/contentdetectorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2524 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/contentissue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/contentrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2638 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/contentsettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      437 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/correctionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2076 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/createcustomizationrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1008 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/createtermsrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      890 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/createtermsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/customizationsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/deleteresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/draft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      695 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/failmessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/failresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1681 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/fulllinkedterm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4416 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/fulltermwithuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/generatetemplaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/generationmodelinforesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/generationmodelsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/hyperparameters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2034 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/input.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/linkedtermcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/magicrequestinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3026 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/modelcustomization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1249 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/modelfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/modelfilesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2186 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/pagepublicapiresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2370 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/pagewithsectionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      975 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/paginatedresult_fulltermwithuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/paginatedresult_pagepublicapiresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      970 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/paginatedresult_snippetwithuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      985 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/paginatedresult_userpublicresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      685 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/pagination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      609 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/processedcontent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/sectioninfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/simpleuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/snippettagv2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/snippetupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/snippetwithuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/subscriptionpublicresponseapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/templatedetailsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3209 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termexample.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termexamplecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/terminologyuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1344 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termmistake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termmistakecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termtagcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termtagresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3139 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/termupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1008 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/updatetermsrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      550 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/uploadmodelfilerequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/usage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      542 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/usageitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2557 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models/shared/userpublicresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2259 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/models_.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7161 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5524 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/snippet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3613 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/styleguide.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7285 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/terminology.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2288 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.080897 writerai-0.4.0/src/writer/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-17 12:53:29.000000 writerai-0.4.0/src/writer/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:53:39.080897 writerai-0.4.0/src/writerai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-17 12:53:38.000000 writerai-0.4.0/src/writerai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 12:53:38.000000 writerai-0.4.0/src/writerai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:53:38.000000 writerai-0.4.0/src/writerai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-17 12:53:38.000000 writerai-0.4.0/src/writerai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 12:53:38.000000 writerai-0.4.0/src/writerai.egg-info/top_level.txt
```

### Comparing `writerai-0.3.1/PKG-INFO` & `writerai-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: writerai
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python SDK for Writer API
 Home-page: UNKNOWN
 Author: writerai
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <div align="center">
         <source srcset="https://user-images.githubusercontent.com/6267663/223574357-9a053550-02f9-49f1-b453-1b11db148d7b.svg" media="(prefers-color-scheme: dark)" width="500">
         <img src="https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-44e8-ac48-f9494101e1dc.svg" width="500">
     <h1>Python SDK</h1>
    <p>AI for everyone.</p>
    <a href="https://dev.writer.com/docs"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=000000&style=for-the-badge" /></a>
-   <a href="https://github.com/writerai/writer-client-sdk-python/actions"><img src="https://img.shields.io/github/actions/workflow/status/writerai/writer-client-sdk-python/speakeasy_generate.yaml?style=for-the-badge" /></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" /></a>
   <a href="https://github.com/writerai/writer-client-sdk-python/releases"><img src="https://img.shields.io/github/v/release/writerai/writer-client-sdk-python?sort=semver&style=for-the-badge" /></a>
 </div>
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
@@ -50,27 +49,27 @@
     ),
     organization_id=548814,
 )
 
 
 req = operations.DetectContentRequest(
     content_detector_request=shared.ContentDetectorRequest(
-        input="example",
+        input="provident",
     ),
 )
     
 res = s.ai_content_detector.detect(req)
 
 if res.content_detector_responses is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### ai_content_detector
 
 * `detect` - Content detector api
 
 ### billing
```

#### html2text {}

```diff
@@ -1,36 +1,34 @@
-Metadata-Version: 2.1 Name: writerai Version: 0.3.1 Summary: Python SDK for
+Metadata-Version: 2.1 Name: writerai Version: 0.4.0 Summary: Python SDK for
 Writer API Home-page: UNKNOWN Author: writerai License: UNKNOWN Platform:
 UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/markdown
   [https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-
                           44e8-ac48-f9494101e1dc.svg]
                            ****** Python SDK ******
                                AI for everyone.
            [https://img.shields.io/static/v1?label=Docs&message=API
- Ref&color=000000&style=for-the-badge] [https://img.shields.io/github/actions/
-              workflow/status/writerai/writer-client-sdk-python/
-  speakeasy_generate.yaml?style=for-the-badge] [https://img.shields.io/badge/
-  License-MIT-blue.svg?style=for-the-badge] [https://img.shields.io/github/v/
-  release/writerai/writer-client-sdk-python?sort=semver&style=for-the-badge]
+ Ref&color=000000&style=for-the-badge] [https://img.shields.io/badge/License-
+  MIT-blue.svg?style=for-the-badge] [https://img.shields.io/github/v/release/
+      writerai/writer-client-sdk-python?sort=semver&style=for-the-badge]
  ## SDK Installation ```bash pip install writerai ```  ## Authentication Writer
 authenticates your API requests using your accountâs API keys. If you do not
 include your key when making an API request, or use one that is incorrect or
 outdated, Writer returns an error. Your API keys are available in the account
 dashboard. We include randomly generated API keys in our code examples if you
 are not logged in. Replace these with your own or log in to see code examples
 populated with your own API keys. [writer-auth] If you cannot see your secret
 API keys in the Dashboard, this means you do not have access to them. Contact
 your Writer account owner and ask to be added to their team as a developer. ##
 SDK Example Usage  ```python import writer from writer.models import
 operations, shared s = writer.Writer( security=shared.Security
 ( api_key="YOUR_API_KEY_HERE", ), organization_id=548814, ) req =
 operations.DetectContentRequest
-( content_detector_request=shared.ContentDetectorRequest( input="example", ), )
-res = s.ai_content_detector.detect(req) if res.content_detector_responses is
-not None: # handle response ```   ## SDK Available Operations ###
+( content_detector_request=shared.ContentDetectorRequest( input="provident", ),
+) res = s.ai_content_detector.detect(req) if res.content_detector_responses is
+not None: # handle response ```   ## Available Resources and Operations ###
 ai_content_detector * `detect` - Content detector api ### billing *
 `get_subscription_details` - Get your organization subscription details ###
 co_write * `generate_content` - Generate content using predefined templates *
 `list_templates` - Get a list of your existing CoWrite templates ###
 completions * `create` - Create completion for LLM model *
 `create_model_customization_completion` - Create completion for LLM
 customization model ### content * `check` - Check your content against your
```

### Comparing `writerai-0.3.1/README.md` & `writerai-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 <div align="center">
         <source srcset="https://user-images.githubusercontent.com/6267663/223574357-9a053550-02f9-49f1-b453-1b11db148d7b.svg" media="(prefers-color-scheme: dark)" width="500">
         <img src="https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-44e8-ac48-f9494101e1dc.svg" width="500">
     <h1>Python SDK</h1>
    <p>AI for everyone.</p>
    <a href="https://dev.writer.com/docs"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=000000&style=for-the-badge" /></a>
-   <a href="https://github.com/writerai/writer-client-sdk-python/actions"><img src="https://img.shields.io/github/actions/workflow/status/writerai/writer-client-sdk-python/speakeasy_generate.yaml?style=for-the-badge" /></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" /></a>
   <a href="https://github.com/writerai/writer-client-sdk-python/releases"><img src="https://img.shields.io/github/v/release/writerai/writer-client-sdk-python?sort=semver&style=for-the-badge" /></a>
 </div>
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
@@ -39,27 +38,27 @@
     ),
     organization_id=548814,
 )
 
 
 req = operations.DetectContentRequest(
     content_detector_request=shared.ContentDetectorRequest(
-        input="example",
+        input="provident",
     ),
 )
     
 res = s.ai_content_detector.detect(req)
 
 if res.content_detector_responses is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### ai_content_detector
 
 * `detect` - Content detector api
 
 ### billing
```

#### html2text {}

```diff
@@ -1,33 +1,31 @@
   [https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-
                           44e8-ac48-f9494101e1dc.svg]
                            ****** Python SDK ******
                                AI for everyone.
            [https://img.shields.io/static/v1?label=Docs&message=API
- Ref&color=000000&style=for-the-badge] [https://img.shields.io/github/actions/
-              workflow/status/writerai/writer-client-sdk-python/
-  speakeasy_generate.yaml?style=for-the-badge] [https://img.shields.io/badge/
-  License-MIT-blue.svg?style=for-the-badge] [https://img.shields.io/github/v/
-  release/writerai/writer-client-sdk-python?sort=semver&style=for-the-badge]
+ Ref&color=000000&style=for-the-badge] [https://img.shields.io/badge/License-
+  MIT-blue.svg?style=for-the-badge] [https://img.shields.io/github/v/release/
+      writerai/writer-client-sdk-python?sort=semver&style=for-the-badge]
  ## SDK Installation ```bash pip install writerai ```  ## Authentication Writer
 authenticates your API requests using your accountâs API keys. If you do not
 include your key when making an API request, or use one that is incorrect or
 outdated, Writer returns an error. Your API keys are available in the account
 dashboard. We include randomly generated API keys in our code examples if you
 are not logged in. Replace these with your own or log in to see code examples
 populated with your own API keys. [writer-auth] If you cannot see your secret
 API keys in the Dashboard, this means you do not have access to them. Contact
 your Writer account owner and ask to be added to their team as a developer. ##
 SDK Example Usage  ```python import writer from writer.models import
 operations, shared s = writer.Writer( security=shared.Security
 ( api_key="YOUR_API_KEY_HERE", ), organization_id=548814, ) req =
 operations.DetectContentRequest
-( content_detector_request=shared.ContentDetectorRequest( input="example", ), )
-res = s.ai_content_detector.detect(req) if res.content_detector_responses is
-not None: # handle response ```   ## SDK Available Operations ###
+( content_detector_request=shared.ContentDetectorRequest( input="provident", ),
+) res = s.ai_content_detector.detect(req) if res.content_detector_responses is
+not None: # handle response ```   ## Available Resources and Operations ###
 ai_content_detector * `detect` - Content detector api ### billing *
 `get_subscription_details` - Get your organization subscription details ###
 co_write * `generate_content` - Generate content using predefined templates *
 `list_templates` - Get a list of your existing CoWrite templates ###
 completions * `create` - Create completion for LLM model *
 `create_model_customization_completion` - Create completion for LLM
 customization model ### content * `check` - Check your content against your
```

### Comparing `writerai-0.3.1/setup.py` & `writerai-0.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import setuptools
 
 try:
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="writerai",
-    version="0.3.1",
+    version="0.4.0",
     author="writerai",
     description="Python SDK for Writer API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `writerai-0.3.1/src/writer/ai_content_detector.py` & `writerai-0.4.0/src/writer/ai_content_detector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
 class AIContentDetector:
+    r"""Methods related to AI Content Detector"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -18,17 +21,15 @@
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
     def detect(self, request: operations.DetectContentRequest) -> operations.DetectContentResponse:
-        r"""Content detector api
-        """
-        
+        r"""Content detector api"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.DetectContentRequest, base_url, '/content/organization/{organizationId}/detect', request, self._globals)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "content_detector_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
```

### Comparing `writerai-0.3.1/src/writer/billing.py` & `writerai-0.4.0/src/writer/billing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
 class Billing:
+    r"""Methods related to Billing"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -18,17 +21,15 @@
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
     def get_subscription_details(self) -> operations.GetSubscriptionDetailsResponse:
-        r"""Get your organization subscription details
-        """
-        
+        r"""Get your organization subscription details"""
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/billing/subscription'
         
         
         client = self._security_client
```

### Comparing `writerai-0.3.1/src/writer/completions.py` & `writerai-0.4.0/src/writer/completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
 class Completions:
+    r"""Methods related to Completions"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -18,17 +21,15 @@
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
     def create(self, request: operations.CreateCompletionRequest) -> operations.CreateCompletionResponse:
-        r"""Create completion for LLM model
-        """
-        
+        r"""Create completion for LLM model"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateCompletionRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/completions', request, self._globals)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "completion_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
@@ -55,17 +56,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def create_model_customization_completion(self, request: operations.CreateModelCustomizationCompletionRequest) -> operations.CreateModelCustomizationCompletionResponse:
-        r"""Create completion for LLM customization model
-        """
-        
+        r"""Create completion for LLM customization model"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateModelCustomizationCompletionRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}/completions', request, self._globals)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "completion_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
```

### Comparing `writerai-0.3.1/src/writer/content.py` & `writerai-0.4.0/src/writer/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
 class Content:
+    r"""Methods related to Content"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -18,17 +21,15 @@
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
     def check(self, request: operations.ContentCheckRequest) -> operations.ContentCheckResponse:
-        r"""Check your content against your preset styleguide.
-        """
-        
+        r"""Check your content against your preset styleguide."""
         base_url = self._server_url
         
         url = utils.generate_url(operations.ContentCheckRequest, base_url, '/content/organization/{organizationId}/team/{teamId}/check', request, self._globals)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "content_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
@@ -55,17 +56,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def correct(self, request: operations.ContentCorrectRequest) -> operations.ContentCorrectResponse:
-        r"""Apply the style guide suggestions directly to your content.
-        """
-        
+        r"""Apply the style guide suggestions directly to your content."""
         base_url = self._server_url
         
         url = utils.generate_url(operations.ContentCorrectRequest, base_url, '/content/organization/{organizationId}/team/{teamId}/correct', request, self._globals)
         
         headers = utils.get_headers(request)
         req_content_type, data, form = utils.serialize_request_body(request, "content_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
```

### Comparing `writerai-0.3.1/src/writer/cowrite.py` & `writerai-0.4.0/src/writer/cowrite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
 class CoWrite:
+    r"""Methods related to CoWrite"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -18,17 +21,15 @@
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
     def generate_content(self, request: operations.GenerateContentRequest) -> operations.GenerateContentResponse:
-        r"""Generate content using predefined templates
-        """
-        
+        r"""Generate content using predefined templates"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.GenerateContentRequest, base_url, '/cowrite/organization/{organizationId}/team/{teamId}/generate', request, self._globals)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "generate_template_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
@@ -55,17 +56,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def list_templates(self, request: operations.ListTemplatesRequest) -> operations.ListTemplatesResponse:
-        r"""Get a list of your existing CoWrite templates
-        """
-        
+        r"""Get a list of your existing CoWrite templates"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListTemplatesRequest, base_url, '/cowrite/organization/{organizationId}/team/{teamId}/template/{templateId}', request, self._globals)
         
         
         client = self._security_client
```

### Comparing `writerai-0.3.1/src/writer/download_the_customized_model.py` & `writerai-0.4.0/src/writer/models_.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
-class DownloadTheCustomizedModel:
+class Models:
+    r"""Methods related to Model"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -17,35 +20,34 @@
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
-    def fetch_file(self, request: operations.FetchCustomizedModelFileRequest) -> operations.FetchCustomizedModelFileResponse:
-        r"""Download your fine-tuned model (available only for Palmyra Base and Palmyra Large)
-        """
-        
+    def list(self, request: operations.ListModelsRequest) -> operations.ListModelsResponse:
+        r"""List available LLM models"""
         base_url = self._server_url
         
-        url = utils.generate_url(operations.FetchCustomizedModelFileRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}/fetch', request, self._globals)
+        url = utils.generate_url(operations.ListModelsRequest, base_url, '/llm/organization/{organizationId}/model', request, self._globals)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.FetchCustomizedModelFileResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListModelsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(content_type, 'application/octet-stream'):
-                res.fetch_customized_model_file_200_application_octet_stream_binary_string = http_res.content
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.GenerationModelsResponse])
+                res.generation_models_response = out
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
```

### Comparing `writerai-0.3.1/src/writer/files.py` & `writerai-0.4.0/src/writer/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
 class Files:
+    r"""Methods related to Files"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -18,17 +21,15 @@
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
     def delete(self, request: operations.DeleteFileRequest) -> operations.DeleteFileResponse:
-        r"""Delete file
-        """
-        
+        r"""Delete file"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.DeleteFileRequest, base_url, '/llm/organization/{organizationId}/file/{fileId}', request, self._globals)
         
         
         client = self._security_client
         
@@ -49,17 +50,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def get(self, request: operations.GetFileRequest) -> operations.GetFileResponse:
-        r"""Get file
-        """
-        
+        r"""Get file"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetFileRequest, base_url, '/llm/organization/{organizationId}/file/{fileId}', request, self._globals)
         
         
         client = self._security_client
         
@@ -80,17 +79,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def list(self, request: operations.ListFilesRequest) -> operations.ListFilesResponse:
-        r"""List files
-        """
-        
+        r"""List files"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListFilesRequest, base_url, '/llm/organization/{organizationId}/file', request, self._globals)
         
         
         client = self._security_client
         
@@ -111,17 +108,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def upload(self, request: operations.UploadFileRequest) -> operations.UploadFileResponse:
-        r"""Upload file
-        """
-        
+        r"""Upload file"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.UploadFileRequest, base_url, '/llm/organization/{organizationId}/file', request, self._globals)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "upload_model_file_request", 'multipart')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
```

### Comparing `writerai-0.3.1/src/writer/modelcustomization.py` & `writerai-0.4.0/src/writer/modelcustomization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
 class ModelCustomization:
+    r"""Methods related to Model Customization"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -18,17 +21,15 @@
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
     def create(self, request: operations.CreateModelCustomizationRequest) -> operations.CreateModelCustomizationResponse:
-        r"""Create model customization
-        """
-        
+        r"""Create model customization"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateModelCustomizationRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization', request, self._globals)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "create_customization_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
@@ -55,17 +56,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def delete(self, request: operations.DeleteModelCustomizationRequest) -> operations.DeleteModelCustomizationResponse:
-        r"""Delete Model customization
-        """
-        
+        r"""Delete Model customization"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.DeleteModelCustomizationRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}', request, self._globals)
         
         
         client = self._security_client
         
@@ -86,17 +85,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def get(self, request: operations.GetModelCustomizationRequest) -> operations.GetModelCustomizationResponse:
-        r"""Get model customization
-        """
-        
+        r"""Get model customization"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetModelCustomizationRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}', request, self._globals)
         
         
         client = self._security_client
         
@@ -117,17 +114,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def list(self, request: operations.ListModelCustomizationsRequest) -> operations.ListModelCustomizationsResponse:
-        r"""List model customizations
-        """
-        
+        r"""List model customizations"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListModelCustomizationsRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization', request, self._globals)
         
         
         client = self._security_client
```

### Comparing `writerai-0.3.1/src/writer/models/operations/__init__.py` & `writerai-0.4.0/src/writer/models/operations/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from .addterms import *
 from .contentcheck import *
 from .contentcorrect import *
 from .createcompletion import *
 from .createmodelcustomization import *
 from .createmodelcustomizationcompletion import *
 from .deletefile import *
```

### Comparing `writerai-0.3.1/src/writer/models/operations/addterms.py` & `writerai-0.4.0/src/writer/models/operations/addterms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import createtermsrequest as shared_createtermsrequest
 from ..shared import createtermsresponse as shared_createtermsresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class AddTermsRequest:
-    create_terms_request: shared_createtermsrequest.CreateTermsRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+    create_terms_request: shared_createtermsrequest.CreateTermsRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class AddTermsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    create_terms_response: Optional[shared_createtermsresponse.CreateTermsResponse] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    create_terms_response: Optional[shared_createtermsresponse.CreateTermsResponse] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/contentcheck.py` & `writerai-0.4.0/src/writer/models/operations/contentcheck.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import contentrequest as shared_contentrequest
 from ..shared import failresponse as shared_failresponse
 from ..shared import processedcontent as shared_processedcontent
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ContentCheckRequest:
-    content_request: shared_contentrequest.ContentRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+    content_request: shared_contentrequest.ContentRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class ContentCheckResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    processed_content: Optional[shared_processedcontent.ProcessedContent] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    processed_content: Optional[shared_processedcontent.ProcessedContent] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/contentcorrect.py` & `writerai-0.4.0/src/writer/models/operations/contentcorrect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import contentrequest as shared_contentrequest
 from ..shared import correctionresponse as shared_correctionresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ContentCorrectRequest:
-    content_request: shared_contentrequest.ContentRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
-    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
+    
+    content_request: shared_contentrequest.ContentRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class ContentCorrectResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    correction_response: Optional[shared_correctionresponse.CorrectionResponse] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    correction_response: Optional[shared_correctionresponse.CorrectionResponse] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/createcompletion.py` & `writerai-0.4.0/src/writer/models/operations/createcompletion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import completionrequest as shared_completionrequest
 from ..shared import completionresponse as shared_completionresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateCompletionRequest:
-    completion_request: shared_completionrequest.CompletionRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+    completion_request: shared_completionrequest.CompletionRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class CreateCompletionResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    completion_response: Optional[shared_completionresponse.CompletionResponse] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    completion_response: Optional[shared_completionresponse.CompletionResponse] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/createmodelcustomization.py` & `writerai-0.4.0/src/writer/models/operations/createmodelcustomization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import createcustomizationrequest as shared_createcustomizationrequest
 from ..shared import failresponse as shared_failresponse
 from ..shared import modelcustomization as shared_modelcustomization
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateModelCustomizationRequest:
-    create_customization_request: shared_createcustomizationrequest.CreateCustomizationRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+    create_customization_request: shared_createcustomizationrequest.CreateCustomizationRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class CreateModelCustomizationResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    model_customization: Optional[shared_modelcustomization.ModelCustomization] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    model_customization: Optional[shared_modelcustomization.ModelCustomization] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/createmodelcustomizationcompletion.py` & `writerai-0.4.0/src/writer/models/operations/createmodelcustomizationcompletion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import completionrequest as shared_completionrequest
 from ..shared import completionresponse as shared_completionresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateModelCustomizationCompletionRequest:
-    completion_request: shared_completionrequest.CompletionRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+    completion_request: shared_completionrequest.CompletionRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
+    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})  
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class CreateModelCustomizationCompletionResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    completion_response: Optional[shared_completionresponse.CompletionResponse] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    completion_response: Optional[shared_completionresponse.CompletionResponse] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/deletefile.py` & `writerai-0.4.0/src/writer/models/operations/fetchcustomizedmodelfile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
-from typing import Any, Optional
+from typing import Optional
 
 
 @dataclasses.dataclass
-class DeleteFileRequest:
-    file_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'fileId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+class FetchCustomizedModelFileRequest:
+    
+    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})  
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class DeleteFileResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    delete_file_200_application_json_object: Optional[dict[str, Any]] = dataclasses.field(default=None)
+class FetchCustomizedModelFileResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    fetch_customized_model_file_200_application_octet_stream_binary_string: Optional[bytes] = dataclasses.field(default=None)  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/deletemodelcustomization.py` & `writerai-0.4.0/src/writer/models/operations/deletemodelcustomization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from typing import Any, Optional
 
 
 @dataclasses.dataclass
 class DeleteModelCustomizationRequest:
-    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})  
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class DeleteModelCustomizationResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    delete_model_customization_200_application_json_object: Optional[dict[str, Any]] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    delete_model_customization_200_application_json_object: Optional[dict[str, Any]] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/deletesnippets.py` & `writerai-0.4.0/src/writer/models/operations/deletesnippets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import deleteresponse as shared_deleteresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class DeleteSnippetsRequest:
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
-    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
+    
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
+    ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class DeleteSnippetsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    delete_response: Optional[shared_deleteresponse.DeleteResponse] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    delete_response: Optional[shared_deleteresponse.DeleteResponse] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/deleteterms.py` & `writerai-0.4.0/src/writer/models/operations/deleteterms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import deleteresponse as shared_deleteresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class DeleteTermsRequest:
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    ids: Optional[list[int]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
-    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
+    
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
+    ids: Optional[list[int]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class DeleteTermsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    delete_response: Optional[shared_deleteresponse.DeleteResponse] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    delete_response: Optional[shared_deleteresponse.DeleteResponse] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/detectcontent.py` & `writerai-0.4.0/src/writer/models/operations/detectcontent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import contentdetectorrequest as shared_contentdetectorrequest
 from ..shared import contentdetectorresponse as shared_contentdetectorresponse
 from ..shared import failresponse as shared_failresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class DetectContentRequest:
-    content_detector_request: shared_contentdetectorrequest.ContentDetectorRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+    content_detector_request: shared_contentdetectorrequest.ContentDetectorRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class DetectContentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    content_detector_responses: Optional[list[shared_contentdetectorresponse.ContentDetectorResponse]] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    content_detector_responses: Optional[list[shared_contentdetectorresponse.ContentDetectorResponse]] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/fetchcustomizedmodelfile.py` & `writerai-0.4.0/src/writer/models/operations/deletefile.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclasses.dataclass
-class FetchCustomizedModelFileRequest:
-    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+class DeleteFileRequest:
+    
+    file_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'fileId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class FetchCustomizedModelFileResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+class DeleteFileResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    delete_file_200_application_json_object: Optional[dict[str, Any]] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    fetch_customized_model_file_200_application_octet_stream_binary_string: Optional[bytes] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/findsnippets.py` & `writerai-0.4.0/src/writer/models/operations/findsnippets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,45 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import paginatedresult_snippetwithuser as shared_paginatedresult_snippetwithuser
 from enum import Enum
 from typing import Optional
 
 class FindSnippetsSortFieldEnum(str, Enum):
-    SHORTCUT = "shortcut"
-    CREATION_TIME = "creationTime"
-    MODIFICATION_TIME = "modificationTime"
+    SHORTCUT = 'shortcut'
+    CREATION_TIME = 'creationTime'
+    MODIFICATION_TIME = 'modificationTime'
 
 class FindSnippetsSortOrderEnum(str, Enum):
-    ASC = "asc"
-    DESC = "desc"
+    ASC = 'asc'
+    DESC = 'desc'
 
 
 @dataclasses.dataclass
 class FindSnippetsRequest:
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
-    search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})
-    shortcuts: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'shortcuts', 'style': 'form', 'explode': True }})
-    sort_field: Optional[FindSnippetsSortFieldEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})
-    sort_order: Optional[FindSnippetsSortOrderEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})
-    tags: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tags', 'style': 'form', 'explode': True }})
+    
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
+    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})  
+    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+    search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})  
+    shortcuts: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'shortcuts', 'style': 'form', 'explode': True }})  
+    sort_field: Optional[FindSnippetsSortFieldEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})  
+    sort_order: Optional[FindSnippetsSortOrderEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})  
+    tags: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tags', 'style': 'form', 'explode': True }})  
     
 
 @dataclasses.dataclass
 class FindSnippetsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    paginated_result_snippet_with_user: Optional[shared_paginatedresult_snippetwithuser.PaginatedResultSnippetWithUser] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    paginated_result_snippet_with_user: Optional[shared_paginatedresult_snippetwithuser.PaginatedResultSnippetWithUser] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/findterms.py` & `writerai-0.4.0/src/writer/models/operations/findterms.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,58 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import paginatedresult_fulltermwithuser as shared_paginatedresult_fulltermwithuser
 from enum import Enum
 from typing import Optional
 
 class FindTermsPartOfSpeechEnum(str, Enum):
-    NOUN = "noun"
-    VERB = "verb"
-    ADVERB = "adverb"
-    ADJECTIVE = "adjective"
+    NOUN = 'noun'
+    VERB = 'verb'
+    ADVERB = 'adverb'
+    ADJECTIVE = 'adjective'
 
 class FindTermsSortFieldEnum(str, Enum):
-    TERM = "term"
-    CREATION_TIME = "creationTime"
-    MODIFICATION_TIME = "modificationTime"
-    TYPE = "type"
+    TERM = 'term'
+    CREATION_TIME = 'creationTime'
+    MODIFICATION_TIME = 'modificationTime'
+    TYPE = 'type'
 
 class FindTermsSortOrderEnum(str, Enum):
-    ASC = "asc"
-    DESC = "desc"
+    ASC = 'asc'
+    DESC = 'desc'
 
 class FindTermsTypeEnum(str, Enum):
-    APPROVED = "approved"
-    BANNED = "banned"
-    PENDING = "pending"
+    APPROVED = 'approved'
+    BANNED = 'banned'
+    PENDING = 'pending'
 
 
 @dataclasses.dataclass
 class FindTermsRequest:
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
-    part_of_speech: Optional[FindTermsPartOfSpeechEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'partOfSpeech', 'style': 'form', 'explode': True }})
-    sort_field: Optional[FindTermsSortFieldEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})
-    sort_order: Optional[FindTermsSortOrderEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})
-    tags: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tags', 'style': 'form', 'explode': True }})
-    term: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'term', 'style': 'form', 'explode': True }})
-    type: Optional[FindTermsTypeEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'type', 'style': 'form', 'explode': True }})
+    
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
+    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})  
+    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+    part_of_speech: Optional[FindTermsPartOfSpeechEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'partOfSpeech', 'style': 'form', 'explode': True }})  
+    sort_field: Optional[FindTermsSortFieldEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})  
+    sort_order: Optional[FindTermsSortOrderEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})  
+    tags: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tags', 'style': 'form', 'explode': True }})  
+    term: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'term', 'style': 'form', 'explode': True }})  
+    type: Optional[FindTermsTypeEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'type', 'style': 'form', 'explode': True }})  
     
 
 @dataclasses.dataclass
 class FindTermsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    paginated_result_full_term_with_user: Optional[shared_paginatedresult_fulltermwithuser.PaginatedResultFullTermWithUser] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    paginated_result_full_term_with_user: Optional[shared_paginatedresult_fulltermwithuser.PaginatedResultFullTermWithUser] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/generate_content.py` & `writerai-0.4.0/src/writer/models/operations/generate_content.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import draft as shared_draft
 from ..shared import failresponse as shared_failresponse
 from ..shared import generatetemplaterequest as shared_generatetemplaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GenerateContentRequest:
-    generate_template_request: shared_generatetemplaterequest.GenerateTemplateRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+    generate_template_request: shared_generatetemplaterequest.GenerateTemplateRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class GenerateContentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    draft: Optional[shared_draft.Draft] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    draft: Optional[shared_draft.Draft] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/getfile.py` & `writerai-0.4.0/src/writer/models/operations/listfiles.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
-from ..shared import modelfile as shared_modelfile
+from ..shared import modelfilesresponse as shared_modelfilesresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetFileRequest:
-    file_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'fileId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+class ListFilesRequest:
+    
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class GetFileResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+class ListFilesResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    model_file: Optional[shared_modelfile.ModelFile] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    model_files_response: Optional[shared_modelfilesresponse.ModelFilesResponse] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/getmodelcustomization.py` & `writerai-0.4.0/src/writer/models/operations/getmodelcustomization.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import modelcustomization as shared_modelcustomization
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetModelCustomizationRequest:
-    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+    customization_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customizationId', 'style': 'simple', 'explode': False }})  
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class GetModelCustomizationResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    model_customization: Optional[shared_modelcustomization.ModelCustomization] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    model_customization: Optional[shared_modelcustomization.ModelCustomization] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/getsubscriptiondetails.py` & `writerai-0.4.0/src/writer/models/operations/getsubscriptiondetails.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import subscriptionpublicresponseapi as shared_subscriptionpublicresponseapi
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetSubscriptionDetailsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    subscription_public_response_api: Optional[shared_subscriptionpublicresponseapi.SubscriptionPublicResponseAPI] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    subscription_public_response_api: Optional[shared_subscriptionpublicresponseapi.SubscriptionPublicResponseAPI] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/listfiles.py` & `writerai-0.4.0/src/writer/models/operations/listmodelcustomizations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import customizationsresponse as shared_customizationsresponse
 from ..shared import failresponse as shared_failresponse
-from ..shared import modelfilesresponse as shared_modelfilesresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListFilesRequest:
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+class ListModelCustomizationsRequest:
+    
+    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class ListFilesResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+class ListModelCustomizationsResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    customizations_response: Optional[shared_customizationsresponse.CustomizationsResponse] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    model_files_response: Optional[shared_modelfilesresponse.ModelFilesResponse] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/listmodelcustomizations.py` & `writerai-0.4.0/src/writer/models/operations/pagedetails.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import customizationsresponse as shared_customizationsresponse
 from ..shared import failresponse as shared_failresponse
+from ..shared import pagewithsectionresponse as shared_pagewithsectionresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListModelCustomizationsRequest:
-    model_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'modelId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+class PageDetailsRequest:
+    
+    page_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'pageId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class ListModelCustomizationsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    customizations_response: Optional[shared_customizationsresponse.CustomizationsResponse] = dataclasses.field(default=None)
+class PageDetailsResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    page_with_section_response: Optional[shared_pagewithsectionresponse.PageWithSectionResponse] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/listmodels.py` & `writerai-0.4.0/src/writer/models/operations/listmodels.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import generationmodelsresponse as shared_generationmodelsresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListModelsRequest:
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class ListModelsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    generation_models_response: Optional[shared_generationmodelsresponse.GenerationModelsResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    generation_models_response: Optional[shared_generationmodelsresponse.GenerationModelsResponse] = dataclasses.field(default=None)  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/listpages.py` & `writerai-0.4.0/src/writer/models/operations/listpages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,34 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import paginatedresult_pagepublicapiresponse as shared_paginatedresult_pagepublicapiresponse
 from enum import Enum
 from typing import Optional
 
 class ListPagesStatusEnum(str, Enum):
-    LIVE = "live"
-    OFFLINE = "offline"
+    LIVE = 'live'
+    OFFLINE = 'offline'
 
 
 @dataclasses.dataclass
 class ListPagesRequest:
-    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-    status: Optional[ListPagesStatusEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'status', 'style': 'form', 'explode': True }})
+    
+    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})  
+    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})  
+    status: Optional[ListPagesStatusEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'status', 'style': 'form', 'explode': True }})  
     
 
 @dataclasses.dataclass
 class ListPagesResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    paginated_result_page_public_api_response: Optional[shared_paginatedresult_pagepublicapiresponse.PaginatedResultPagePublicAPIResponse] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    paginated_result_page_public_api_response: Optional[shared_paginatedresult_pagepublicapiresponse.PaginatedResultPagePublicAPIResponse] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/listtemplates.py` & `writerai-0.4.0/src/writer/models/operations/listtemplates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import templatedetailsresponse as shared_templatedetailsresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListTemplatesRequest:
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    template_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'templateId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+    
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
+    template_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'templateId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class ListTemplatesResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    template_details_response: Optional[shared_templatedetailsresponse.TemplateDetailsResponse] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    template_details_response: Optional[shared_templatedetailsresponse.TemplateDetailsResponse] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/listusers.py` & `writerai-0.4.0/src/writer/models/operations/listusers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,45 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import paginatedresult_userpublicresponse as shared_paginatedresult_userpublicresponse
 from enum import Enum
 from typing import Optional
 
 class ListUsersSortFieldEnum(str, Enum):
-    ID = "id"
-    NAME = "name"
-    CREATION_TIME = "creationTime"
-    DELETED = "deleted"
-    MODIFICATION_TIME = "modificationTime"
-    EMAIL = "email"
-    LAST_SEEN = "lastSeen"
+    ID = 'id'
+    NAME = 'name'
+    CREATION_TIME = 'creationTime'
+    DELETED = 'deleted'
+    MODIFICATION_TIME = 'modificationTime'
+    EMAIL = 'email'
+    LAST_SEEN = 'lastSeen'
 
 class ListUsersSortOrderEnum(str, Enum):
-    ASC = "asc"
-    DESC = "desc"
+    ASC = 'asc'
+    DESC = 'desc'
 
 
 @dataclasses.dataclass
 class ListUsersRequest:
-    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-    search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})
-    sort_field: Optional[ListUsersSortFieldEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})
-    sort_order: Optional[ListUsersSortOrderEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})
+    
+    limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})  
+    offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})  
+    search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})  
+    sort_field: Optional[ListUsersSortFieldEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortField', 'style': 'form', 'explode': True }})  
+    sort_order: Optional[ListUsersSortOrderEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sortOrder', 'style': 'form', 'explode': True }})  
     
 
 @dataclasses.dataclass
 class ListUsersResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    paginated_result_user_public_response: Optional[shared_paginatedresult_userpublicresponse.PaginatedResultUserPublicResponse] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    paginated_result_user_public_response: Optional[shared_paginatedresult_userpublicresponse.PaginatedResultUserPublicResponse] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/pagedetails.py` & `writerai-0.4.0/src/writer/models/operations/uploadfile.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
-from ..shared import pagewithsectionresponse as shared_pagewithsectionresponse
+from ..shared import modelfile as shared_modelfile
+from ..shared import uploadmodelfilerequest as shared_uploadmodelfilerequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class PageDetailsRequest:
-    page_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'pageId', 'style': 'simple', 'explode': False }})
+class UploadFileRequest:
+    
+    upload_model_file_request: shared_uploadmodelfilerequest.UploadModelFileRequest = dataclasses.field(metadata={'request': { 'media_type': 'multipart/form-data' }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class PageDetailsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+class UploadFileResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    page_with_section_response: Optional[shared_pagewithsectionresponse.PageWithSectionResponse] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    model_file: Optional[shared_modelfile.ModelFile] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/updatesnippets.py` & `writerai-0.4.0/src/writer/models/operations/updatesnippets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import failresponse as shared_failresponse
 from ..shared import snippetupdate as shared_snippetupdate
 from ..shared import snippetwithuser as shared_snippetwithuser
 from typing import Optional
 
 
 @dataclasses.dataclass
 class UpdateSnippetsRequest:
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
-    request_body: Optional[list[shared_snippetupdate.SnippetUpdate]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
+    
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+    request_body: Optional[list[shared_snippetupdate.SnippetUpdate]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class UpdateSnippetsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    snippet_with_users: Optional[list[shared_snippetwithuser.SnippetWithUser]] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    snippet_with_users: Optional[list[shared_snippetwithuser.SnippetWithUser]] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/updateterms.py` & `writerai-0.4.0/src/writer/models/operations/updateterms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import createtermsresponse as shared_createtermsresponse
 from ..shared import failresponse as shared_failresponse
 from ..shared import updatetermsrequest as shared_updatetermsrequest
 from typing import Optional
 
 
 @dataclasses.dataclass
 class UpdateTermsRequest:
-    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})
-    update_terms_request: shared_updatetermsrequest.UpdateTermsRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
-    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})
+    
+    team_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'teamId', 'style': 'simple', 'explode': False }})  
+    update_terms_request: shared_updatetermsrequest.UpdateTermsRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})  
+    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})  
+    x_request_id: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Request-ID', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class UpdateTermsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    create_terms_response: Optional[shared_createtermsresponse.CreateTermsResponse] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    create_terms_response: Optional[shared_createtermsresponse.CreateTermsResponse] = dataclasses.field(default=None)  
     fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `writerai-0.3.1/src/writer/models/operations/uploadfile.py` & `writerai-0.4.0/src/writer/models/shared/createtermsresponse.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,18 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import failresponse as shared_failresponse
-from ..shared import modelfile as shared_modelfile
-from ..shared import uploadmodelfilerequest as shared_uploadmodelfilerequest
+from ..shared import failmessage as shared_failmessage
+from ..shared import fulltermwithuser as shared_fulltermwithuser
+from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
+from writer import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UploadFileRequest:
-    upload_model_file_request: shared_uploadmodelfilerequest.UploadModelFileRequest = dataclasses.field(metadata={'request': { 'media_type': 'multipart/form-data' }})
-    organization_id: Optional[int] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'organizationId', 'style': 'simple', 'explode': False }})
+class CreateTermsResponse:
     
-
-@dataclasses.dataclass
-class UploadFileResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    fail_response: Optional[shared_failresponse.FailResponse] = dataclasses.field(default=None)
-    headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
-    model_file: Optional[shared_modelfile.ModelFile] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    fails: Optional[list[shared_failmessage.FailMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fails'), 'exclude': lambda f: f is None }})  
+    models: Optional[list[shared_fulltermwithuser.FullTermWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/__init__.py` & `writerai-0.4.0/src/writer/models/shared/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from .approvedtermextension import *
 from .approvedtermextensioncreate import *
 from .completiongenerationchoice import *
 from .completiongenerationchoicelogprobs import *
 from .completionrequest import *
 from .completionresponse import *
 from .contentdetectorrequest import *
```

### Comparing `writerai-0.3.1/src/writer/models/shared/approvedtermextension.py` & `writerai-0.4.0/src/writer/models/shared/approvedtermextension.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ApprovedTermExtension:
-    capitalize: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('capitalize') }})
-    fix_case: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCase') }})
-    fix_common_mistakes: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCommonMistakes') }})
-    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    
+    capitalize: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('capitalize') }})  
+    fix_case: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCase') }})  
+    fix_common_mistakes: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCommonMistakes') }})  
+    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})  
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/approvedtermextensioncreate.py` & `writerai-0.4.0/src/writer/models/shared/magicrequestinput.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
+from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ApprovedTermExtensionCreate:
-    capitalize: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('capitalize') }})
-    fix_case: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCase') }})
-    fix_common_mistakes: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixCommonMistakes') }})
+class MagicRequestInput:
+    
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
+    value: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/completiongenerationchoice.py` & `writerai-0.4.0/src/writer/models/shared/completiongenerationchoice.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from ..shared import completiongenerationchoicelogprobs as shared_completiongenerationchoicelogprobs
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CompletionGenerationChoice:
-    text: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text') }})
-    logprobs: Optional[shared_completiongenerationchoicelogprobs.CompletionGenerationChoiceLogprobs] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logprobs'), 'exclude': lambda f: f is None }})
+    
+    text: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text') }})  
+    logprobs: Optional[shared_completiongenerationchoicelogprobs.CompletionGenerationChoiceLogprobs] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logprobs'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/completiongenerationchoicelogprobs.py` & `writerai-0.4.0/src/writer/models/shared/completiongenerationchoicelogprobs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CompletionGenerationChoiceLogprobs:
-    text_offset: Optional[list[int]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('textOffset'), 'exclude': lambda f: f is None }})
-    token_logprobs: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tokenLogprobs'), 'exclude': lambda f: f is None }})
-    tokens: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tokens'), 'exclude': lambda f: f is None }})
-    top_logprobs: Optional[list[dict[str, str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topLogprobs'), 'exclude': lambda f: f is None }})
+    
+    text_offset: Optional[list[int]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('textOffset'), 'exclude': lambda f: f is None }})  
+    token_logprobs: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tokenLogprobs'), 'exclude': lambda f: f is None }})  
+    tokens: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tokens'), 'exclude': lambda f: f is None }})  
+    top_logprobs: Optional[list[dict[str, str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topLogprobs'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/completionrequest.py` & `writerai-0.4.0/src/writer/models/shared/input.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from typing import Optional
 from writer import utils
 
+class InputTypeEnum(str, Enum):
+    TEXTBOX = 'textbox'
+    TEXTAREA = 'textarea'
+    DROPDOWN = 'dropdown'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class CompletionRequest:
-    prompt: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt') }})
-    best_of: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bestOf'), 'exclude': lambda f: f is None }})
-    frequency_penalty: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('frequencyPenalty'), 'exclude': lambda f: f is None }})
-    logprobs: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logprobs'), 'exclude': lambda f: f is None }})
-    max_tokens: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxTokens'), 'exclude': lambda f: f is None }})
-    min_tokens: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minTokens'), 'exclude': lambda f: f is None }})
-    n: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('n'), 'exclude': lambda f: f is None }})
-    presence_penalty: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presencePenalty'), 'exclude': lambda f: f is None }})
-    stop: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stop'), 'exclude': lambda f: f is None }})
-    temperature: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('temperature'), 'exclude': lambda f: f is None }})
-    top_p: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topP'), 'exclude': lambda f: f is None }})
+class Input:
+    
+    dynamic: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dynamic') }})  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
+    required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})  
+    type: InputTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
+    help: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('help'), 'exclude': lambda f: f is None }})  
+    max_fields: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxFields'), 'exclude': lambda f: f is None }})  
+    min_fields: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minFields'), 'exclude': lambda f: f is None }})  
+    options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})  
+    subtitle: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtitle'), 'exclude': lambda f: f is None }})  
+    unit_copy: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unitCopy'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/completionresponse.py` & `writerai-0.4.0/src/writer/models/shared/completionresponse.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from ..shared import completiongenerationchoice as shared_completiongenerationchoice
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CompletionResponse:
-    choices: Optional[list[shared_completiongenerationchoice.CompletionGenerationChoice]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('choices'), 'exclude': lambda f: f is None }})
+    
+    choices: Optional[list[shared_completiongenerationchoice.CompletionGenerationChoice]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('choices'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/contentdetectorresponse.py` & `writerai-0.4.0/src/writer/models/shared/contentdetectorresponse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from writer import utils
 
 class ContentDetectorResponseLabelEnum(str, Enum):
-    FAKE = "fake"
-    REAL = "real"
+    FAKE = 'fake'
+    REAL = 'real'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ContentDetectorResponse:
-    label: ContentDetectorResponseLabelEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label') }})
-    score: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('score') }})
+    
+    label: ContentDetectorResponseLabelEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label') }})  
+    score: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('score') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/contentissue.py` & `writerai-0.4.0/src/writer/models/shared/contentissue.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,60 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Any, Optional
 from writer import utils
 
 class ContentIssueServiceEnum(str, Enum):
-    COMMON_MISTAKES = "common-mistakes"
-    BANNED_WORDS = "banned-words"
-    DICTIONARY = "dictionary"
-    GEC = "gec"
-    INFINITIVE = "infinitive"
-    SPELLING = "spelling"
-    WRITING_STYLE = "writing-style"
-    CUSTOM_RULES = "custom-rules"
-    SENTENCE_CASE = "sentence-case"
-    ACRONYM = "acronym"
-    OXFORD_COMMA = "oxford-comma"
-    ML_PUNCTUATION = "ml-punctuation"
-    EMOJIS = "emojis"
-    GENDER_PRONOUNS = "gender-pronouns"
-    SENSITIVITY = "sensitivity"
-    PLAGIARISM = "plagiarism"
-    READABILITY = "readability"
-    SENTENCE_COMPLEXITY = "sentence-complexity"
-    VOCABULARY = "vocabulary"
-    PARAGRAPH_LENGTH = "paragraph-length"
-    PLAIN_LANGUAGE = "plain-language"
-    HEALTHY_COMMN = "healthy-commn"
-    CONFIDENCE = "confidence"
-    DATA_LOSS_PREVENTION = "data-loss-prevention"
-    HATE_SPEECH = "hate-speech"
-    CONTENT_SAFEGUARDS = "content-safeguards"
-    FEEDBACK = "feedback"
-    CLAIM = "claim"
-    QUOTE = "quote"
-    GENDER_NOUNS = "gender-nouns"
-    GENDER_TONE = "gender-tone"
-    GRAMMAR = "grammar"
-    PUNCTUATION_DARK = "punctuation-dark"
-    FORMATTING = "formatting"
-    TWITTER = "twitter"
-    GEC_DARK = "gec-dark"
-    GEC_GPT3 = "gec-gpt3"
+    COMMON_MISTAKES = 'common-mistakes'
+    BANNED_WORDS = 'banned-words'
+    DICTIONARY = 'dictionary'
+    GEC = 'gec'
+    INFINITIVE = 'infinitive'
+    SPELLING = 'spelling'
+    WRITING_STYLE = 'writing-style'
+    CUSTOM_RULES = 'custom-rules'
+    SENTENCE_CASE = 'sentence-case'
+    ACRONYM = 'acronym'
+    OXFORD_COMMA = 'oxford-comma'
+    ML_PUNCTUATION = 'ml-punctuation'
+    EMOJIS = 'emojis'
+    GENDER_PRONOUNS = 'gender-pronouns'
+    SENSITIVITY = 'sensitivity'
+    PLAGIARISM = 'plagiarism'
+    READABILITY = 'readability'
+    SENTENCE_COMPLEXITY = 'sentence-complexity'
+    VOCABULARY = 'vocabulary'
+    PARAGRAPH_LENGTH = 'paragraph-length'
+    PLAIN_LANGUAGE = 'plain-language'
+    HEALTHY_COMMN = 'healthy-commn'
+    CONFIDENCE = 'confidence'
+    DATA_LOSS_PREVENTION = 'data-loss-prevention'
+    HATE_SPEECH = 'hate-speech'
+    CONTENT_SAFEGUARDS = 'content-safeguards'
+    FEEDBACK = 'feedback'
+    CLAIM = 'claim'
+    QUOTE = 'quote'
+    GENDER_NOUNS = 'gender-nouns'
+    GENDER_TONE = 'gender-tone'
+    GRAMMAR = 'grammar'
+    PUNCTUATION_DARK = 'punctuation-dark'
+    FORMATTING = 'formatting'
+    TWITTER = 'twitter'
+    GEC_DARK = 'gec-dark'
+    GEC_GPT3 = 'gec-gpt3'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ContentIssue:
-    from_: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from') }})
-    service: ContentIssueServiceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service') }})
-    until: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('until') }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    meta: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta'), 'exclude': lambda f: f is None }})
-    suggestions: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('suggestions'), 'exclude': lambda f: f is None }})
+    
+    from_: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from') }})  
+    service: ContentIssueServiceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service') }})  
+    until: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('until') }})  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
+    meta: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta'), 'exclude': lambda f: f is None }})  
+    suggestions: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('suggestions'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/contentrequest.py` & `writerai-0.4.0/src/writer/models/shared/contentrequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from ..shared import contentsettings as shared_contentsettings
 from dataclasses_json import Undefined, dataclass_json
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ContentRequest:
-    content: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content') }})
-    settings: shared_contentsettings.ContentSettings = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('settings') }})
+    
+    content: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content') }})  
+    settings: shared_contentsettings.ContentSettings = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('settings') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/contentsettings.py` & `writerai-0.4.0/src/writer/models/shared/contentsettings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ContentSettings:
-    age_and_family_status: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ageAndFamilyStatus') }})
-    confidence: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('confidence') }})
-    content_safeguards: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentSafeguards') }})
-    disability: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disability') }})
-    gender_identity_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderIdentitySensitivity') }})
-    gender_inclusive_nouns: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderInclusiveNouns') }})
-    gender_inclusive_pronouns: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderInclusivePronouns') }})
-    grammar: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grammar') }})
-    healthy_communication: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('healthyCommunication') }})
-    passive_voice: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('passiveVoice') }})
-    race_ethnicity_nationality_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raceEthnicityNationalitySensitivity') }})
-    sexual_orientation_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sexualOrientationSensitivity') }})
-    spelling: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('spelling') }})
-    substance_use_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('substanceUseSensitivity') }})
-    unclear_reference: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unclearReference') }})
-    wordiness: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('wordiness') }})
+    
+    age_and_family_status: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ageAndFamilyStatus') }})  
+    confidence: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('confidence') }})  
+    content_safeguards: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentSafeguards') }})  
+    disability: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disability') }})  
+    gender_identity_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderIdentitySensitivity') }})  
+    gender_inclusive_nouns: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderInclusiveNouns') }})  
+    gender_inclusive_pronouns: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('genderInclusivePronouns') }})  
+    grammar: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grammar') }})  
+    healthy_communication: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('healthyCommunication') }})  
+    passive_voice: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('passiveVoice') }})  
+    race_ethnicity_nationality_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raceEthnicityNationalitySensitivity') }})  
+    sexual_orientation_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sexualOrientationSensitivity') }})  
+    spelling: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('spelling') }})  
+    substance_use_sensitivity: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('substanceUseSensitivity') }})  
+    unclear_reference: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unclearReference') }})  
+    wordiness: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('wordiness') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/createcustomizationrequest.py` & `writerai-0.4.0/src/writer/models/shared/completionrequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-from ..shared import hyperparameters as shared_hyperparameters
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class CreateCustomizationRequest:
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    training_dataset_file_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trainingDatasetFileId') }})
-    additional_hyper_parameters: Optional[shared_hyperparameters.HyperParameters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalHyperParameters'), 'exclude': lambda f: f is None }})
-    batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batchSize'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    epochs: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('epochs'), 'exclude': lambda f: f is None }})
-    learning_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('learningRate'), 'exclude': lambda f: f is None }})
-    prompt_template: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptTemplate'), 'exclude': lambda f: f is None }})
-    validation_dataset_file_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validationDatasetFileId'), 'exclude': lambda f: f is None }})
+class CompletionRequest:
+    
+    prompt: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt') }})  
+    best_of: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bestOf'), 'exclude': lambda f: f is None }})  
+    frequency_penalty: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('frequencyPenalty'), 'exclude': lambda f: f is None }})  
+    logprobs: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logprobs'), 'exclude': lambda f: f is None }})  
+    max_tokens: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxTokens'), 'exclude': lambda f: f is None }})  
+    min_tokens: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minTokens'), 'exclude': lambda f: f is None }})  
+    n: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('n'), 'exclude': lambda f: f is None }})  
+    presence_penalty: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presencePenalty'), 'exclude': lambda f: f is None }})  
+    stop: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stop'), 'exclude': lambda f: f is None }})  
+    temperature: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('temperature'), 'exclude': lambda f: f is None }})  
+    top_p: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topP'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/createtermsrequest.py` & `writerai-0.4.0/src/writer/models/shared/updatetermsrequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-from ..shared import termcreate as shared_termcreate
+from ..shared import termupdate as shared_termupdate
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
-class CreateTermsRequestFailHandlingEnum(str, Enum):
-    ACCUMULATE = "accumulate"
-    VALIDATE = "validate"
-    SKIP = "skip"
-    VALIDATE_ONLY = "validateOnly"
+class UpdateTermsRequestFailHandlingEnum(str, Enum):
+    ACCUMULATE = 'accumulate'
+    VALIDATE = 'validate'
+    SKIP = 'skip'
+    VALIDATE_ONLY = 'validateOnly'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class CreateTermsRequest:
-    fail_handling: Optional[CreateTermsRequestFailHandlingEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('failHandling'), 'exclude': lambda f: f is None }})
-    models: Optional[list[shared_termcreate.TermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})
+class UpdateTermsRequest:
+    
+    fail_handling: Optional[UpdateTermsRequestFailHandlingEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('failHandling'), 'exclude': lambda f: f is None }})  
+    models: Optional[list[shared_termupdate.TermUpdate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/createtermsresponse.py` & `writerai-0.4.0/src/writer/models/shared/pagination.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-from ..shared import failmessage as shared_failmessage
-from ..shared import fulltermwithuser as shared_fulltermwithuser
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class CreateTermsResponse:
-    fails: Optional[list[shared_failmessage.FailMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fails'), 'exclude': lambda f: f is None }})
-    models: Optional[list[shared_fulltermwithuser.FullTermWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})
+class Pagination:
+    
+    limit: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit'), 'exclude': lambda f: f is None }})  
+    offset: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('offset'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/customizationsresponse.py` & `writerai-0.4.0/src/writer/models/shared/customizationsresponse.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from ..shared import modelcustomization as shared_modelcustomization
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CustomizationsResponse:
-    customizations: Optional[list[shared_modelcustomization.ModelCustomization]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customizations'), 'exclude': lambda f: f is None }})
+    
+    customizations: Optional[list[shared_modelcustomization.ModelCustomization]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customizations'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/draft.py` & `writerai-0.4.0/src/writer/models/shared/draft.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from typing import Any, Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Draft:
-    body: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body') }})
-    created_user_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUserId') }})
-    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    deleted: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deleted') }})
-    document_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('documentId') }})
-    inputs: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs') }})
-    organization_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('organizationId') }})
-    team_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('teamId') }})
-    template_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('templateId') }})
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
+    
+    body: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body') }})  
+    created_user_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUserId') }})  
+    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    deleted: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deleted') }})  
+    document_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('documentId') }})  
+    inputs: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs') }})  
+    organization_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('organizationId') }})  
+    team_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('teamId') }})  
+    template_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('templateId') }})  
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
+    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/failmessage.py` & `writerai-0.4.0/src/writer/models/shared/usageitem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Any
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class FailMessage:
-    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
-    extras: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extras') }})
-    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
+class UsageItem:
+    
+    limit: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit') }})  
+    value: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/failresponse.py` & `writerai-0.4.0/src/writer/models/shared/simpleuser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-from ..shared import failmessage as shared_failmessage
 from dataclasses_json import Undefined, dataclass_json
-from typing import Any, Optional
+from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class FailResponse:
-    extras: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extras') }})
-    tpe: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tpe') }})
-    errors: Optional[list[shared_failmessage.FailMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})
+class SimpleUser:
+    
+    first_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName') }})  
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})  
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/fulllinkedterm.py` & `writerai-0.4.0/src/writer/models/shared/fulllinkedterm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from ..shared import approvedtermextension as shared_approvedtermextension
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
 class FullLinkedTermPosEnum(str, Enum):
-    NOUN = "noun"
-    VERB = "verb"
-    ADVERB = "adverb"
-    ADJECTIVE = "adjective"
+    NOUN = 'noun'
+    VERB = 'verb'
+    ADVERB = 'adverb'
+    ADJECTIVE = 'adjective'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class FullLinkedTerm:
-    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
-    linked_term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTermId') }})
-    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})
-    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})
-    approved_term_extension: Optional[shared_approvedtermextension.ApprovedTermExtension] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    pos: Optional[FullLinkedTermPosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
+    
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})  
+    linked_term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTermId') }})  
+    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})  
+    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})  
+    approved_term_extension: Optional[shared_approvedtermextension.ApprovedTermExtension] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})  
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
+    pos: Optional[FullLinkedTermPosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/fulltermwithuser.py` & `writerai-0.4.0/src/writer/models/shared/fulltermwithuser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import approvedtermextension as shared_approvedtermextension
 from ..shared import fulllinkedterm as shared_fulllinkedterm
 from ..shared import termexample as shared_termexample
 from ..shared import terminologyuser as shared_terminologyuser
@@ -11,40 +13,41 @@
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
 class FullTermWithUserPosEnum(str, Enum):
-    NOUN = "noun"
-    VERB = "verb"
-    ADVERB = "adverb"
-    ADJECTIVE = "adjective"
+    NOUN = 'noun'
+    VERB = 'verb'
+    ADVERB = 'adverb'
+    ADJECTIVE = 'adjective'
 
 class FullTermWithUserTypeEnum(str, Enum):
-    APPROVED = "approved"
-    BANNED = "banned"
-    PENDING = "pending"
+    APPROVED = 'approved'
+    BANNED = 'banned'
+    PENDING = 'pending'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class FullTermWithUser:
-    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
-    created_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUser') }})
-    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    highlight: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight') }})
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    modified_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedUser') }})
-    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})
-    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})
-    type: FullTermWithUserTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    approved_term_extension: Optional[shared_approvedtermextension.ApprovedTermExtension] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})
-    backlinked_terms: Optional[list[shared_fulllinkedterm.FullLinkedTerm]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('backlinkedTerms'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    examples: Optional[list[shared_termexample.TermExample]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})
-    linked_terms: Optional[list[shared_fulllinkedterm.FullLinkedTerm]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})
-    mistakes: Optional[list[shared_termmistake.TermMistake]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})
-    pos: Optional[FullTermWithUserPosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
-    tags: Optional[list[shared_termtagresponse.TermTagResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
+    
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})  
+    created_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUser') }})  
+    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    highlight: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight') }})  
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    modified_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedUser') }})  
+    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})  
+    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})  
+    type: FullTermWithUserTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
+    approved_term_extension: Optional[shared_approvedtermextension.ApprovedTermExtension] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})  
+    backlinked_terms: Optional[list[shared_fulllinkedterm.FullLinkedTerm]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('backlinkedTerms'), 'exclude': lambda f: f is None }})  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
+    examples: Optional[list[shared_termexample.TermExample]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})  
+    linked_terms: Optional[list[shared_fulllinkedterm.FullLinkedTerm]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})  
+    mistakes: Optional[list[shared_termmistake.TermMistake]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})  
+    pos: Optional[FullTermWithUserPosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})  
+    tags: Optional[list[shared_termtagresponse.TermTagResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/generatetemplaterequest.py` & `writerai-0.4.0/src/writer/models/shared/termexample.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,24 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-from ..shared import magicrequestinput as shared_magicrequestinput
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from typing import Optional
 from writer import utils
 
+class TermExampleTypeEnum(str, Enum):
+    GOOD = 'good'
+    BAD = 'bad'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GenerateTemplateRequest:
-    template_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('templateId') }})
-    inputs: Optional[list[shared_magicrequestinput.MagicRequestInput]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs'), 'exclude': lambda f: f is None }})
+class TermExample:
+    
+    example: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('example') }})  
+    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})  
+    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})  
+    type: TermExampleTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/generationmodelinforesponse.py` & `writerai-0.4.0/src/writer/models/shared/generationmodelinforesponse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from writer import utils
 
 class GenerationModelInfoResponseTypeEnum(str, Enum):
-    GPT = "GPT"
-    INSTRUCT = "Instruct"
+    GPT = 'GPT'
+    INSTRUCT = 'Instruct'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GenerationModelInfoResponse:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    type: GenerationModelInfoResponseTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
+    type: GenerationModelInfoResponseTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/generationmodelsresponse.py` & `writerai-0.4.0/src/writer/models/shared/terminologyuser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-from ..shared import generationmodelinforesponse as shared_generationmodelinforesponse
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GenerationModelsResponse:
-    data: Optional[list[shared_generationmodelinforesponse.GenerationModelInfoResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+class TerminologyUser:
+    
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})  
+    full_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullName'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/input.py` & `writerai-0.4.0/src/writer/models/shared/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
-class InputTypeEnum(str, Enum):
-    TEXTBOX = "textbox"
-    TEXTAREA = "textarea"
-    DROPDOWN = "dropdown"
+class MetaDataTierEnum(str, Enum):
+    ENTERPRISE_1 = 'enterprise-1'
+    ENTERPRISE_2 = 'enterprise-2'
+    ENTERPRISE_3 = 'enterprise-3'
+    ENTERPRISE_4 = 'enterprise-4'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Input:
-    dynamic: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dynamic') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})
-    type: InputTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    help: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('help'), 'exclude': lambda f: f is None }})
-    max_fields: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxFields'), 'exclude': lambda f: f is None }})
-    min_fields: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minFields'), 'exclude': lambda f: f is None }})
-    options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})
-    subtitle: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtitle'), 'exclude': lambda f: f is None }})
-    unit_copy: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unitCopy'), 'exclude': lambda f: f is None }})
+class MetaData:
+    
+    portal: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('portal') }})  
+    reporting: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reporting') }})  
+    snippets_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snippetsCount') }})  
+    sso_access: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssoAccess') }})  
+    styleguide: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('styleguide') }})  
+    team_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('teamCount') }})  
+    terms_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termsCount') }})  
+    tier: Optional[MetaDataTierEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tier'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/linkedtermcreate.py` & `writerai-0.4.0/src/writer/models/shared/linkedtermcreate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class LinkedTermCreate:
-    linked_term_id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTermId'), 'exclude': lambda f: f is None }})
-    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
+    
+    linked_term_id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTermId'), 'exclude': lambda f: f is None }})  
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/magicrequestinput.py` & `writerai-0.4.0/src/writer/models/shared/termtagresponse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class MagicRequestInput:
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    value: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
+class TermTagResponse:
+    
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    parent_tag_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentTagId') }})  
+    tag: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag') }})  
+    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/metadata.py` & `writerai-0.4.0/src/writer/models/shared/usage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,18 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
+from ..shared import usageitem as shared_usageitem
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-from typing import Optional
 from writer import utils
 
-class MetaDataTierEnum(str, Enum):
-    ENTERPRISE_1 = "enterprise-1"
-    ENTERPRISE_2 = "enterprise-2"
-    ENTERPRISE_3 = "enterprise-3"
-    ENTERPRISE_4 = "enterprise-4"
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class MetaData:
-    portal: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('portal') }})
-    reporting: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reporting') }})
-    snippets_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snippetsCount') }})
-    sso_access: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssoAccess') }})
-    styleguide: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('styleguide') }})
-    team_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('teamCount') }})
-    terms_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termsCount') }})
-    tier: Optional[MetaDataTierEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tier'), 'exclude': lambda f: f is None }})
+class Usage:
+    
+    co_write_words: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('coWriteWords') }})  
+    team: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('team') }})  
+    user: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user') }})  
+    words: shared_usageitem.UsageItem = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('words') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/modelcustomization.py` & `writerai-0.4.0/src/writer/models/shared/modelcustomization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,32 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import hyperparameters as shared_hyperparameters
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ModelCustomization:
-    base_model_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('baseModelId') }})
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    status: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    training_dataset_file_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trainingDatasetFileId') }})
-    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    additional_hyper_parameters: Optional[shared_hyperparameters.HyperParameters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalHyperParameters'), 'exclude': lambda f: f is None }})
-    batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batchSize'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    epochs: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('epochs'), 'exclude': lambda f: f is None }})
-    learning_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('learningRate'), 'exclude': lambda f: f is None }})
-    prompt_template: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptTemplate'), 'exclude': lambda f: f is None }})
-    validation_dataset_file_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validationDatasetFileId'), 'exclude': lambda f: f is None }})
+    
+    base_model_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('baseModelId') }})  
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
+    status: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})  
+    training_dataset_file_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trainingDatasetFileId') }})  
+    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    additional_hyper_parameters: Optional[shared_hyperparameters.HyperParameters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalHyperParameters'), 'exclude': lambda f: f is None }})  
+    batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batchSize'), 'exclude': lambda f: f is None }})  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
+    epochs: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('epochs'), 'exclude': lambda f: f is None }})  
+    learning_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('learningRate'), 'exclude': lambda f: f is None }})  
+    prompt_template: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptTemplate'), 'exclude': lambda f: f is None }})  
+    validation_dataset_file_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validationDatasetFileId'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/modelfile.py` & `writerai-0.4.0/src/writer/models/shared/modelfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ModelFile:
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    format: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    number_of_samples: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfSamples') }})
-    size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size') }})
+    
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    format: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
+    number_of_samples: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfSamples') }})  
+    size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/modelfilesresponse.py` & `writerai-0.4.0/src/writer/models/shared/modelfilesresponse.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from ..shared import modelfile as shared_modelfile
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ModelFilesResponse:
-    files: Optional[list[shared_modelfile.ModelFile]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('files'), 'exclude': lambda f: f is None }})
+    
+    files: Optional[list[shared_modelfile.ModelFile]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('files'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/pagepublicapiresponse.py` & `writerai-0.4.0/src/writer/models/shared/pagepublicapiresponse.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import sectioninfo as shared_sectioninfo
 from ..shared import simpleuser as shared_simpleuser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
 class PagePublicAPIResponseStatusEnum(str, Enum):
-    LIVE = "live"
-    OFFLINE = "offline"
+    LIVE = 'live'
+    OFFLINE = 'offline'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PagePublicAPIResponse:
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    order: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order') }})
-    status: PagePublicAPIResponseStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})
-    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
-    section: Optional[shared_sectioninfo.SectionInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('section'), 'exclude': lambda f: f is None }})
-    updated_by: Optional[shared_simpleuser.SimpleUser] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedBy'), 'exclude': lambda f: f is None }})
+    
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    order: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order') }})  
+    status: PagePublicAPIResponseStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})  
+    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})  
+    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})  
+    section: Optional[shared_sectioninfo.SectionInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('section'), 'exclude': lambda f: f is None }})  
+    updated_by: Optional[shared_simpleuser.SimpleUser] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedBy'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/pagewithsectionresponse.py` & `writerai-0.4.0/src/writer/models/shared/pagewithsectionresponse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import sectioninfo as shared_sectioninfo
 from ..shared import simpleuser as shared_simpleuser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
 class PageWithSectionResponseStatusEnum(str, Enum):
-    LIVE = "live"
-    OFFLINE = "offline"
+    LIVE = 'live'
+    OFFLINE = 'offline'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PageWithSectionResponse:
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    order: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order') }})
-    status: PageWithSectionResponseStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})
-    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
-    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
-    section: Optional[shared_sectioninfo.SectionInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('section'), 'exclude': lambda f: f is None }})
-    updated_by: Optional[shared_simpleuser.SimpleUser] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedBy'), 'exclude': lambda f: f is None }})
+    
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    order: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order') }})  
+    status: PageWithSectionResponseStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})  
+    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})  
+    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})  
+    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})  
+    section: Optional[shared_sectioninfo.SectionInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('section'), 'exclude': lambda f: f is None }})  
+    updated_by: Optional[shared_simpleuser.SimpleUser] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedBy'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/paginatedresult_fulltermwithuser.py` & `writerai-0.4.0/src/writer/models/shared/paginatedresult_pagepublicapiresponse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-from ..shared import fulltermwithuser as shared_fulltermwithuser
+from ..shared import pagepublicapiresponse as shared_pagepublicapiresponse
 from ..shared import pagination as shared_pagination
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PaginatedResultFullTermWithUser:
-    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})
-    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})
-    result: Optional[list[shared_fulltermwithuser.FullTermWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
+class PaginatedResultPagePublicAPIResponse:
+    
+    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})  
+    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})  
+    result: Optional[list[shared_pagepublicapiresponse.PagePublicAPIResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/paginatedresult_pagepublicapiresponse.py` & `writerai-0.4.0/src/writer/models/shared/paginatedresult_userpublicresponse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-from ..shared import pagepublicapiresponse as shared_pagepublicapiresponse
 from ..shared import pagination as shared_pagination
+from ..shared import userpublicresponse as shared_userpublicresponse
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PaginatedResultPagePublicAPIResponse:
-    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})
-    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})
-    result: Optional[list[shared_pagepublicapiresponse.PagePublicAPIResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
+class PaginatedResultUserPublicResponse:
+    
+    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})  
+    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})  
+    result: Optional[list[shared_userpublicresponse.UserPublicResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/paginatedresult_snippetwithuser.py` & `writerai-0.4.0/src/writer/models/shared/paginatedresult_snippetwithuser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from ..shared import pagination as shared_pagination
 from ..shared import snippetwithuser as shared_snippetwithuser
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PaginatedResultSnippetWithUser:
-    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})
-    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})
-    result: Optional[list[shared_snippetwithuser.SnippetWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
+    
+    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})  
+    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})  
+    result: Optional[list[shared_snippetwithuser.SnippetWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/paginatedresult_userpublicresponse.py` & `writerai-0.4.0/src/writer/models/shared/paginatedresult_fulltermwithuser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
+from ..shared import fulltermwithuser as shared_fulltermwithuser
 from ..shared import pagination as shared_pagination
-from ..shared import userpublicresponse as shared_userpublicresponse
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PaginatedResultUserPublicResponse:
-    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})
-    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})
-    result: Optional[list[shared_userpublicresponse.UserPublicResponse]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
+class PaginatedResultFullTermWithUser:
+    
+    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})  
+    total_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalCount') }})  
+    result: Optional[list[shared_fulltermwithuser.FullTermWithUser]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('result'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/pagination.py` & `writerai-0.4.0/src/writer/models/shared/sectioninfo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Pagination:
-    limit: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit'), 'exclude': lambda f: f is None }})
-    offset: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('offset'), 'exclude': lambda f: f is None }})
+class SectionInfo:
+    
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})  
+    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/processedcontent.py` & `writerai-0.4.0/src/writer/models/shared/processedcontent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from ..shared import contentissue as shared_contentissue
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ProcessedContent:
-    issues: Optional[list[shared_contentissue.ContentIssue]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('issues'), 'exclude': lambda f: f is None }})
+    
+    issues: Optional[list[shared_contentissue.ContentIssue]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('issues'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/sectioninfo.py` & `writerai-0.4.0/src/writer/models/shared/failmessage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
+from typing import Any
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SectionInfo:
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})
-    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
+class FailMessage:
+    
+    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})  
+    extras: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extras') }})  
+    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/snippetupdate.py` & `writerai-0.4.0/src/writer/models/shared/snippetupdate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from ..shared import snippettagv2 as shared_snippettagv2
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SnippetUpdate:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    snippet: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snippet') }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    shortcut: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shortcut'), 'exclude': lambda f: f is None }})
-    tags: Optional[list[shared_snippettagv2.SnippetTagV2]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
+    
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    snippet: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snippet') }})  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
+    shortcut: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shortcut'), 'exclude': lambda f: f is None }})  
+    tags: Optional[list[shared_snippettagv2.SnippetTagV2]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/snippetwithuser.py` & `writerai-0.4.0/src/writer/models/shared/snippetwithuser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import snippettagv2 as shared_snippettagv2
 from ..shared import terminologyuser as shared_terminologyuser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
@@ -9,17 +11,18 @@
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SnippetWithUser:
-    created_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUser') }})
-    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    modified_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedUser') }})
-    snippet: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snippet') }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    shortcut: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shortcut'), 'exclude': lambda f: f is None }})
-    tags: Optional[list[shared_snippettagv2.SnippetTagV2]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
+    
+    created_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdUser') }})  
+    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    modified_user: shared_terminologyuser.TerminologyUser = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedUser') }})  
+    snippet: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snippet') }})  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
+    shortcut: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shortcut'), 'exclude': lambda f: f is None }})  
+    tags: Optional[list[shared_snippettagv2.SnippetTagV2]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/subscriptionpublicresponseapi.py` & `writerai-0.4.0/src/writer/models/shared/subscriptionpublicresponseapi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,42 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import metadata as shared_metadata
 from ..shared import usage as shared_usage
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from writer import utils
 
 class SubscriptionPublicResponseAPIProductNameEnum(str, Enum):
-    FREE = "free"
-    PRO = "pro"
-    TEAM = "team"
-    ENTERPRISE = "enterprise"
-    LEGACY = "legacy"
+    FREE = 'free'
+    PRO = 'pro'
+    TEAM = 'team'
+    ENTERPRISE = 'enterprise'
+    LEGACY = 'legacy'
 
 class SubscriptionPublicResponseAPIStatusEnum(str, Enum):
-    TRIALING = "trialing"
-    ACTIVE = "active"
-    PAST_DUE = "past_due"
-    INCOMPLETE = "incomplete"
-    INCOMPLETE_EXPIRED = "incomplete_expired"
-    UNPAID = "unpaid"
-    CANCELED = "canceled"
+    TRIALING = 'trialing'
+    ACTIVE = 'active'
+    PAST_DUE = 'past_due'
+    INCOMPLETE = 'incomplete'
+    INCOMPLETE_EXPIRED = 'incomplete_expired'
+    UNPAID = 'unpaid'
+    CANCELED = 'canceled'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SubscriptionPublicResponseAPI:
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    meta: shared_metadata.MetaData = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta') }})
-    product_name: SubscriptionPublicResponseAPIProductNameEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('productName') }})
-    seats: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seats') }})
-    status: SubscriptionPublicResponseAPIStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    subscription_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subscriptionId') }})
-    usage: shared_usage.Usage = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('usage') }})
+    
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    meta: shared_metadata.MetaData = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta') }})  
+    product_name: SubscriptionPublicResponseAPIProductNameEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('productName') }})  
+    seats: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seats') }})  
+    status: SubscriptionPublicResponseAPIStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})  
+    subscription_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subscriptionId') }})  
+    usage: shared_usage.Usage = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('usage') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/templatedetailsresponse.py` & `writerai-0.4.0/src/writer/models/shared/templatedetailsresponse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import input as shared_input
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TemplateDetailsResponse:
-    category_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('categoryId') }})
-    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    guide_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guideUrl'), 'exclude': lambda f: f is None }})
-    inputs: Optional[list[shared_input.Input]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs'), 'exclude': lambda f: f is None }})
+    
+    category_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('categoryId') }})  
+    creation_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    modification_time: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modificationTime'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
+    guide_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guideUrl'), 'exclude': lambda f: f is None }})  
+    inputs: Optional[list[shared_input.Input]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/termcreate.py` & `writerai-0.4.0/src/writer/models/shared/termcreate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,43 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from ..shared import approvedtermextensioncreate as shared_approvedtermextensioncreate
 from ..shared import linkedtermcreate as shared_linkedtermcreate
 from ..shared import termexamplecreate as shared_termexamplecreate
 from ..shared import termmistakecreate as shared_termmistakecreate
 from ..shared import termtagcreate as shared_termtagcreate
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
 class TermCreatePosEnum(str, Enum):
-    NOUN = "noun"
-    VERB = "verb"
-    ADVERB = "adverb"
-    ADJECTIVE = "adjective"
+    NOUN = 'noun'
+    VERB = 'verb'
+    ADVERB = 'adverb'
+    ADJECTIVE = 'adjective'
 
 class TermCreateTypeEnum(str, Enum):
-    APPROVED = "approved"
-    BANNED = "banned"
-    PENDING = "pending"
+    APPROVED = 'approved'
+    BANNED = 'banned'
+    PENDING = 'pending'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TermCreate:
-    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
-    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})
-    type: TermCreateTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    approved_term_extension: Optional[shared_approvedtermextensioncreate.ApprovedTermExtensionCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    examples: Optional[list[shared_termexamplecreate.TermExampleCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})
-    highlight: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight'), 'exclude': lambda f: f is None }})
-    linked_terms: Optional[list[shared_linkedtermcreate.LinkedTermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})
-    mistakes: Optional[list[shared_termmistakecreate.TermMistakeCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})
-    pos: Optional[TermCreatePosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
-    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
-    tags: Optional[list[shared_termtagcreate.TermTagCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
+    
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})  
+    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})  
+    type: TermCreateTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
+    approved_term_extension: Optional[shared_approvedtermextensioncreate.ApprovedTermExtensionCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
+    examples: Optional[list[shared_termexamplecreate.TermExampleCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})  
+    highlight: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight'), 'exclude': lambda f: f is None }})  
+    linked_terms: Optional[list[shared_linkedtermcreate.LinkedTermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})  
+    mistakes: Optional[list[shared_termmistakecreate.TermMistakeCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})  
+    pos: Optional[TermCreatePosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})  
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})  
+    tags: Optional[list[shared_termtagcreate.TermTagCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/termexample.py` & `writerai-0.4.0/src/writer/models/shared/generatetemplaterequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,17 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
+from ..shared import magicrequestinput as shared_magicrequestinput
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from typing import Optional
 from writer import utils
 
-class TermExampleTypeEnum(str, Enum):
-    GOOD = "good"
-    BAD = "bad"
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TermExample:
-    example: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('example') }})
-    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})
-    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})
-    type: TermExampleTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+class GenerateTemplateRequest:
+    
+    template_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('templateId') }})  
+    inputs: Optional[list[shared_magicrequestinput.MagicRequestInput]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/termexamplecreate.py` & `writerai-0.4.0/src/writer/models/shared/termexamplecreate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from writer import utils
 
 class TermExampleCreateTypeEnum(str, Enum):
-    GOOD = "good"
-    BAD = "bad"
+    GOOD = 'good'
+    BAD = 'bad'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TermExampleCreate:
-    example: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('example') }})
-    type: TermExampleCreateTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    
+    example: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('example') }})  
+    type: TermExampleCreateTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/terminologyuser.py` & `writerai-0.4.0/src/writer/models/shared/failresponse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
+from ..shared import failmessage as shared_failmessage
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from writer import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TerminologyUser:
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    full_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullName'), 'exclude': lambda f: f is None }})
+class FailResponse:
+    r"""Bad Request"""
+    
+    extras: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extras') }})  
+    tpe: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tpe') }})  
+    errors: Optional[list[shared_failmessage.FailMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/termmistake.py` & `writerai-0.4.0/src/writer/models/shared/termmistake.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
 class TermMistakePosEnum(str, Enum):
-    NOUN = "noun"
-    VERB = "verb"
-    ADVERB = "adverb"
-    ADJECTIVE = "adjective"
+    NOUN = 'noun'
+    VERB = 'verb'
+    ADVERB = 'adverb'
+    ADJECTIVE = 'adjective'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TermMistake:
-    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
-    mistake: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistake') }})
-    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})
-    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    pos: Optional[TermMistakePosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
+    
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})  
+    mistake: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistake') }})  
+    term_bank_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termBankId') }})  
+    term_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('termId') }})  
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
+    pos: Optional[TermMistakePosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/termmistakecreate.py` & `writerai-0.4.0/src/writer/models/shared/termmistakecreate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
 class TermMistakeCreatePosEnum(str, Enum):
-    NOUN = "noun"
-    VERB = "verb"
-    ADVERB = "adverb"
-    ADJECTIVE = "adjective"
+    NOUN = 'noun'
+    VERB = 'verb'
+    ADVERB = 'adverb'
+    ADJECTIVE = 'adjective'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TermMistakeCreate:
-    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
-    mistake: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistake') }})
-    pos: Optional[TermMistakeCreatePosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
-    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
+    
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})  
+    mistake: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistake') }})  
+    pos: Optional[TermMistakeCreatePosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})  
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/termupdate.py` & `writerai-0.4.0/src/writer/models/shared/termupdate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,43 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 from ..shared import approvedtermextensioncreate as shared_approvedtermextensioncreate
 from ..shared import linkedtermcreate as shared_linkedtermcreate
 from ..shared import termexamplecreate as shared_termexamplecreate
 from ..shared import termmistakecreate as shared_termmistakecreate
 from ..shared import termtagcreate as shared_termtagcreate
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
 class TermUpdatePosEnum(str, Enum):
-    NOUN = "noun"
-    VERB = "verb"
-    ADVERB = "adverb"
-    ADJECTIVE = "adjective"
+    NOUN = 'noun'
+    VERB = 'verb'
+    ADVERB = 'adverb'
+    ADJECTIVE = 'adjective'
 
 class TermUpdateTypeEnum(str, Enum):
-    APPROVED = "approved"
-    BANNED = "banned"
-    PENDING = "pending"
+    APPROVED = 'approved'
+    BANNED = 'banned'
+    PENDING = 'pending'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TermUpdate:
-    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})
-    type: TermUpdateTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    approved_term_extension: Optional[shared_approvedtermextensioncreate.ApprovedTermExtensionCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    examples: Optional[list[shared_termexamplecreate.TermExampleCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})
-    highlight: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight'), 'exclude': lambda f: f is None }})
-    linked_terms: Optional[list[shared_linkedtermcreate.LinkedTermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})
-    mistakes: Optional[list[shared_termmistakecreate.TermMistakeCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})
-    pos: Optional[TermUpdatePosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})
-    tags: Optional[list[shared_termtagcreate.TermTagCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
+    
+    case_sensitive: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('caseSensitive') }})  
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    term: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('term') }})  
+    type: TermUpdateTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
+    approved_term_extension: Optional[shared_approvedtermextensioncreate.ApprovedTermExtensionCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('approvedTermExtension'), 'exclude': lambda f: f is None }})  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
+    examples: Optional[list[shared_termexamplecreate.TermExampleCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('examples'), 'exclude': lambda f: f is None }})  
+    highlight: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highlight'), 'exclude': lambda f: f is None }})  
+    linked_terms: Optional[list[shared_linkedtermcreate.LinkedTermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkedTerms'), 'exclude': lambda f: f is None }})  
+    mistakes: Optional[list[shared_termmistakecreate.TermMistakeCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mistakes'), 'exclude': lambda f: f is None }})  
+    pos: Optional[TermUpdatePosEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pos'), 'exclude': lambda f: f is None }})  
+    tags: Optional[list[shared_termtagcreate.TermTagCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tags'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/updatetermsrequest.py` & `writerai-0.4.0/src/writer/models/shared/createtermsrequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-from ..shared import termupdate as shared_termupdate
+from ..shared import termcreate as shared_termcreate
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from writer import utils
 
-class UpdateTermsRequestFailHandlingEnum(str, Enum):
-    ACCUMULATE = "accumulate"
-    VALIDATE = "validate"
-    SKIP = "skip"
-    VALIDATE_ONLY = "validateOnly"
+class CreateTermsRequestFailHandlingEnum(str, Enum):
+    ACCUMULATE = 'accumulate'
+    VALIDATE = 'validate'
+    SKIP = 'skip'
+    VALIDATE_ONLY = 'validateOnly'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UpdateTermsRequest:
-    fail_handling: Optional[UpdateTermsRequestFailHandlingEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('failHandling'), 'exclude': lambda f: f is None }})
-    models: Optional[list[shared_termupdate.TermUpdate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})
+class CreateTermsRequest:
+    
+    fail_handling: Optional[CreateTermsRequestFailHandlingEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('failHandling'), 'exclude': lambda f: f is None }})  
+    models: Optional[list[shared_termcreate.TermCreate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('models'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models/shared/userpublicresponse.py` & `writerai-0.4.0/src/writer/models/shared/userpublicresponse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 from writer import utils
 
 class UserPublicResponseAccountStatusEnum(str, Enum):
-    INVITED = "invited"
-    SIGNED_UP = "signed_up"
+    INVITED = 'invited'
+    SIGNED_UP = 'signed_up'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UserPublicResponse:
-    account_status: UserPublicResponseAccountStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountStatus') }})
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    first_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName') }})
-    full_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullName') }})
-    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    avatar: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('avatar'), 'exclude': lambda f: f is None }})
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    invited_by: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invitedBy'), 'exclude': lambda f: f is None }})
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
-    last_seen_online: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSeenOnline'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    timezone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timezone'), 'exclude': lambda f: f is None }})
+    
+    account_status: UserPublicResponseAccountStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountStatus') }})  
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    first_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName') }})  
+    full_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullName') }})  
+    id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    avatar: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('avatar'), 'exclude': lambda f: f is None }})  
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})  
+    invited_by: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invitedBy'), 'exclude': lambda f: f is None }})  
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})  
+    last_seen_online: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSeenOnline'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})  
+    timezone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timezone'), 'exclude': lambda f: f is None }})
```

### Comparing `writerai-0.3.1/src/writer/models_.py` & `writerai-0.4.0/src/writer/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
-class Models:
+class User:
+    r"""Methods related to User"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -17,36 +20,35 @@
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
-    def list(self, request: operations.ListModelsRequest) -> operations.ListModelsResponse:
-        r"""List available LLM models
-        """
-        
+    def list(self, request: operations.ListUsersRequest) -> operations.ListUsersResponse:
+        r"""List users"""
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListModelsRequest, base_url, '/llm/organization/{organizationId}/model', request, self._globals)
+        url = base_url.removesuffix('/') + '/user'
         
+        query_params = utils.get_query_params(operations.ListUsersRequest, request, self._globals)
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListModelsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListUsersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.GenerationModelsResponse])
-                res.generation_models_response = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PaginatedResultUserPublicResponse])
+                res.paginated_result_user_public_response = out
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
```

### Comparing `writerai-0.3.1/src/writer/snippet.py` & `writerai-0.4.0/src/writer/snippet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
 class Snippet:
+    r"""Methods related to Snippets"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -18,17 +21,15 @@
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
     def delete(self, request: operations.DeleteSnippetsRequest) -> operations.DeleteSnippetsResponse:
-        r"""Delete snippets
-        """
-        
+        r"""Delete snippets"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.DeleteSnippetsRequest, base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, self._globals)
         
         headers = utils.get_headers(request)
         query_params = utils.get_query_params(operations.DeleteSnippetsRequest, request, self._globals)
         
@@ -51,17 +52,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def find(self, request: operations.FindSnippetsRequest) -> operations.FindSnippetsResponse:
-        r"""Find snippets
-        """
-        
+        r"""Find snippets"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.FindSnippetsRequest, base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, self._globals)
         
         query_params = utils.get_query_params(operations.FindSnippetsRequest, request, self._globals)
         
         client = self._security_client
@@ -83,17 +82,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def update(self, request: operations.UpdateSnippetsRequest) -> operations.UpdateSnippetsResponse:
-        r"""Update snippets
-        """
-        
+        r"""Update snippets"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateSnippetsRequest, base_url, '/snippet/organization/{organizationId}/team/{teamId}', request, self._globals)
         
         headers = utils.get_headers(request)
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
```

### Comparing `writerai-0.3.1/src/writer/styleguide.py` & `writerai-0.4.0/src/writer/styleguide.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
 class Styleguide:
+    r"""Methods related to Styleguide"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -18,17 +21,15 @@
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
     def get(self, request: operations.PageDetailsRequest) -> operations.PageDetailsResponse:
-        r"""Page details
-        """
-        
+        r"""Page details"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.PageDetailsRequest, base_url, '/styleguide/page/{pageId}', request, self._globals)
         
         
         client = self._security_client
         
@@ -49,17 +50,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def list_pages(self, request: operations.ListPagesRequest) -> operations.ListPagesResponse:
-        r"""List your styleguide pages
-        """
-        
+        r"""List your styleguide pages"""
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/styleguide/page'
         
         query_params = utils.get_query_params(operations.ListPagesRequest, request, self._globals)
         
         client = self._security_client
```

### Comparing `writerai-0.3.1/src/writer/terminology.py` & `writerai-0.4.0/src/writer/terminology.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
 class Terminology:
+    r"""Methods related to Terminology"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -18,17 +21,15 @@
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
     def add(self, request: operations.AddTermsRequest) -> operations.AddTermsResponse:
-        r"""Add terms
-        """
-        
+        r"""Add terms"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.AddTermsRequest, base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, self._globals)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "create_terms_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
@@ -55,17 +56,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def delete(self, request: operations.DeleteTermsRequest) -> operations.DeleteTermsResponse:
-        r"""Delete terms
-        """
-        
+        r"""Delete terms"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.DeleteTermsRequest, base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, self._globals)
         
         headers = utils.get_headers(request)
         query_params = utils.get_query_params(operations.DeleteTermsRequest, request, self._globals)
         
@@ -88,17 +87,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def find(self, request: operations.FindTermsRequest) -> operations.FindTermsResponse:
-        r"""Find terms
-        """
-        
+        r"""Find terms"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.FindTermsRequest, base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, self._globals)
         
         query_params = utils.get_query_params(operations.FindTermsRequest, request, self._globals)
         
         client = self._security_client
@@ -120,17 +117,15 @@
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
 
         return res
 
     def update(self, request: operations.UpdateTermsRequest) -> operations.UpdateTermsResponse:
-        r"""Update terms
-        """
-        
+        r"""Update terms"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateTermsRequest, base_url, '/terminology/organization/{organizationId}/team/{teamId}', request, self._globals)
         
         headers = utils.get_headers(request)
         req_content_type, data, form = utils.serialize_request_body(request, "update_terms_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
```

### Comparing `writerai-0.3.1/src/writer/user.py` & `writerai-0.4.0/src/writer/download_the_customized_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
 from typing import Any, Optional
 from writer.models import operations, shared
 
-class User:
+class DownloadTheCustomizedModel:
+    r"""Methods related to Download the customized model"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
     _globals: dict[str, dict[str, dict[str, Any]]]
@@ -17,37 +20,33 @@
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         self._globals = gbls
         
-    def list(self, request: operations.ListUsersRequest) -> operations.ListUsersResponse:
-        r"""List users
-        """
-        
+    def fetch_file(self, request: operations.FetchCustomizedModelFileRequest) -> operations.FetchCustomizedModelFileResponse:
+        r"""Download your fine-tuned model (available only for Palmyra Base and Palmyra Large)"""
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/user'
+        url = utils.generate_url(operations.FetchCustomizedModelFileRequest, base_url, '/llm/organization/{organizationId}/model/{modelId}/customization/{customizationId}/fetch', request, self._globals)
         
-        query_params = utils.get_query_params(operations.ListUsersRequest, request, self._globals)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListUsersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.FetchCustomizedModelFileResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.PaginatedResultUserPublicResponse])
-                res.paginated_result_user_public_response = out
+            if utils.match_content_type(content_type, 'application/octet-stream'):
+                res.fetch_customized_model_file_200_application_octet_stream_binary_string = http_res.content
         elif http_res.status_code in [400, 401, 403, 404, 500]:
             res.headers = http_res.headers
             
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.FailResponse])
                 res.fail_response = out
```

### Comparing `writerai-0.3.1/src/writer/utils/retries.py` & `writerai-0.4.0/src/writer/utils/retries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import random
 import time
 
 import requests
 
 
 class BackoffStrategy:
```

### Comparing `writerai-0.3.1/src/writer/utils/utils.py` & `writerai-0.4.0/src/writer/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import base64
 import json
 import re
 from dataclasses import Field, dataclass, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from email.message import Message
 from enum import Enum
@@ -146,70 +148,79 @@
         if request_metadata is not None:
             continue
 
         param_metadata = field.metadata.get('path_param')
         if param_metadata is None:
             continue
 
-        if param_metadata.get('style', 'simple') == 'simple':
-            param = getattr(
-                path_params, field.name) if path_params is not None else None
-            param = _populate_from_globals(
-                field.name, param, 'pathParam', gbls)
+        param = getattr(
+            path_params, field.name) if path_params is not None else None
+        param = _populate_from_globals(
+            field.name, param, 'pathParam', gbls)
 
-            if param is None:
-                continue
+        if param is None:
+            continue
 
-            if isinstance(param, list):
-                pp_vals: list[str] = []
-                for pp_val in param:
-                    if pp_val is None:
-                        continue
-                    pp_vals.append(_val_to_string(pp_val))
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            elif isinstance(param, dict):
-                pp_vals: list[str] = []
-                for pp_key in param:
-                    if param[pp_key] is None:
-                        continue
-                    if param_metadata.get('explode'):
-                        pp_vals.append(
-                            f"{pp_key}={_val_to_string(param[pp_key])}")
-                    else:
-                        pp_vals.append(
-                            f"{pp_key},{_val_to_string(param[pp_key])}")
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            elif not isinstance(param, (str, int, float, complex, bool)):
-                pp_vals: list[str] = []
-                param_fields: Tuple[Field, ...] = fields(param)
-                for param_field in param_fields:
-                    param_value_metadata = param_field.metadata.get(
-                        'path_param')
-                    if not param_value_metadata:
-                        continue
-
-                    parm_name = param_value_metadata.get(
-                        'field_name', field.name)
-
-                    param_field_val = getattr(param, param_field.name)
-                    if param_field_val is None:
-                        continue
-                    if param_metadata.get('explode'):
-                        pp_vals.append(
-                            f"{parm_name}={_val_to_string(param_field_val)}")
-                    else:
-                        pp_vals.append(
-                            f"{parm_name},{_val_to_string(param_field_val)}")
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            else:
+        f_name = param_metadata.get("field_name", field.name)
+        serialization = param_metadata.get('serialization', '')
+        if serialization != '':
+            serialized_params = _get_serialized_params(
+                param_metadata, f_name, param)
+            for key, value in serialized_params.items():
                 path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    '{' + key + '}', value, 1)
+        else:
+            if param_metadata.get('style', 'simple') == 'simple':
+                if isinstance(param, list):
+                    pp_vals: list[str] = []
+                    for pp_val in param:
+                        if pp_val is None:
+                            continue
+                        pp_vals.append(_val_to_string(pp_val))
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                elif isinstance(param, dict):
+                    pp_vals: list[str] = []
+                    for pp_key in param:
+                        if param[pp_key] is None:
+                            continue
+                        if param_metadata.get('explode'):
+                            pp_vals.append(
+                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        else:
+                            pp_vals.append(
+                                f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                elif not isinstance(param, (str, int, float, complex, bool)):
+                    pp_vals: list[str] = []
+                    param_fields: Tuple[Field, ...] = fields(param)
+                    for param_field in param_fields:
+                        param_value_metadata = param_field.metadata.get(
+                            'path_param')
+                        if not param_value_metadata:
+                            continue
+
+                        parm_name = param_value_metadata.get(
+                            'field_name', field.name)
+
+                        param_field_val = getattr(param, param_field.name)
+                        if param_field_val is None:
+                            continue
+                        if param_metadata.get('explode'):
+                            pp_vals.append(
+                                f"{parm_name}={_val_to_string(param_field_val)}")
+                        else:
+                            pp_vals.append(
+                                f"{parm_name},{_val_to_string(param_field_val)}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                else:
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
 
     return server_url.removesuffix("/") + path
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
@@ -240,16 +251,20 @@
             query_params, param_name) if query_params is not None else None
 
         value = _populate_from_globals(param_name, value, 'queryParam', gbls)
 
         f_name = metadata.get("field_name")
         serialization = metadata.get('serialization', '')
         if serialization != '':
-            params = params | _get_serialized_query_params(
-                metadata, f_name, value)
+            serialized_parms = _get_serialized_params(metadata, f_name, value)
+            for key, value in serialized_parms.items():
+                if key in params:
+                    params[key].extend(value)
+                else:
+                    params[key] = [value]
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
                     metadata, f_name, value)
             elif style == 'form':
                 params = params | _get_form_query_params(
@@ -276,16 +291,16 @@
 
         if value != '':
             headers[metadata.get('field_name', field.name)] = value
 
     return headers
 
 
-def _get_serialized_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
-    params: dict[str, list[str]] = {}
+def _get_serialized_params(metadata: dict, field_name: str, obj: any) -> dict[str, str]:
+    params: dict[str, str] = {}
 
     serialization = metadata.get('serialization', '')
     if serialization == 'json':
         params[metadata.get("field_name", field_name)] = marshal_json(obj)
 
     return params
```

### Comparing `writerai-0.3.1/src/writerai.egg-info/PKG-INFO` & `writerai-0.4.0/src/writerai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: writerai
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python SDK for Writer API
 Home-page: UNKNOWN
 Author: writerai
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <div align="center">
         <source srcset="https://user-images.githubusercontent.com/6267663/223574357-9a053550-02f9-49f1-b453-1b11db148d7b.svg" media="(prefers-color-scheme: dark)" width="500">
         <img src="https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-44e8-ac48-f9494101e1dc.svg" width="500">
     <h1>Python SDK</h1>
    <p>AI for everyone.</p>
    <a href="https://dev.writer.com/docs"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=000000&style=for-the-badge" /></a>
-   <a href="https://github.com/writerai/writer-client-sdk-python/actions"><img src="https://img.shields.io/github/actions/workflow/status/writerai/writer-client-sdk-python/speakeasy_generate.yaml?style=for-the-badge" /></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" /></a>
   <a href="https://github.com/writerai/writer-client-sdk-python/releases"><img src="https://img.shields.io/github/v/release/writerai/writer-client-sdk-python?sort=semver&style=for-the-badge" /></a>
 </div>
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
@@ -50,27 +49,27 @@
     ),
     organization_id=548814,
 )
 
 
 req = operations.DetectContentRequest(
     content_detector_request=shared.ContentDetectorRequest(
-        input="example",
+        input="provident",
     ),
 )
     
 res = s.ai_content_detector.detect(req)
 
 if res.content_detector_responses is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### ai_content_detector
 
 * `detect` - Content detector api
 
 ### billing
```

#### html2text {}

```diff
@@ -1,36 +1,34 @@
-Metadata-Version: 2.1 Name: writerai Version: 0.3.1 Summary: Python SDK for
+Metadata-Version: 2.1 Name: writerai Version: 0.4.0 Summary: Python SDK for
 Writer API Home-page: UNKNOWN Author: writerai License: UNKNOWN Platform:
 UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/markdown
   [https://user-images.githubusercontent.com/6267663/223574369-77805bfe-6d95-
                           44e8-ac48-f9494101e1dc.svg]
                            ****** Python SDK ******
                                AI for everyone.
            [https://img.shields.io/static/v1?label=Docs&message=API
- Ref&color=000000&style=for-the-badge] [https://img.shields.io/github/actions/
-              workflow/status/writerai/writer-client-sdk-python/
-  speakeasy_generate.yaml?style=for-the-badge] [https://img.shields.io/badge/
-  License-MIT-blue.svg?style=for-the-badge] [https://img.shields.io/github/v/
-  release/writerai/writer-client-sdk-python?sort=semver&style=for-the-badge]
+ Ref&color=000000&style=for-the-badge] [https://img.shields.io/badge/License-
+  MIT-blue.svg?style=for-the-badge] [https://img.shields.io/github/v/release/
+      writerai/writer-client-sdk-python?sort=semver&style=for-the-badge]
  ## SDK Installation ```bash pip install writerai ```  ## Authentication Writer
 authenticates your API requests using your accountâs API keys. If you do not
 include your key when making an API request, or use one that is incorrect or
 outdated, Writer returns an error. Your API keys are available in the account
 dashboard. We include randomly generated API keys in our code examples if you
 are not logged in. Replace these with your own or log in to see code examples
 populated with your own API keys. [writer-auth] If you cannot see your secret
 API keys in the Dashboard, this means you do not have access to them. Contact
 your Writer account owner and ask to be added to their team as a developer. ##
 SDK Example Usage  ```python import writer from writer.models import
 operations, shared s = writer.Writer( security=shared.Security
 ( api_key="YOUR_API_KEY_HERE", ), organization_id=548814, ) req =
 operations.DetectContentRequest
-( content_detector_request=shared.ContentDetectorRequest( input="example", ), )
-res = s.ai_content_detector.detect(req) if res.content_detector_responses is
-not None: # handle response ```   ## SDK Available Operations ###
+( content_detector_request=shared.ContentDetectorRequest( input="provident", ),
+) res = s.ai_content_detector.detect(req) if res.content_detector_responses is
+not None: # handle response ```   ## Available Resources and Operations ###
 ai_content_detector * `detect` - Content detector api ### billing *
 `get_subscription_details` - Get your organization subscription details ###
 co_write * `generate_content` - Generate content using predefined templates *
 `list_templates` - Get a list of your existing CoWrite templates ###
 completions * `create` - Create completion for LLM model *
 `create_model_customization_completion` - Create completion for LLM
 customization model ### content * `check` - Check your content against your
```

### Comparing `writerai-0.3.1/src/writerai.egg-info/SOURCES.txt` & `writerai-0.4.0/src/writerai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

