# Comparing `tmp/keeper-secrets-manager-core-16.5.2.tar.gz` & `tmp/keeper-secrets-manager-core-16.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keeper-secrets-manager-core-16.5.2.tar", last modified: Tue Mar 28 17:46:00 2023, max compression
+gzip compressed data, was "keeper-secrets-manager-core-16.5.3.tar", last modified: Mon Apr 17 20:28:16 2023, max compression
```

## Comparing `keeper-secrets-manager-core-16.5.2.tar` & `keeper-secrets-manager-core-16.5.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:46:00.005690 keeper-secrets-manager-core-16.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-03-28 17:46:00.005690 keeper-secrets-manager-core-16.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:46:00.001690 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/configkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)    67982 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:46:00.005690 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/dto/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/dto/dtos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/dto/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/keeper_globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:46:00.001690 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-03-28 17:45:59.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-28 17:45:59.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 17:45:59.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 17:45:59.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-28 17:45:59.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-28 17:45:59.000000 keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-28 17:46:00.005690 keeper-secrets-manager-core-16.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-28 17:45:45.000000 keeper-secrets-manager-core-16.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:28:16.970933 keeper-secrets-manager-core-16.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-17 20:28:16.970933 keeper-secrets-manager-core-16.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:28:16.966933 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/configkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67982 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:28:16.966933 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/keeper_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:28:16.966933 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 20:28:16.000000 keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 20:28:16.970933 keeper-secrets-manager-core-16.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-17 20:28:01.000000 keeper-secrets-manager-core-16.5.3/setup.py
```

### Comparing `keeper-secrets-manager-core-16.5.2/PKG-INFO` & `keeper-secrets-manager-core-16.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-core
-Version: 16.5.2
+Version: 16.5.3
 Summary: Keeper Secrets Manager for Python 3
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://github.com/Keeper-Security/secrets-manager
@@ -27,14 +27,17 @@
 
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.5.3
+* KSM-393 - Fix file permissions on localized Windows OS
+
 ## 16.5.2
 * KSM-375 - Make HTTPError to be more informative
 * KSM-376 - Support for PAM record types
 * KSM-381 - Transactions
 * Fixed [Issue 441](https://github.com/Keeper-Security/secrets-manager/issues/441) - Bug caused by space in username
 
 ## 16.5.1
```

### Comparing `keeper-secrets-manager-core-16.5.2/README.md` & `keeper-secrets-manager-core-16.5.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.5.3
+* KSM-393 - Fix file permissions on localized Windows OS
+
 ## 16.5.2
 * KSM-375 - Make HTTPError to be more informative
 * KSM-376 - Support for PAM record types
 * KSM-381 - Transactions
 * Fixed [Issue 441](https://github.com/Keeper-Security/secrets-manager/issues/441) - Bug caused by space in username
 
 ## 16.5.1
```

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/configkeys.py` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/configkeys.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/core.py` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/core.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/crypto.py` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/crypto.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/dto/dtos.py` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/dtos.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/dto/payload.py` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/dto/payload.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/exceptions.py` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/helpers.py` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/helpers.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/keeper_globals.py` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/keeper_globals.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/mock.py` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/mock.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/storage.py` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/storage.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core/utils.py` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from urllib import parse
 import subprocess
 import stat
 from distutils.util import strtobool
 
 from keeper_secrets_manager_core.keeper_globals import logger_name
 
-ALLOWED_WINDOWS_CONFIG_ADMINS = ['Administrators', 'SYSTEM']
+ALLOWED_WINDOWS_CONFIG_ADMINS = [b'Administrators', b'SYSTEM']
 ENCODING = 'UTF-8'
 SPECIAL_CHARACTERS = '''"!@#$%()+;<>=?[]{}^.,'''
 DEFAULT_PASSWORD_LENGTH = 32
 
 
 def get_os():
     if _platform.lower().startswith("linux"):
@@ -201,153 +201,244 @@
             sample += sample_string[pos]
 
     return sample
 
 
 def get_windows_user_sid_and_name(logger=None):
     try:
-        user_sid = subprocess.check_output(['whoami', '/user'], encoding='utf-8').splitlines()[-1]
+        user_sid = subprocess.check_output(['whoami', '/user']).splitlines()[-1]
     except subprocess.CalledProcessError as e:
         logger.info(f'Cannot get current Windows user via "whoami": {e}')
         return None, None
     else:
-        return reversed(user_sid.split('\\')[-1].rsplit(' ', 1))
+        return reversed(user_sid.split(b'\\')[-1].rsplit(b' ', 1))
 
 
 def set_config_mode(file, logger=None):
 
-    # Allow the user skip locking down the configuration file's mode.
-    if bool(strtobool(os.environ.get("KSM_CONFIG_SKIP_MODE", "FALSE"))) is False:
-        # For Windows, use icacls. cacls is obsolete.
-
-        if _platform.lower().startswith("win") is True:
-
-            sid, user = get_windows_user_sid_and_name()
-
-            # https://stackoverflow.com/questions/5264595/windows-chmod-600
-            # https://github.com/PowerShell/Win32-OpenSSH/issues/132
-
-            # Remove mode inherited by the directory.
-            # Remove everyone's access
-            # Grant the current user full access
-            # Allow Administrators full access
-            commands = [
-                'icacls.exe "{}" /reset'.format(file),
-                'icacls.exe "{}" /inheritance:r'.format(file),
-                'icacls.exe "{}" /remove:g Everyone:F'.format(file),
-                'icacls.exe "{}" /grant:r Administrators:F'.format(file),
-                'icacls.exe "{}" /grant:r *{}:F'.format(file, sid),
-            ]
-            for command in commands:
-                if logger is not None:
-                    logger.debug("Set Mode Command " + command)
-                output = subprocess.run(command, capture_output=True)
-                if output.stderr is not None and "Access is denied" in output.stderr.decode():
-                    raise Exception("Access denied to configuration file {}.".format(file))
-                if output.stdout is not None and "Failed processing 0 files" not in output.stdout.decode():
-                    message = "Could not change the ACL for file '{}'. Set the environmental variable " \
-                              "'KSM_CONFIG_SKIP_MODE' to 'TRUE' to skip setting the ACL mode.".format(file)
-                    if output.stderr is not None:
-                        message += ": " + output.stderr.decode()
-                    else:
-                        message += "."
+    try:
+        # Allow the user skip locking down the configuration file's mode.
+        if bool(strtobool(os.environ.get("KSM_CONFIG_SKIP_MODE", "FALSE"))) is False:
+            # For Windows, use icacls. cacls is obsolete.
 
-                    raise Exception(message)
-        else:
-            # In Linux/MacOs get file permissions to 0600.
-            os.chmod(file, stat.S_IREAD | stat.S_IWRITE)
+            if _platform.lower().startswith("win") is True:
+
+                sid, user = get_windows_user_sid_and_name()
+                if isinstance(sid, bytes):
+                    sid = sid.decode()
+
+                # https://stackoverflow.com/questions/5264595/windows-chmod-600
+                # https://github.com/PowerShell/Win32-OpenSSH/issues/132
+
+                # Remove mode inherited by the directory.
+                # Remove everyone's access
+                # Grant the current user full access
+                # Allow Administrators full access
+                commands = [
+                    'icacls.exe "{}" /reset'.format(file),
+                    'icacls.exe "{}" /inheritance:r'.format(file),
+                    'icacls.exe "{}" /remove:g Everyone:F'.format(file),
+                    'icacls.exe "{}" /grant:r Administrators:F'.format(file),
+                    'icacls.exe "{}" /grant:r *{}:F'.format(file, sid),
+                ]
+                for command in commands:
+                    if logger is not None:
+                        logger.debug("Set Mode Command " + command)
+                    output = subprocess.run(command, capture_output=True)
+                    if output.returncode == 2:
+                        raise FileNotFoundError("Cannot find configuration file {}.".format(file))
+                    if output.returncode == 5:
+                        raise PermissionError("Access denied to configuration file {}.".format(file))
+                    if output.returncode == 1332:
+                        if logger is not None:
+                            logger.debug(f"Failed to set some ACL permissions: {command}")
+                        continue
+                        # Probably localized group/user names or non-existent/renamed group/user
+                        # Error 1332: No mapping between account names and security IDs was done.
+                        # Successfully processed 0 files; Failed processing 0 files
+                    if output.returncode != 0:
+                        message = "Could not change the ACL for file '{}'. Set the environmental variable " \
+                                "'KSM_CONFIG_SKIP_MODE' to 'TRUE' to skip setting the ACL mode.".format(file)
+                        if output.stderr:
+                            message += ": " + str(output.stderr).lstrip("b").strip("'")
+                        else:
+                            message += "."
+
+                        raise PermissionError(message)
+            else:
+                # In Linux/MacOs get file permissions to 0600.
+                os.chmod(file, stat.S_IREAD | stat.S_IWRITE)
+    except (FileNotFoundError, PermissionError):
+        raise
+    except Exception as e:
+        if logger is not None:
+            logger.debug("set_config_mode failed: " + str(e))
+
+
+localized_admins = []
+def populate_windows_localized_admin_names_win32api():
+    """ Uses Win32 API to get localized account names for known admin accounts """
+
+    import ctypes
+
+    ERROR_INVALID_PARAMETER = 87
+    ERROR_INSUFFICIENT_BUFFER = 122
+    WinLocalSystemSid = 22  # NT AUTHORITY\SYSTEM
+    # WinLocalServiceSid = 23  # NT AUTHORITY\LOCAL SERVICE
+    WinBuiltinAdministratorsSid = 26  # BUILTIN\Administrators
+
+    advapi32 = ctypes.windll.advapi32
+
+    def get_account_name(sid_type):
+        sid_size = ctypes.c_ulong(256)
+        sid = (ctypes.c_byte * sid_size.value)()
+
+        if not advapi32.CreateWellKnownSid(sid_type, None, sid, ctypes.byref(sid_size)):
+            error = ctypes.GetLastError()
+            if error == ERROR_INVALID_PARAMETER or error == ERROR_INSUFFICIENT_BUFFER:
+                sid = (ctypes.c_byte * sid_size.value)()
+                if not advapi32.CreateWellKnownSid(sid_type, None, sid, ctypes.byref(sid_size)):
+                    raise ctypes.WinError()
+
+        name_size = ctypes.c_ulong(0)
+        domain_size = ctypes.c_ulong(0)
+        sid_name_use = ctypes.c_ulong(0)
+        advapi32.LookupAccountSidW(None, sid, None, ctypes.byref(name_size), None, ctypes.byref(domain_size), ctypes.byref(sid_name_use))
+        error = ctypes.GetLastError()
+        if error and error != ERROR_INSUFFICIENT_BUFFER:
+            raise ctypes.WinError(error)
+
+        name = (ctypes.c_wchar * name_size.value)()
+        domain = (ctypes.c_wchar * domain_size.value)()
+        if not advapi32.LookupAccountSidW(None, sid, name, ctypes.byref(name_size), domain, ctypes.byref(domain_size), ctypes.byref(sid_name_use)):
+            raise ctypes.WinError()
+
+        return domain.value, name.value
+
+    # populate only once - lazy init
+    if not localized_admins:
+        admins = []
+        _, name = get_account_name(WinLocalSystemSid)
+        if name:
+            admins.append(name)  # SYSTEM: S-1-5-18
+        _, name = get_account_name(WinBuiltinAdministratorsSid)
+        if name:
+            admins.append(name)  # Administrators: S-1-5-32-544
+
+        # WMI names are unicode - convert to console's code page
+        if admins:
+            cmd = "echo."
+            for admin in admins:
+                cmd += f" & echo {admin}"
+            locout = subprocess.run(["cmd", "/c", cmd], capture_output=True)
+            if locout.returncode == 0 and locout.stdout:
+                for line in locout.stdout.split(b"\n"):
+                    if line.strip():
+                        localized_admins.append(line.strip())
 
 
 def check_config_mode(file, color_mod=None, logger=None) -> bool:
     """Check for correct permissions on file
 
         Return result of check as boolean
     """
 
-    # If we are skipping setting the mode, skip checking.
-    if bool(strtobool(os.environ.get("KSM_CONFIG_SKIP_MODE", "FALSE"))) is True:
-        retval = True
-    else:
-        # For Windows, use icacls. cacls is obsolete.
-        if _platform.lower().startswith("win") is True:
+    retval = False
+    try:
+        # If we are skipping setting the mode, skip checking.
+        if bool(strtobool(os.environ.get("KSM_CONFIG_SKIP_MODE", "FALSE"))) is True:
+            retval = True
+        else:
+            # For Windows, use icacls. cacls is obsolete.
+            if _platform.lower().startswith("win") is True:
 
-            # If this doesn't error out, then we know the file exists
-            output = subprocess.run(["icacls.exe", file], capture_output=True)
-            if output.stderr is not None:
-                if "Access is denied" in output.stderr.decode():
-                    raise PermissionError("Access denied to configuration file {}.".format(file))
-                if "cannot find" in output.stderr.decode():
-                    raise FileNotFoundError("Cannot find configuration file {}.".format(file))
+                # If this doesn't error out, then we know the file exists
+                output = subprocess.run(["icacls.exe", file], capture_output=True)
 
-            # Try to access the file. If it now can't be found, it's a permission problem.
-            try:
-                with open(file, "r") as fh:
-                    fh.close()
-            except (FileNotFoundError, PermissionError):
-                raise PermissionError("Access denied to configuration file {}.".format(file))
+                # check the returncode only - error messages could be in any language
+                if output.returncode > 0:
+                    if output.returncode == 2:
+                        raise FileNotFoundError("Cannot find configuration file {}.".format(file))
+                    if output.returncode == 5:
+                        raise PermissionError("Access denied to configuration file {}.".format(file))
+                    raise PermissionError("Error accessing configuration file {}.".format(file))
 
-            if bool(strtobool(os.environ.get("KSM_CONFIG_SKIP_MODE_WARNING", "FALSE"))) is True:
-                retval = True
-            else:
-                # We need to figure out who we are. subprocess run will use cmd
-                sid, user = get_windows_user_sid_and_name()
-                if sid is None:
-                    # Don't fail check when user SID is missing.
+                # Try to access the file. If it now can't be found, it's a permission problem.
+                try:
+                    with open(file, "r") as fh:
+                        fh.close()
+                except (FileNotFoundError, PermissionError):
+                    raise PermissionError("Access denied to configuration file {}.".format(file))
+
+                if bool(strtobool(os.environ.get("KSM_CONFIG_SKIP_MODE_WARNING", "FALSE"))) is True:
                     retval = True
                 else:
-                    allowed_users = [u.lower() for u in ALLOWED_WINDOWS_CONFIG_ADMINS + [user]]
-                    for line in output.stdout.decode().split("\n"):
-                        parts = line[len(file):].split(":")
-                        if len(parts) == 2:
-                            found_user = parts[0].split("\\").pop()
-                            if found_user.lower() not in allowed_users:
-
-                                message = "The config file mode is too open for '{}'. Use `icacls` to remove access " \
-                                          "for other users and groups.\n\n".format(file)
-                                message += '> icacls.exe "{}" /reset\n'.format(file)
-                                message += '> icacls.exe "{}" /inheritance:r\n'.format(file)
-                                message += '> icacls.exe "{}" /remove:g Everyone:F\n'.format(file)
-                                message += '> icacls.exe "{}" /grant:r Administrators:F\n'.format(file)
-                                message += '> icacls.exe "{}" /grant:r *{}:F\n'.format(file, sid)
-                                message += "\nTo disable this check, set the environmental variable " \
-                                           "'KSM_CONFIG_SKIP_MODE_WARNING' to 'TRUE'."
-                                if color_mod is not None:
-                                    message = color_mod.Fore.RED + message + color_mod.Style.RESET_ALL
-
-                                print(message, file=sys.stderr)
-                                # Prevent multiple nagging per execution.
-                                os.environ["KSM_CONFIG_SKIP_MODE_WARNING"] = "TRUE"
-                                retval = False
-                                break
-                    else:
+                    # We need to figure out who we are. subprocess run will use cmd
+                    sid, user = get_windows_user_sid_and_name()
+                    if sid is None:
+                        # Don't fail check when user SID is missing.
                         retval = True
-        else:
-            # Can the user read the file? First check if the file exists. If it does, os.access might throw
-            # and exception about it not existing. This mean we don't have access.
-            if os.path.exists(file) is True:
-                try:
-                    if os.access(file, os.R_OK) is False:
+                    else:
+                        populate_windows_localized_admin_names_win32api()
+                        allowed_users = set([u.lower() for u in ALLOWED_WINDOWS_CONFIG_ADMINS + localized_admins + [user]])
+                        stdout = output.stdout or b""
+                        for line in stdout.split(b"\n"):
+                            parts = line[len(file):].split(b":")
+                            if len(parts) == 2:
+                                found_user = parts[0].split(b"\\").pop()
+                                if found_user.lower() not in allowed_users:
+
+                                    message = "The config file mode is too open for '{}'. Use `icacls` to remove access " \
+                                            "for other users and groups.\n\n".format(file)
+                                    message += '> icacls.exe "{}" /reset\n'.format(file)
+                                    message += '> icacls.exe "{}" /inheritance:r\n'.format(file)
+                                    message += '> icacls.exe "{}" /remove:g Everyone:F\n'.format(file)
+                                    message += '> icacls.exe "{}" /grant:r Administrators:F\n'.format(file)
+                                    message += '> icacls.exe "{}" /grant:r *{}:F\n'.format(file, sid)
+                                    message += "\nTo disable this check, set the environmental variable " \
+                                            "'KSM_CONFIG_SKIP_MODE_WARNING' to 'TRUE'."
+                                    if color_mod is not None:
+                                        message = color_mod.Fore.RED + message + color_mod.Style.RESET_ALL
+
+                                    print(message, file=sys.stderr)
+                                    # Prevent multiple nagging per execution.
+                                    os.environ["KSM_CONFIG_SKIP_MODE_WARNING"] = "TRUE"
+                                    retval = False
+                                    break
+                        else:
+                            retval = True
+            else:
+                # Can the user read the file? First check if the file exists. If it does, os.access might throw
+                # and exception about it not existing. This mean we don't have access.
+                if os.path.exists(file) is True:
+                    try:
+                        if os.access(file, os.R_OK) is False:
+                            raise PermissionError("Access denied to configuration file {}.".format(file))
+                    except FileNotFoundError:
                         raise PermissionError("Access denied to configuration file {}.".format(file))
-                except FileNotFoundError:
-                    raise PermissionError("Access denied to configuration file {}.".format(file))
 
-            # Allow user to skip being nagged by warning message.
-            if bool(strtobool(os.environ.get("KSM_CONFIG_SKIP_MODE_WARNING", "FALSE"))) is True:
-                retval = True
-            else:
-                mode = oct(os.stat(file).st_mode)
-                # Make sure group and user have no rights. Allow owner to have anything.
-                if mode[-2:] == "00":
+                # Allow user to skip being nagged by warning message.
+                if bool(strtobool(os.environ.get("KSM_CONFIG_SKIP_MODE_WARNING", "FALSE"))) is True:
                     retval = True
                 else:
-                    print("The config file mode, {}, is too open. "
-                          "It is recommended to execute 'chmod 0600 {}' to remove group and user "
-                          "access. To disable this warning, set the environment variable "
-                          "'KSM_CONFIG_SKIP_MODE_WARNING' to 'TRUE'.".format(mode[-4:], file), file=sys.stderr)
-                    retval = False
+                    mode = oct(os.stat(file).st_mode)
+                    # Make sure group and user have no rights. Allow owner to have anything.
+                    if mode[-2:] == "00":
+                        retval = True
+                    else:
+                        print("The config file mode, {}, is too open. "
+                            "It is recommended to execute 'chmod 0600 {}' to remove group and user "
+                            "access. To disable this warning, set the environment variable "
+                            "'KSM_CONFIG_SKIP_MODE_WARNING' to 'TRUE'.".format(mode[-4:], file), file=sys.stderr)
+                        retval = False
+    except (FileNotFoundError, PermissionError):
+        raise
+    except Exception as e:
+        if logger is not None:
+            logger.debug("check_config_mode failed: " + str(e))
 
     return retval
 
 
 def generate_password(length: int = DEFAULT_PASSWORD_LENGTH,
                       lowercase: Optional[int] = None,
                       uppercase: Optional[int] = None,
```

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core.egg-info/PKG-INFO` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-core
-Version: 16.5.2
+Version: 16.5.3
 Summary: Keeper Secrets Manager for Python 3
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://github.com/Keeper-Security/secrets-manager
@@ -27,14 +27,17 @@
 
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.5.3
+* KSM-393 - Fix file permissions on localized Windows OS
+
 ## 16.5.2
 * KSM-375 - Make HTTPError to be more informative
 * KSM-376 - Support for PAM record types
 * KSM-381 - Transactions
 * Fixed [Issue 441](https://github.com/Keeper-Security/secrets-manager/issues/441) - Bug caused by space in username
 
 ## 16.5.1
```

### Comparing `keeper-secrets-manager-core-16.5.2/keeper_secrets_manager_core.egg-info/SOURCES.txt` & `keeper-secrets-manager-core-16.5.3/keeper_secrets_manager_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.2/setup.py` & `keeper-secrets-manager-core-16.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'requests==2.28.2',
     'cryptography>=39.0.1',
     'importlib_metadata==6.0.0'
 ]
 
 setup(
     name="keeper-secrets-manager-core",
-    version="16.5.2",
+    version="16.5.3",
     description="Keeper Secrets Manager for Python 3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Keeper Security",
     author_email="sm@keepersecurity.com",
     url="https://github.com/Keeper-Security/secrets-manager",
     license="MIT",
```

