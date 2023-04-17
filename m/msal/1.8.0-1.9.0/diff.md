# Comparing `tmp/msal-1.8.0.tar.gz` & `tmp/msal-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/msal-1.8.0.tar", last modified: Wed Dec 16 04:52:45 2020, max compression
+gzip compressed data, was "msal-1.9.0.tar", last modified: Tue Feb  9 07:57:57 2021, max compression
```

## Comparing `msal-1.8.0.tar` & `msal-1.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 04:52:45.000000 msal-1.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10757 2020-12-16 04:52:45.000000 msal-1.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2020-12-16 04:52:23.000000 msal-1.8.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 04:52:45.000000 msal-1.8.0/msal/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6443 2020-12-16 04:52:23.000000 msal-1.8.0/msal/mex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65983 2020-12-16 04:52:23.000000 msal-1.8.0/msal/application.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4417 2020-12-16 04:52:23.000000 msal-1.8.0/msal/wstrust_response.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 04:52:45.000000 msal-1.8.0/msal/oauth2cli/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2516 2020-12-16 04:52:23.000000 msal-1.8.0/msal/oauth2cli/http.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11039 2020-12-16 04:52:23.000000 msal-1.8.0/msal/oauth2cli/oidc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11098 2020-12-16 04:52:23.000000 msal-1.8.0/msal/oauth2cli/authcode.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40544 2020-12-16 04:52:23.000000 msal-1.8.0/msal/oauth2cli/oauth2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4900 2020-12-16 04:52:23.000000 msal-1.8.0/msal/oauth2cli/assertion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2020-12-16 04:52:23.000000 msal-1.8.0/msal/oauth2cli/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1702 2020-12-16 04:52:23.000000 msal-1.8.0/msal/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14049 2020-12-16 04:52:23.000000 msal-1.8.0/msal/token_cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2020-12-16 04:52:23.000000 msal-1.8.0/msal/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7488 2020-12-16 04:52:23.000000 msal-1.8.0/msal/authority.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6027 2020-12-16 04:52:23.000000 msal-1.8.0/msal/wstrust_request.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-16 04:52:45.000000 msal-1.8.0/msal.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10757 2020-12-16 04:52:45.000000 msal-1.8.0/msal.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-12-16 04:52:45.000000 msal-1.8.0/msal.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2020-12-16 04:52:45.000000 msal-1.8.0/msal.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      475 2020-12-16 04:52:45.000000 msal-1.8.0/msal.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-12-16 04:52:45.000000 msal-1.8.0/msal.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      188 2020-12-16 04:52:45.000000 msal-1.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     3847 2020-12-16 04:52:23.000000 msal-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-09 07:57:57.249634 msal-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)    10757 2021-02-09 07:57:57.249634 msal-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     8376 2021-02-09 07:57:47.000000 msal-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-09 07:57:57.249634 msal-1.9.0/msal/
+-rw-r--r--   0 runner    (1001) docker     (116)     1532 2021-02-09 07:57:47.000000 msal-1.9.0/msal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    66739 2021-02-09 07:57:47.000000 msal-1.9.0/msal/application.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7488 2021-02-09 07:57:47.000000 msal-1.9.0/msal/authority.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1702 2021-02-09 07:57:47.000000 msal-1.9.0/msal/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6443 2021-02-09 07:57:47.000000 msal-1.9.0/msal/mex.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-09 07:57:57.249634 msal-1.9.0/msal/oauth2cli/
+-rw-r--r--   0 runner    (1001) docker     (116)      205 2021-02-09 07:57:47.000000 msal-1.9.0/msal/oauth2cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5285 2021-02-09 07:57:47.000000 msal-1.9.0/msal/oauth2cli/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12429 2021-02-09 07:57:47.000000 msal-1.9.0/msal/oauth2cli/authcode.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2516 2021-02-09 07:57:47.000000 msal-1.9.0/msal/oauth2cli/http.py
+-rw-r--r--   0 runner    (1001) docker     (116)    40841 2021-02-09 07:57:47.000000 msal-1.9.0/msal/oauth2cli/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11255 2021-02-09 07:57:47.000000 msal-1.9.0/msal/oauth2cli/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14049 2021-02-09 07:57:47.000000 msal-1.9.0/msal/token_cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6027 2021-02-09 07:57:47.000000 msal-1.9.0/msal/wstrust_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4417 2021-02-09 07:57:47.000000 msal-1.9.0/msal/wstrust_response.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-09 07:57:57.249634 msal-1.9.0/msal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    10757 2021-02-09 07:57:57.000000 msal-1.9.0/msal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      475 2021-02-09 07:57:57.000000 msal-1.9.0/msal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-09 07:57:57.000000 msal-1.9.0/msal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       64 2021-02-09 07:57:57.000000 msal-1.9.0/msal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        5 2021-02-09 07:57:57.000000 msal-1.9.0/msal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      188 2021-02-09 07:57:57.249634 msal-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     3847 2021-02-09 07:57:47.000000 msal-1.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `msal-1.8.0/PKG-INFO` & `msal-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal
-Version: 1.8.0
+Version: 1.9.0
 Summary: The Microsoft Authentication Library (MSAL) for Python library enables your app to access the Microsoft Cloud by supporting authentication of users with Microsoft Azure Active Directory accounts (AAD) and Microsoft Accounts (MSA) using industry standard OAuth2 and OpenID Connect.
 Home-page: https://github.com/AzureAD/microsoft-authentication-library-for-python
 Author: Microsoft Corporation
 Author-email: nugetaad@microsoft.com
 License: MIT
 Project-URL: Changelog, https://github.com/AzureAD/microsoft-authentication-library-for-python/releases
 Description: # Microsoft Authentication Library (MSAL) for Python
```

### Comparing `msal-1.8.0/README.md` & `msal-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `msal-1.8.0/msal/mex.py` & `msal-1.9.0/msal/mex.py`

 * *Files identical despite different names*

### Comparing `msal-1.8.0/msal/application.py` & `msal-1.9.0/msal/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .mex import send_request as mex_send_request
 from .wstrust_request import send_request as wst_send_request
 from .wstrust_response import *
 from .token_cache import TokenCache
 
 
 # The __init__.py will import this. Not the other way around.
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
 logger = logging.getLogger(__name__)
 
 def decorate_scope(
         scopes, client_id,
         reserved_scope=frozenset(['openid', 'profile', 'offline_access'])):
     if not isinstance(scopes, (list, set, tuple)):
@@ -52,15 +52,17 @@
         decorated = scope_set | reserved_scope
     return list(decorated)
 
 CLIENT_REQUEST_ID = 'client-request-id'
 CLIENT_CURRENT_TELEMETRY = 'x-client-current-telemetry'
 
 def _get_new_correlation_id():
-    return str(uuid.uuid4())
+    correlation_id = str(uuid.uuid4())
+    logger.debug("Generates correlation_id: %s", correlation_id)
+    return correlation_id
 
 
 def _build_current_telemetry_request_header(public_api_id, force_refresh=False):
     return "1|{},{}|".format(public_api_id, "1" if force_refresh else "0")
 
 
 def extract_certs(public_cert_content):
@@ -435,24 +437,28 @@
             self.http_client
             ) if authority else self.authority
 
         client = Client(
             {"authorization_endpoint": the_authority.authorization_endpoint},
             self.client_id,
             http_client=self.http_client)
-        return client.build_auth_request_uri(
-            response_type=response_type,
-            redirect_uri=redirect_uri, state=state, login_hint=login_hint,
-            prompt=prompt,
-            scope=decorate_scope(scopes, self.client_id),
-            nonce=nonce,
-            domain_hint=domain_hint,
-            claims=_merge_claims_challenge_and_capabilities(
-                self._client_capabilities, claims_challenge),
-            )
+        warnings.warn(
+            "Change your get_authorization_request_url() "
+            "to initiate_auth_code_flow()", DeprecationWarning)
+        with warnings.catch_warnings(record=True):
+            return client.build_auth_request_uri(
+                response_type=response_type,
+                redirect_uri=redirect_uri, state=state, login_hint=login_hint,
+                prompt=prompt,
+                scope=decorate_scope(scopes, self.client_id),
+                nonce=nonce,
+                domain_hint=domain_hint,
+                claims=_merge_claims_challenge_and_capabilities(
+                    self._client_capabilities, claims_challenge),
+                )
 
     def acquire_token_by_auth_code_flow(
             self, auth_code_flow, auth_response, scopes=None, **kwargs):
         """Validate the auth response being redirected back, and obtain tokens.
 
         It automatically provides nonce protection.
 
@@ -566,28 +572,32 @@
         # If scope is absent on the wire, STS will give you a token associated
         # to the FIRST scope sent during the authorization request.
         # So in theory, you can omit scope here when you were working with only
         # one scope. But, MSAL decorates your scope anyway, so they are never
         # really empty.
         assert isinstance(scopes, list), "Invalid parameter type"
         self._validate_ssh_cert_input_data(kwargs.get("data", {}))
-        return self.client.obtain_token_by_authorization_code(
-            code, redirect_uri=redirect_uri,
-            scope=decorate_scope(scopes, self.client_id),
-            headers={
-                CLIENT_REQUEST_ID: _get_new_correlation_id(),
-                CLIENT_CURRENT_TELEMETRY: _build_current_telemetry_request_header(
-                    self.ACQUIRE_TOKEN_BY_AUTHORIZATION_CODE_ID),
-                },
-            data=dict(
-                kwargs.pop("data", {}),
-                claims=_merge_claims_challenge_and_capabilities(
-                    self._client_capabilities, claims_challenge)),
-            nonce=nonce,
-            **kwargs)
+        warnings.warn(
+            "Change your acquire_token_by_authorization_code() "
+            "to acquire_token_by_auth_code_flow()", DeprecationWarning)
+        with warnings.catch_warnings(record=True):
+            return self.client.obtain_token_by_authorization_code(
+                code, redirect_uri=redirect_uri,
+                scope=decorate_scope(scopes, self.client_id),
+                headers={
+                    CLIENT_REQUEST_ID: _get_new_correlation_id(),
+                    CLIENT_CURRENT_TELEMETRY: _build_current_telemetry_request_header(
+                        self.ACQUIRE_TOKEN_BY_AUTHORIZATION_CODE_ID),
+                    },
+                data=dict(
+                    kwargs.pop("data", {}),
+                    claims=_merge_claims_challenge_and_capabilities(
+                        self._client_capabilities, claims_challenge)),
+                nonce=nonce,
+                **kwargs)
 
     def get_accounts(self, username=None):
         """Get a list of accounts which previously signed in, i.e. exists in cache.
 
         An account can later be used in :func:`~acquire_token_silent`
         to find its tokens.
 
@@ -938,15 +948,15 @@
                     "(https://tools.ietf.org/html/rfc7517).")
             if not data.get("key_id"):
                 raise ValueError(
                     "When requesting an SSH certificate, "
                     "you must include a string parameter named 'key_id' "
                     "which identifies the key in the 'req_cnf' argument.")
 
-    def acquire_token_by_refresh_token(self, refresh_token, scopes):
+    def acquire_token_by_refresh_token(self, refresh_token, scopes, **kwargs):
         """Acquire token(s) based on a refresh token (RT) obtained from elsewhere.
 
         You use this method only when you have old RTs from elsewhere,
         and now you want to migrate them into MSAL.
         Calling this method results in new tokens automatically storing into MSAL.
 
         You do NOT need to use this method if you are already using MSAL.
@@ -961,26 +971,27 @@
             Each scope needs to be in the Microsoft identity platform (v2) format.
             See `Scopes not resources <https://docs.microsoft.com/en-us/azure/active-directory/develop/migrate-python-adal-msal#scopes-not-resources>`_.
 
         :return:
             * A dict contains "error" and some other keys, when error happened.
             * A dict contains no "error" key means migration was successful.
         """
+        self._validate_ssh_cert_input_data(kwargs.get("data", {}))
         return self.client.obtain_token_by_refresh_token(
             refresh_token,
             scope=decorate_scope(scopes, self.client_id),
             headers={
                 CLIENT_REQUEST_ID: _get_new_correlation_id(),
                 CLIENT_CURRENT_TELEMETRY: _build_current_telemetry_request_header(
                     self.ACQUIRE_TOKEN_BY_REFRESH_TOKEN),
             },
             rt_getter=lambda rt: rt,
             on_updating_rt=False,
             on_removing_rt=lambda rt_item: None,  # No OP
-            )
+            **kwargs)
 
 
 class PublicClientApplication(ClientApplication):  # browser app or mobile app
 
     DEVICE_FLOW_CORRELATION_ID = "_correlation_id"
 
     def __init__(self, client_id, client_credential=None, **kwargs):
@@ -1229,14 +1240,15 @@
 
         :return: A dict representing the json response from AAD:
 
             - A successful response would contain "access_token" key,
             - an error response would contain "error" and usually "error_description".
         """
         # TBD: force_refresh behavior
+        self._validate_ssh_cert_input_data(kwargs.get("data", {}))
         return self.client.obtain_token_for_client(
             scope=scopes,  # This grant flow requires no scope decoration
             headers={
                 CLIENT_REQUEST_ID: _get_new_correlation_id(),
                 CLIENT_CURRENT_TELEMETRY: _build_current_telemetry_request_header(
                     self.ACQUIRE_TOKEN_FOR_CLIENT_ID),
                 },
@@ -1290,8 +1302,7 @@
                     self._client_capabilities, claims_challenge)),
             headers={
                 CLIENT_REQUEST_ID: _get_new_correlation_id(),
                 CLIENT_CURRENT_TELEMETRY: _build_current_telemetry_request_header(
                     self.ACQUIRE_TOKEN_ON_BEHALF_OF_ID),
                 },
             **kwargs)
-
```

### Comparing `msal-1.8.0/msal/wstrust_response.py` & `msal-1.9.0/msal/wstrust_response.py`

 * *Files identical despite different names*

### Comparing `msal-1.8.0/msal/oauth2cli/http.py` & `msal-1.9.0/msal/oauth2cli/http.py`

 * *Files identical despite different names*

### Comparing `msal-1.8.0/msal/oauth2cli/oidc.py` & `msal-1.9.0/msal/oauth2cli/oidc.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,37 +43,41 @@
     decoded = json.loads(decode_part(id_token.split('.')[1]))
     err = None  # https://openid.net/specs/openid-connect-core-1_0.html#IDTokenValidation
     _now = now or time.time()
     skew = 120  # 2 minutes
     if _now + skew < decoded.get("nbf", _now - 1):  # nbf is optional per JWT specs
         # This is not an ID token validation, but a JWT validation
         # https://tools.ietf.org/html/rfc7519#section-4.1.5
-        err = "0. The ID token is not yet valid"
+        err = "0. The ID token is not yet valid."
     if issuer and issuer != decoded["iss"]:
         # https://openid.net/specs/openid-connect-discovery-1_0.html#ProviderConfigurationResponse
         err = ('2. The Issuer Identifier for the OpenID Provider, "%s", '
             "(which is typically obtained during Discovery), "
             "MUST exactly match the value of the iss (issuer) Claim.") % issuer
     if client_id:
         valid_aud = client_id in decoded["aud"] if isinstance(
             decoded["aud"], list) else client_id == decoded["aud"]
         if not valid_aud:
-            err = "3. The aud (audience) Claim must contain this client's client_id."
+            err = (
+                "3. The aud (audience) claim must contain this client's client_id "
+                '"%s", case-sensitively. Was your client_id in wrong casing?'
+                # Some IdP accepts wrong casing request but issues right casing IDT
+                ) % client_id
     # Per specs:
     # 6. If the ID Token is received via direct communication between
     # the Client and the Token Endpoint (which it is during _obtain_token()),
     # the TLS server validation MAY be used to validate the issuer
     # in place of checking the token signature.
     if _now > decoded["exp"]:
         err = "9. The current time MUST be before the time represented by the exp Claim."
     if nonce and nonce != decoded.get("nonce"):
         err = ("11. Nonce must be the same value "
-            "as the one that was sent in the Authentication Request")
+            "as the one that was sent in the Authentication Request.")
     if err:
-        raise RuntimeError("%s id_token was: %s" % (
+        raise RuntimeError("%s The id_token was: %s" % (
             err, json.dumps(decoded, indent=2)))
     return decoded
 
 
 def _nonce_hash(nonce):
     # https://openid.net/specs/openid-connect-core-1_0.html#NonceNotes
     return hashlib.sha256(nonce.encode("ascii")).hexdigest()
```

### Comparing `msal-1.8.0/msal/oauth2cli/authcode.py` & `msal-1.9.0/msal/oauth2cli/authcode.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,27 +29,17 @@
                 Open this link to <a href='$auth_uri'>Sign In</a>
                 (You may want to use incognito window)
                 <hr><a href='$abort_uri'>Abort</a>
                 </body></html>""",
             ).get("code")
 
 
-def _browse(auth_uri):
+def _browse(auth_uri):  # throws ImportError, possibly webbrowser.Error in future
     import webbrowser  # Lazy import. Some distro may not have this.
-    controller = webbrowser.get()  # Get a default controller
-    # Some Linux Distro does not setup default browser properly,
-    # so we try to explicitly use some popular browser, if we found any.
-    for browser in ["chrome", "firefox", "safari", "windows-default"]:
-        try:
-            controller = webbrowser.get(browser)
-            break
-        except webbrowser.Error:
-            pass  # This browser is not installed. Try next one.
-    logger.info("Please open a browser on THIS device to visit: %s" % auth_uri)
-    controller.open(auth_uri)
+    return webbrowser.open(auth_uri)  # Use default browser. Customizable by $BROWSER
 
 
 def _qs2kv(qs):
     """Flatten parse_qs()'s single-item lists into the item itself"""
     return {k: v[0] if isinstance(v, list) and len(v) == 1 else v
         for k, v in qs.items()}
 
@@ -126,50 +116,79 @@
 
     def get_port(self):
         """The port this server actually listening to"""
         # https://docs.python.org/2.7/library/socketserver.html#SocketServer.BaseServer.server_address
         return self._server.server_address[1]
 
     def get_auth_response(self, auth_uri=None, timeout=None, state=None,
-            welcome_template=None, success_template=None, error_template=None):
-        """Wait and return the auth response, or None when timeout.
+            welcome_template=None, success_template=None, error_template=None,
+            auth_uri_callback=None,
+            ):
+        """Wait and return the auth response. Raise RuntimeError when timeout.
 
         :param str auth_uri:
             If provided, this function will try to open a local browser.
         :param int timeout: In seconds. None means wait indefinitely.
         :param str state:
-            You may provide the state you used in auth_url,
+            You may provide the state you used in auth_uri,
             then we will use it to validate incoming response.
         :param str welcome_template:
             If provided, your end user will see it instead of the auth_uri.
             When present, it shall be a plaintext or html template following
             `Python Template string syntax <https://docs.python.org/3/library/string.html#template-strings>`_,
             and include some of these placeholders: $auth_uri and $abort_uri.
         :param str success_template:
             The page will be displayed when authentication was largely successful.
             Placeholders can be any of these:
             https://tools.ietf.org/html/rfc6749#section-5.1
         :param str error_template:
             The page will be displayed when authentication encountered error.
             Placeholders can be any of these:
             https://tools.ietf.org/html/rfc6749#section-5.2
+        :param callable auth_uri_callback:
+            A function with the shape of lambda auth_uri: ...
+            When a browser was unable to be launch, this function will be called,
+            so that the app could tell user to manually visit the auth_uri.
         :return:
             The auth response of the first leg of Auth Code flow,
             typically {"code": "...", "state": "..."} or {"error": "...", ...}
             See https://tools.ietf.org/html/rfc6749#section-4.1.2
             and https://openid.net/specs/openid-connect-core-1_0.html#AuthResponse
             Returns None when the state was mismatched, or when timeout occurred.
         """
         welcome_uri = "http://localhost:{p}".format(p=self.get_port())
         abort_uri = "{loc}?error=abort".format(loc=welcome_uri)
         logger.debug("Abort by visit %s", abort_uri)
         self._server.welcome_page = Template(welcome_template or "").safe_substitute(
             auth_uri=auth_uri, abort_uri=abort_uri)
-        if auth_uri:
-            _browse(welcome_uri if welcome_template else auth_uri)
+        if auth_uri:  # Now attempt to open a local browser to visit it
+            _uri = welcome_uri if welcome_template else auth_uri
+            logger.info("Open a browser on this device to visit: %s" % _uri)
+            browser_opened = False
+            try:
+                browser_opened = _browse(_uri)
+            except:  # Had to use broad except, because the potential
+                     # webbrowser.Error is purposely undefined outside of _browse().
+                # Absorb and proceed. Because browser could be manually run elsewhere.
+                logger.exception("_browse(...) unsuccessful")
+            if not browser_opened:
+                if not auth_uri_callback:
+                    logger.warning(
+                        "Found no browser in current environment. "
+                        "If this program is being run inside a container "
+                        "which has access to host network "
+                        "(i.e. started by `docker run --net=host -it ...`), "
+                        "you can use browser on host to visit the following link. "
+                        "Otherwise, this auth attempt would either timeout "
+                        "(current timeout setting is {timeout}) "
+                        "or be aborted by CTRL+C. Auth URI: {auth_uri}".format(
+                            auth_uri=_uri, timeout=timeout))
+                else:  # Then it is the auth_uri_callback()'s job to inform the user
+                    auth_uri_callback(_uri)
+
         self._server.success_template = Template(success_template or
             "Authentication completed. You can close this window now.")
         self._server.error_template = Template(error_template or
             "Authentication failed. $error: $error_description. ($error_uri)")
 
         self._server.timeout = timeout  # Otherwise its handle_timeout() won't work
         self._server.auth_response = {}  # Shared with _AuthCodeHandler
```

### Comparing `msal-1.8.0/msal/oauth2cli/oauth2.py` & `msal-1.9.0/msal/oauth2cli/oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,16 @@
                     s.request = functools.partial(s.request, timeout=3)
 
                 and then feed that patched session instance to this class.
 
             client_secret (str):  Triggers HTTP AUTH for Confidential Client
             client_assertion (bytes, callable):
                 The client assertion to authenticate this client, per RFC 7521.
-                It can be a raw SAML2 assertion (this method will encode it for you),
-                or a raw JWT assertion.
+                It can be a raw SAML2 assertion (we will base64 encode it for you),
+                or a raw JWT assertion in bytes (which we will relay to http layer).
                 It can also be a callable (recommended),
                 so that we will do lazy creation of an assertion.
             client_assertion_type (str):
                 The type of your :attr:`client_assertion` parameter.
                 It is typically the value of :attr:`CLIENT_ASSERTION_TYPE_SAML2` or
                 :attr:`CLIENT_ASSERTION_TYPE_JWT`, the only two defined in RFC 7521.
             default_headers (dict):
@@ -194,15 +194,17 @@
 
         if self.default_body.get("client_assertion_type") and self.client_assertion:
             # See https://tools.ietf.org/html/rfc7521#section-4.2
             encoder = self.client_assertion_encoders.get(
                     self.default_body["client_assertion_type"], lambda a: a)
             _data["client_assertion"] = encoder(
                 self.client_assertion()  # Do lazy on-the-fly computation
-                if callable(self.client_assertion) else self.client_assertion)
+                if callable(self.client_assertion) else self.client_assertion
+                )   # The type is bytes, which is preferrable. See also:
+                    # https://github.com/psf/requests/issues/4503#issuecomment-455001070
 
         _data.update(self.default_body)  # It may contain authen parameters
         _data.update(data or {})  # So the content in data param prevails
         _data = {k: v for k, v in _data.items() if v}  # Clean up None values
 
         if _data.get('scope'):
             _data['scope'] = self._stringify(_data['scope'])
@@ -574,14 +576,15 @@
             scope=None,
             extra_scope_to_consent=None,
             redirect_uri=None,
             timeout=None,
             welcome_template=None,
             success_template=None,
             auth_params=None,
+            auth_uri_callback=None,
             **kwargs):
         """A native app can use this method to obtain token via a local browser.
 
         Internally, it implements PKCE to mitigate the auth code interception attack.
 
         :param scope: A list of scopes that you would like to obtain token for.
         :type scope: collections.Iterable[str]
@@ -631,14 +634,15 @@
                     **(auth_params or {}))
                 auth_response = receiver.get_auth_response(
                     auth_uri=flow["auth_uri"],
                     state=flow["state"],  # Optional but we choose to do it upfront
                     timeout=timeout,
                     welcome_template=welcome_template,
                     success_template=success_template,
+                    auth_uri_callback=auth_uri_callback,
                     )
         except PermissionError:
             if 0 < listen_port < 1024:
                 self.logger.error(
                     "Can't listen on port %s. You may try port 0." % listen_port)
             raise
         return self.obtain_token_by_auth_code_flow(
```

### Comparing `msal-1.8.0/msal/oauth2cli/assertion.py` & `msal-1.9.0/msal/oauth2cli/assertion.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 import logging
 
 import jwt
 
 
 logger = logging.getLogger(__name__)
 
+
+def _str2bytes(raw):
+    # A conversion based on duck-typing rather than six.text_type
+    try:  # Assuming it is a string
+        return raw.encode(encoding="utf-8")
+    except:  # Otherwise we treat it as bytes and return it as-is
+        return raw
+
+
 class AssertionCreator(object):
     def create_normal_assertion(
             self, audience, issuer, subject, expires_at=None, expires_in=600,
             issued_at=None, assertion_id=None, **kwargs):
         """Create an assertion in bytes, based on the provided claims.
 
         All parameter names are defined in https://tools.ietf.org/html/rfc7521#section-5
@@ -99,16 +108,17 @@
             'iat': issued_at or now,
             'jti': assertion_id or str(uuid.uuid4()),
             }
         if not_before:
             payload['nbf'] = not_before
         payload.update(additional_claims or {})
         try:
-            return jwt.encode(
+            str_or_bytes = jwt.encode(  # PyJWT 1 returns bytes, PyJWT 2 returns str
                 payload, self.key, algorithm=self.algorithm, headers=self.headers)
+            return _str2bytes(str_or_bytes)  # We normalize them into bytes
         except:
             if self.algorithm.startswith("RS") or self.algorithm.starswith("ES"):
                 logger.exception(
                     'Some algorithms requires "pip install cryptography". '
                     'See https://pyjwt.readthedocs.io/en/latest/installation.html#cryptographic-dependencies-optional')
             raise
```

### Comparing `msal-1.8.0/msal/exceptions.py` & `msal-1.9.0/msal/exceptions.py`

 * *Files identical despite different names*

### Comparing `msal-1.8.0/msal/token_cache.py` & `msal-1.9.0/msal/token_cache.py`

 * *Files identical despite different names*

### Comparing `msal-1.8.0/msal/__init__.py` & `msal-1.9.0/msal/__init__.py`

 * *Files identical despite different names*

### Comparing `msal-1.8.0/msal/authority.py` & `msal-1.9.0/msal/authority.py`

 * *Files identical despite different names*

### Comparing `msal-1.8.0/msal/wstrust_request.py` & `msal-1.9.0/msal/wstrust_request.py`

 * *Files identical despite different names*

### Comparing `msal-1.8.0/msal.egg-info/PKG-INFO` & `msal-1.9.0/msal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal
-Version: 1.8.0
+Version: 1.9.0
 Summary: The Microsoft Authentication Library (MSAL) for Python library enables your app to access the Microsoft Cloud by supporting authentication of users with Microsoft Azure Active Directory accounts (AAD) and Microsoft Accounts (MSA) using industry standard OAuth2 and OpenID Connect.
 Home-page: https://github.com/AzureAD/microsoft-authentication-library-for-python
 Author: Microsoft Corporation
 Author-email: nugetaad@microsoft.com
 License: MIT
 Project-URL: Changelog, https://github.com/AzureAD/microsoft-authentication-library-for-python/releases
 Description: # Microsoft Authentication Library (MSAL) for Python
```

### Comparing `msal-1.8.0/setup.py` & `msal-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     packages=find_packages(exclude=["tests"]),
     package_data={'': ['LICENSE']},  # Do not use data_files=[...],
         # which would cause the LICENSE being copied to /usr/local,
         # and tend to fail because of insufficient permission.
         # See https://stackoverflow.com/a/14211600/728675 for more detail
     install_requires=[
         'requests>=2.0.0,<3',
-        'PyJWT[crypto]>=1.0.0,<2',
+        'PyJWT[crypto]>=1.0.0,<3',
 
         'cryptography>=0.6,<4',
             # load_pem_private_key() is available since 0.6
             # https://github.com/pyca/cryptography/blob/master/CHANGELOG.rst#06---2014-09-29
             #
             # Not sure what should be used as an upper bound here
             # https://github.com/pyca/cryptography/issues/5532
```

