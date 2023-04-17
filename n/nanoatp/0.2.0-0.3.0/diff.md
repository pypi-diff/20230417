# Comparing `tmp/nanoatp-0.2.0.tar.gz` & `tmp/nanoatp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoatp-0.2.0.tar", max compression
+gzip compressed data, was "nanoatp-0.3.0.tar", max compression
```

## Comparing `nanoatp-0.2.0.tar` & `nanoatp-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.2.0/LICENSE
--rw-r--r--   0        0        0     2482 2023-04-16 10:06:15.513807 nanoatp-0.2.0/README.md
--rw-r--r--   0        0        0      234 2023-04-16 10:06:15.517638 nanoatp-0.2.0/nanoatp/__init__.py
--rw-r--r--   0        0        0     7820 2023-04-16 10:06:15.518718 nanoatp-0.2.0/nanoatp/nanoatp.py
--rw-r--r--   0        0        0      486 2023-04-16 09:51:16.540716 nanoatp-0.2.0/nanoatp/richtext.py
--rw-r--r--   0        0        0      581 2023-04-16 10:06:15.519574 nanoatp-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3293 1970-01-01 00:00:00.000000 nanoatp-0.2.0/setup.py
--rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 nanoatp-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2522 2023-04-16 15:21:42.771721 nanoatp-0.3.0/README.md
+-rw-r--r--   0        0        0      277 2023-04-16 15:21:42.772635 nanoatp-0.3.0/nanoatp/__init__.py
+-rw-r--r--   0        0        0     8200 2023-04-16 15:21:42.773568 nanoatp-0.3.0/nanoatp/nanoatp.py
+-rw-r--r--   0        0        0     3034 2023-04-16 15:21:42.774112 nanoatp-0.3.0/nanoatp/richtext.py
+-rw-r--r--   0        0        0      595 2023-04-16 15:39:30.836238 nanoatp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 nanoatp-0.3.0/PKG-INFO
```

### Comparing `nanoatp-0.2.0/LICENSE` & `nanoatp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoatp-0.2.0/README.md` & `nanoatp-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 # Feeds and content
 agent.getPost(repo, rkey, cid)
 agent.post(record)
 agent.deletePost(postUri)
 agent.uploadBlob(data, encoding)
 agent.uploadImage(path, alt, encoding)  # wrapper for uploadBlob
 
+# Identity
+agent.resolveHandle(handle)
+
 # Session management
 agent.login(identifier, password)
 ```
 
 For example, to post a record, reply to it, and upload an image:
 
 ```python
```

### Comparing `nanoatp-0.2.0/nanoatp/nanoatp.py` & `nanoatp-0.3.0/nanoatp/nanoatp.py`

 * *Files 6% similar despite different names*

```diff
@@ -154,14 +154,22 @@
     def uploadBlob(self, data: bytes, encoding: str) -> dict[str, Any]:
         """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/repo/uploadBlob.json"""
         headers = {"Content-Type": encoding, "Content-Length": str(len(data))}
         headers.update(self.headers)
         response = self.requests.post(f"{self.service}/xrpc/com.atproto.repo.uploadBlob", headers=headers, data=data)
         return response.json()
 
+    def resolveHandle(self, handle: str):
+        """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/identity/resolveHandle.json"""
+        params = {"handle": handle}
+        response = self.requests.get(
+            f"{self.service}/xrpc/com.atproto.identity.resolveHandle", headers=self.headers, params=params
+        )
+        return response.json()
+
 
 # TODO: create util.py?
 def verifySession(session: dict[str, str]):
     """https://github.com/bluesky-social/atproto/blob/main/lexicons/com/atproto/server/createSession.json"""
     # email is optional
     return not session.get("error") and set(session.keys()).issuperset({"did", "handle", "accessJwt", "refreshJwt"})
```

### Comparing `nanoatp-0.2.0/pyproject.toml` & `nanoatp-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "nanoatp"
-version = "0.2.0"
+version = "0.3.0"
 description = "nano implementation of the AT Protocol (Authenticated Transfer Protocol)"
 authors = ["Susumu OTA <1632335+susumuota@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.16"
 requests = "^2.28.2"
+tld = "^0.13"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 black = "^23.3.0"
 pytest = "^7.3.0"
```

### Comparing `nanoatp-0.2.0/PKG-INFO` & `nanoatp-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nanoatp
-Version: 0.2.0
+Version: 0.3.0
 Summary: nano implementation of the AT Protocol (Authenticated Transfer Protocol)
 Author: Susumu OTA
 Author-email: 1632335+susumuota@users.noreply.github.com
 Requires-Python: >=3.9.16,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: tld (>=0.13,<0.14)
 Description-Content-Type: text/markdown
 
 # nanoatp
 
 A nano implementation of the AT Protocol (Authenticated Transfer Protocol).
 
 ## Getting started
@@ -56,14 +57,17 @@
 # Feeds and content
 agent.getPost(repo, rkey, cid)
 agent.post(record)
 agent.deletePost(postUri)
 agent.uploadBlob(data, encoding)
 agent.uploadImage(path, alt, encoding)  # wrapper for uploadBlob
 
+# Identity
+agent.resolveHandle(handle)
+
 # Session management
 agent.login(identifier, password)
 ```
 
 For example, to post a record, reply to it, and upload an image:
 
 ```python
```

