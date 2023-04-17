# Comparing `tmp/gg_release_notes-1.2.8-py3-none-any.whl.zip` & `tmp/gg_release_notes-1.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 10898 bytes, number of entries: 16
--rw-rw-r--  2.0 unx       21 b- defN 23-Apr-17 12:24 gg_release_notes/__init__.py
--rw-rw-r--  2.0 unx     4516 b- defN 23-Apr-17 11:35 gg_release_notes/generate_release_notes.py
+Zip file size: 10892 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx       21 b- defN 23-Apr-17 12:32 gg_release_notes/__init__.py
+-rw-rw-r--  2.0 unx     4515 b- defN 23-Apr-17 12:30 gg_release_notes/generate_release_notes.py
 -rw-rw-r--  2.0 unx     3815 b- defN 23-Apr-17 12:21 gg_release_notes/pull_request.py
 -rw-rw-r--  2.0 unx     4678 b- defN 23-Apr-17 11:35 gg_release_notes/upload.py
 -rw-rw-r--  2.0 unx     1862 b- defN 23-Apr-17 11:35 gg_release_notes/version.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-17 11:35 gg_release_notes/config/__init__.py
 -rw-rw-r--  2.0 unx      306 b- defN 23-Apr-17 11:35 gg_release_notes/config/env_config.py
 -rw-rw-r--  2.0 unx      549 b- defN 23-Apr-17 11:35 gg_release_notes/config/github_config.py
 -rw-rw-r--  2.0 unx     1444 b- defN 23-Apr-17 11:35 gg_release_notes/config/prompt_config.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-17 11:35 gg_release_notes/utils/__init__.py
 -rw-rw-r--  2.0 unx      422 b- defN 23-Apr-17 11:35 gg_release_notes/utils/encode_bs64.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Apr-17 12:24 gg_release_notes-1.2.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3349 b- defN 23-Apr-17 12:24 gg_release_notes-1.2.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-17 12:24 gg_release_notes-1.2.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       17 b- defN 23-Apr-17 12:24 gg_release_notes-1.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1425 b- defN 23-Apr-17 12:24 gg_release_notes-1.2.8.dist-info/RECORD
-16 files, 23562 bytes uncompressed, 8496 bytes compressed:  63.9%
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Apr-17 12:32 gg_release_notes-1.2.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3349 b- defN 23-Apr-17 12:32 gg_release_notes-1.2.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-17 12:32 gg_release_notes-1.2.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       17 b- defN 23-Apr-17 12:32 gg_release_notes-1.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1425 b- defN 23-Apr-17 12:32 gg_release_notes-1.2.9.dist-info/RECORD
+16 files, 23561 bytes uncompressed, 8490 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: gg_release_notes/utils/__init__.py
 Comment: 
 
 Filename: gg_release_notes/utils/encode_bs64.py
 Comment: 
 
-Filename: gg_release_notes-1.2.8.dist-info/LICENSE
+Filename: gg_release_notes-1.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: gg_release_notes-1.2.8.dist-info/METADATA
+Filename: gg_release_notes-1.2.9.dist-info/METADATA
 Comment: 
 
-Filename: gg_release_notes-1.2.8.dist-info/WHEEL
+Filename: gg_release_notes-1.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: gg_release_notes-1.2.8.dist-info/top_level.txt
+Filename: gg_release_notes-1.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: gg_release_notes-1.2.8.dist-info/RECORD
+Filename: gg_release_notes-1.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gg_release_notes/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '1.2.8'
+__version__ = '1.2.9'
```

## gg_release_notes/generate_release_notes.py

```diff
@@ -75,15 +75,15 @@
 
         Returns:
             Tuple[list, list]: Tuple of List of batches of issues to be used in the prompt for the openai API.
         """
         prompt_issues_descriptions = list(
             set(
                 [
-                    "\n" + f"#{' '.join(issue_num)}" + issue_title
+                    "\n" + f"#{''.join(issue_num)}" + issue_title
                     for issue_title, issue_num in self.prod_release_pr.request_pr_commits()
                 ]
             )
         )
         # Cleanup prompt with using regex and replace
         prompt_issues_descriptions = [
             issue.replace(
```

## Comparing `gg_release_notes-1.2.8.dist-info/LICENSE` & `gg_release_notes-1.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gg_release_notes-1.2.8.dist-info/METADATA` & `gg_release_notes-1.2.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gg-release-notes
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python Interface for generating release notes for Github Actions
 Home-page: https://github.com/DataWiz40/gg-release-notes/
 Author: DataWiz40
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic (==1.8.2)
```

## Comparing `gg_release_notes-1.2.8.dist-info/RECORD` & `gg_release_notes-1.2.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-gg_release_notes/__init__.py,sha256=cjYkehMdBwE5OyVBgmb7f8X0eVOCQfCLgw8D6pdxpfU,21
-gg_release_notes/generate_release_notes.py,sha256=1fat4xp_wqWhjsh_x4LpS-dnKnNUqSuARCGk7LIctUE,4516
+gg_release_notes/__init__.py,sha256=S2h29KjM2QfA587KjqKjzd2pK0GLkBmHIq8WDOutUiI,21
+gg_release_notes/generate_release_notes.py,sha256=j3sbXGyv_cpHhnKnTaoQhyEmhCcv3KTUbFWrLMnfsaM,4515
 gg_release_notes/pull_request.py,sha256=aTSIp8mEzi31nKIlD7x2kbUITAHrkBr6CX8YRWbzYO4,3815
 gg_release_notes/upload.py,sha256=2SiJhyhuUHt12-Bc-lNfSwgo8YnWvJV0HvUgPZ7EqI4,4678
 gg_release_notes/version.py,sha256=edHUBMgGvQ7yedBElOshZV5oCEoIai-1SxhHyV5RsUs,1862
 gg_release_notes/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gg_release_notes/config/env_config.py,sha256=fePLMYGqjG1zcL1c_uzDmdIChHH-aYGlmY5sUoZgcxk,306
 gg_release_notes/config/github_config.py,sha256=pNTQWfzIRZcNyUMf8V02U2KhX5wWw_FNSiDlrVAUsM0,549
 gg_release_notes/config/prompt_config.py,sha256=UR66jazUGEJ2mRm6QU1I-dFG-VEgcoccNpFS2z6oh3M,1444
 gg_release_notes/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gg_release_notes/utils/encode_bs64.py,sha256=49q_T5rgI2521-8Uu28x3z32mNjOmR81_4_XpUBSZGM,422
-gg_release_notes-1.2.8.dist-info/LICENSE,sha256=6s7lZbjUjntzF7mVanm7J7p82tlWO3NDTDHXatSRzUw,1066
-gg_release_notes-1.2.8.dist-info/METADATA,sha256=XjvQ8s4sqPPgt12qj6k4fS4WaMffjX23rcsb_KEx__0,3349
-gg_release_notes-1.2.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gg_release_notes-1.2.8.dist-info/top_level.txt,sha256=jI5G2K6bO9NtofvF82VK40eI2hZKs0sjBSLMSJiMjsw,17
-gg_release_notes-1.2.8.dist-info/RECORD,,
+gg_release_notes-1.2.9.dist-info/LICENSE,sha256=6s7lZbjUjntzF7mVanm7J7p82tlWO3NDTDHXatSRzUw,1066
+gg_release_notes-1.2.9.dist-info/METADATA,sha256=NUbnDUUh-vIJOPfg2FqvrZBpw2BVnfNUv-u5DOsLM0o,3349
+gg_release_notes-1.2.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gg_release_notes-1.2.9.dist-info/top_level.txt,sha256=jI5G2K6bO9NtofvF82VK40eI2hZKs0sjBSLMSJiMjsw,17
+gg_release_notes-1.2.9.dist-info/RECORD,,
```

