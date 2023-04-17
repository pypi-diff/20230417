# Comparing `tmp/conllup-0.4.4.tar.gz` & `tmp/conllup-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conllup-0.4.4.tar", last modified: Wed Feb 22 20:55:03 2023, max compression
+gzip compressed data, was "conllup-0.4.5.tar", last modified: Fri Apr 14 16:26:49 2023, max compression
```

## Comparing `conllup-0.4.4.tar` & `conllup-0.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-02-22 20:55:03.408214 conllup-0.4.4/
--rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-02-22 20:55:03.408214 conllup-0.4.4/PKG-INFO
--rw-rw-r--   0 wran      (1000) wran      (1000)     3367 2023-02-22 20:47:32.000000 conllup-0.4.4/README.md
--rw-rw-r--   0 wran      (1000) wran      (1000)       24 2023-02-01 16:20:21.000000 conllup-0.4.4/long_description.rst
--rw-rw-r--   0 wran      (1000) wran      (1000)      246 2023-02-22 20:47:04.000000 conllup-0.4.4/pyproject.toml
--rw-rw-r--   0 wran      (1000) wran      (1000)      482 2023-02-22 20:55:03.408214 conllup-0.4.4/setup.cfg
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-02-22 20:55:03.408214 conllup-0.4.4/src/
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-02-22 20:55:03.408214 conllup-0.4.4/src/conllup/
--rw-rw-r--   0 wran      (1000) wran      (1000)        0 2023-01-30 16:14:25.000000 conllup-0.4.4/src/conllup/__init__.py
--rw-rw-r--   0 wran      (1000) wran      (1000)    11070 2023-02-22 20:46:03.000000 conllup-0.4.4/src/conllup/conllup.py
--rw-rw-r--   0 wran      (1000) wran      (1000)     6803 2023-02-07 18:51:16.000000 conllup-0.4.4/src/conllup/processing.py
--rw-rw-r--   0 wran      (1000) wran      (1000)      552 2023-02-02 18:44:41.000000 conllup-0.4.4/src/conllup/types.py
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-02-22 20:55:03.408214 conllup-0.4.4/src/conllup.egg-info/
--rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-02-22 20:55:03.000000 conllup-0.4.4/src/conllup.egg-info/PKG-INFO
--rw-rw-r--   0 wran      (1000) wran      (1000)      289 2023-02-22 20:55:03.000000 conllup-0.4.4/src/conllup.egg-info/SOURCES.txt
--rw-rw-r--   0 wran      (1000) wran      (1000)        1 2023-02-22 20:55:03.000000 conllup-0.4.4/src/conllup.egg-info/dependency_links.txt
--rw-rw-r--   0 wran      (1000) wran      (1000)        8 2023-02-22 20:55:03.000000 conllup-0.4.4/src/conllup.egg-info/top_level.txt
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-14 16:26:49.305427 conllup-0.4.5/
+-rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-04-14 16:26:49.305427 conllup-0.4.5/PKG-INFO
+-rw-rw-r--   0 wran      (1000) wran      (1000)     3385 2023-04-14 16:24:50.000000 conllup-0.4.5/README.md
+-rw-rw-r--   0 wran      (1000) wran      (1000)       24 2023-02-01 16:20:21.000000 conllup-0.4.5/long_description.rst
+-rw-rw-r--   0 wran      (1000) wran      (1000)      246 2023-04-14 16:23:44.000000 conllup-0.4.5/pyproject.toml
+-rw-rw-r--   0 wran      (1000) wran      (1000)      482 2023-04-14 16:26:49.305427 conllup-0.4.5/setup.cfg
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-14 16:26:49.305427 conllup-0.4.5/src/
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-14 16:26:49.305427 conllup-0.4.5/src/conllup/
+-rw-rw-r--   0 wran      (1000) wran      (1000)        0 2023-01-30 16:14:25.000000 conllup-0.4.5/src/conllup/__init__.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)    11695 2023-04-14 16:23:44.000000 conllup-0.4.5/src/conllup/conllup.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)     6803 2023-02-07 18:51:16.000000 conllup-0.4.5/src/conllup/processing.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)      552 2023-02-02 18:44:41.000000 conllup-0.4.5/src/conllup/types.py
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-14 16:26:49.305427 conllup-0.4.5/src/conllup.egg-info/
+-rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-04-14 16:26:49.000000 conllup-0.4.5/src/conllup.egg-info/PKG-INFO
+-rw-rw-r--   0 wran      (1000) wran      (1000)      289 2023-04-14 16:26:49.000000 conllup-0.4.5/src/conllup.egg-info/SOURCES.txt
+-rw-rw-r--   0 wran      (1000) wran      (1000)        1 2023-04-14 16:26:49.000000 conllup-0.4.5/src/conllup.egg-info/dependency_links.txt
+-rw-rw-r--   0 wran      (1000) wran      (1000)        8 2023-04-14 16:26:49.000000 conllup-0.4.5/src/conllup.egg-info/top_level.txt
```

### Comparing `conllup-0.4.4/README.md` & `conllup-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 ```
 
 ## Deploy new release
 
 Require to have `pip install twine setuptools build` before doing any build 0) check all tests are passing `python3 -m pytest`
 
-1. change versions
+1. change versions in pyproject.toml
 2. build new package `python3 -m build`
 3. upload to pypi `python3 -m twine upload --repository pypi dist/*`
 4. Optional : if you want to try the testpypi version of the package `pip install --index-url https://test.pypi.org/simple/ --no-deps conllup`
 
 ## Changelog
 ### 0.4.4:
 - minor fix
```

### Comparing `conllup-0.4.4/src/conllup/conllup.py` & `conllup-0.4.5/src/conllup/conllup.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,14 +67,17 @@
 
     for featureKeyValue in splittedFeaturesStrings:
         splittedFeature = featureKeyValue.split("=")
         featureKey = splittedFeature[0]
         featureValue = "=".join(
             splittedFeature[1:]
         )  # reconstructing for this case : 'person=first=second'
+        if featuresJson.get(featureKey):
+            # we add all duplicated keys in this list, as it's forbidden in conll format
+            raise Exception(f"DUPLICATED KEY : found (among others) the duplicated `{featureKey}` key")
         featuresJson[featureKey] = featureValue
 
     return featuresJson
 
 
 def _featuresJsonToConll(featuresJson: featuresJson_T) -> str:
     splittedFeatureConll: List[str] = []
@@ -111,18 +114,17 @@
         return int(data, 10)
 
 def _tokenConllToJson(nodeConll: str) -> tokenJson_T:
     trimmedNodeConll = nodeConll.rstrip().strip()
     splittedNodeConll = trimmedNodeConll.split("\t")
     if len(splittedNodeConll) != 10:
         raise Exception(
-            f'CONLL PARSING ERROR : line "{nodeConll}" is not valid, {len(splittedNodeConll)} columns found instead of 10'
+            f'COLUMNS NUMBER ERROR : {len(splittedNodeConll)} columns found instead of 10  --- line content = "{nodeConll}"'
         )
 
-    head_str = splittedNodeConll[6]
     tokenJson = {
         "ID": splittedNodeConll[0],
         "FORM": splittedNodeConll[1],
         "LEMMA": splittedNodeConll[2],
         "UPOS": splittedNodeConll[3],
         "XPOS": splittedNodeConll[4],
         "FEATS": _featuresConllToJson(splittedNodeConll[5]),
@@ -282,44 +284,67 @@
 
 def sentenceJsonToConll(sentenceJson: sentenceJson_T) -> str:
     metaConll = _metaJsonToConll(sentenceJson["metaJson"])
     treeConll = _treeJsonToConll(sentenceJson["treeJson"])
     return "\n".join([metaConll, treeConll]).strip() + "\n"
 
 
+
+
+class EmptyConllError(Exception):
+    pass
+
+class ConllParseError(Exception):
+    pass
+
+def findConllFormatErrors(conllText):
+    errorsMessages = []
+    for idxLine, line in enumerate(conllText.rstrip().split("\n"), start=1):
+        errorSuffix = f"Line {idxLine} : "
+        if line.strip().rstrip():
+            if line[0] != "#":
+                try:
+                    _tokenConllToJson(line)
+                except Exception as e:
+                    errorsMessages.append(errorSuffix + str(e))
+    return errorsMessages
+
+
 def readConlluFile(filePath: str, keepEmptyTrees = False):
     if not os.path.isfile(filePath):
-        raise Exception(f"No file found  `{filePath}`")
+        raise FileNotFoundError(f"No file found `{filePath}`")
+
+    if os.path.getsize(filePath) == 0:
+        raise EmptyConllError(f"You provided an empty conllu `{filePath}`")
+
     sentencesJson: List[sentenceJson_T] = []
     with open(filePath, "r", encoding="utf-8") as infile:
-        for potentialSentenceConll in infile.read().split("\n\n"):
+        conllContent = infile.read().rstrip()
+
+    try:
+        for potentialSentenceConll in conllContent.split("\n\n"):
             if potentialSentenceConll.strip():
                 sentenceJson = sentenceConllToJson(potentialSentenceConll)
-                if keepEmptyTrees == True or len(sentenceJson["treeJson"]["nodesJson"].values()):
+                if keepEmptyTrees or len(sentenceJson["treeJson"]["nodesJson"].values()):
                     sentencesJson.append(sentenceConllToJson(potentialSentenceConll))
-    return sentencesJson
 
+    except Exception as e:
+        errors = findConllFormatErrors(conllContent)
+        if len(errors):
+            # we have detected errors manually
+            errorText = "\n".join(findConllFormatErrors(conllContent))
+        else:
+            # no error was found manually, the error is something else
+            errorText = str(e)
+        fileName = filePath.split("/")[-1]
+        raise ConllParseError(f"Parsing Errors with file `{fileName}` :\n{errorText}")
 
-def readConlluFile(filePath: str, keepEmptyTrees = False):
-    if not os.path.isfile(filePath):
-        raise Exception(f"No file found  `{filePath}`")
-    sentencesJson: List[sentenceJson_T] = []
-    with open(filePath, "r", encoding="utf-8") as infile:
-        currentConll = ""
-        for line in infile:
-            if line == "\n":
-                if currentConll.strip():
-                    sentenceJson = sentenceConllToJson(currentConll)
-                    if keepEmptyTrees == True or len(sentenceJson["treeJson"]["nodesJson"].values()):
-                        sentencesJson.append(sentenceConllToJson(currentConll))
-                    currentConll = ""
-            else:
-                currentConll += line
     return sentencesJson
 
+
 def _getStringForManySentencesJson(sentencesJson: List[sentenceJson_T]):
     sentencesConll = [sentenceJsonToConll(sentenceJson) for sentenceJson in sentencesJson]
     concatString = "\n".join(sentencesConll) + "\n"
     return concatString
 
 
 def writeConlluFile(filePath: str, sentencesJson: List[sentenceJson_T], overwrite=False):
```

### Comparing `conllup-0.4.4/src/conllup/processing.py` & `conllup-0.4.5/src/conllup/processing.py`

 * *Files identical despite different names*

### Comparing `conllup-0.4.4/src/conllup/types.py` & `conllup-0.4.5/src/conllup/types.py`

 * *Files identical despite different names*

