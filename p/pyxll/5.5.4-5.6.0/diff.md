# Comparing `tmp/pyxll-5.5.4-cp39-none-any.whl.zip` & `tmp/pyxll-5.6.0-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,23 @@
-Zip file size: 55791 bytes, number of entries: 20
-?rw-------  2.0 fat    80555 b- defN 22-Dec-23 15:51 pyxll/__init__.py
-?rw-------  2.0 fat     4575 b- defN 22-Dec-23 15:51 pyxll/_cli.py
-?rw-------  2.0 fat    46065 b- defN 22-Dec-23 15:51 pyxll/_utils.py
-?rw-------  2.0 fat      480 b- defN 22-Dec-23 15:51 pyxll/_errors.py
-?rw-------  2.0 fat    12076 b- defN 22-Dec-23 15:51 pyxll/_check.py
-?rw-------  2.0 fat    15396 b- defN 22-Dec-23 15:51 pyxll/_install.py
-?rw-------  2.0 fat    13439 b- defN 22-Dec-23 15:51 pyxll/_update.py
-?rw-------  2.0 fat     7831 b- defN 22-Dec-23 15:51 pyxll/_activate.py
-?rw-------  2.0 fat     4632 b- defN 22-Dec-23 15:51 pyxll/_config.py
-?rw-------  2.0 fat     2213 b- defN 22-Dec-23 15:51 pyxll/_uninstall.py
-?rw-------  2.0 fat     5382 b- defN 22-Dec-23 15:51 pyxll/_cert.py
-?rw-------  2.0 fat       86 b- defN 22-Dec-23 15:51 pyxll/__main__.py
-?rw-------  2.0 fat     2264 b- defN 22-Dec-23 15:51 pyxll/pyxll.crt
-?rw-------  2.0 fat       42 b- defN 22-Dec-23 15:51 pyxll-5.5.4.dist-info/entry_points.txt
-?rw-------  2.0 fat      357 b- defN 22-Dec-23 15:51 pyxll-5.5.4.dist-info/DESCRIPTION.rst
-?rw-------  2.0 fat     3802 b- defN 22-Dec-23 15:51 pyxll-5.5.4.dist-info/METADATA
-?rw-------  2.0 fat      611 b- defN 22-Dec-23 15:51 pyxll-5.5.4.dist-info/metadata.json
-?rw-------  2.0 fat        6 b- defN 22-Dec-23 15:51 pyxll-5.5.4.dist-info/top_level.txt
-?rw-------  2.0 fat       87 b- defN 22-Dec-23 15:51 pyxll-5.5.4.dist-info/WHEEL
-?rw-------  2.0 fat     1535 b- defN 22-Dec-23 15:51 pyxll-5.5.4.dist-info/RECORD
-20 files, 201434 bytes uncompressed, 53373 bytes compressed:  73.5%
+Zip file size: 60041 bytes, number of entries: 21
+?rw-------  2.0 fat    81739 b- defN 23-Apr-17 11:58 pyxll/__init__.py
+?rw-------  2.0 fat     4575 b- defN 23-Apr-17 11:58 pyxll/_cli.py
+?rw-------  2.0 fat    48379 b- defN 23-Apr-17 11:58 pyxll/_utils.py
+?rw-------  2.0 fat      480 b- defN 23-Apr-17 11:58 pyxll/_errors.py
+?rw-------  2.0 fat    10904 b- defN 23-Apr-17 11:58 pyxll/_check.py
+?rw-------  2.0 fat    14417 b- defN 23-Apr-17 11:58 pyxll/_install.py
+?rw-------  2.0 fat    12431 b- defN 23-Apr-17 11:58 pyxll/_update.py
+?rw-------  2.0 fat     6826 b- defN 23-Apr-17 11:58 pyxll/_activate.py
+?rw-------  2.0 fat     4632 b- defN 23-Apr-17 11:58 pyxll/_config.py
+?rw-------  2.0 fat     2226 b- defN 23-Apr-17 11:58 pyxll/_uninstall.py
+?rw-------  2.0 fat     5382 b- defN 23-Apr-17 11:58 pyxll/_cert.py
+?rw-------  2.0 fat    16705 b- defN 23-Apr-17 11:58 pyxll/_admin.py
+?rw-------  2.0 fat       86 b- defN 23-Apr-17 11:58 pyxll/__main__.py
+?rw-------  2.0 fat     2264 b- defN 23-Apr-17 11:58 pyxll/pyxll.crt
+?rw-------  2.0 fat       42 b- defN 23-Apr-17 11:58 pyxll-5.6.0.dist-info/entry_points.txt
+?rw-------  2.0 fat      357 b- defN 23-Apr-17 11:58 pyxll-5.6.0.dist-info/DESCRIPTION.rst
+?rw-------  2.0 fat     3802 b- defN 23-Apr-17 11:58 pyxll-5.6.0.dist-info/METADATA
+?rw-------  2.0 fat      611 b- defN 23-Apr-17 11:58 pyxll-5.6.0.dist-info/metadata.json
+?rw-------  2.0 fat        6 b- defN 23-Apr-17 11:58 pyxll-5.6.0.dist-info/top_level.txt
+?rw-------  2.0 fat       87 b- defN 23-Apr-17 11:58 pyxll-5.6.0.dist-info/WHEEL
+?rw-------  2.0 fat     1609 b- defN 23-Apr-17 11:58 pyxll-5.6.0.dist-info/RECORD
+21 files, 217560 bytes uncompressed, 57517 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -27,35 +27,38 @@
 
 Filename: pyxll/_uninstall.py
 Comment: 
 
 Filename: pyxll/_cert.py
 Comment: 
 
+Filename: pyxll/_admin.py
+Comment: 
+
 Filename: pyxll/__main__.py
 Comment: 
 
 Filename: pyxll/pyxll.crt
 Comment: 
 
-Filename: pyxll-5.5.4.dist-info/entry_points.txt
+Filename: pyxll-5.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyxll-5.5.4.dist-info/DESCRIPTION.rst
+Filename: pyxll-5.6.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: pyxll-5.5.4.dist-info/METADATA
+Filename: pyxll-5.6.0.dist-info/METADATA
 Comment: 
 
-Filename: pyxll-5.5.4.dist-info/metadata.json
+Filename: pyxll-5.6.0.dist-info/metadata.json
 Comment: 
 
-Filename: pyxll-5.5.4.dist-info/top_level.txt
+Filename: pyxll-5.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyxll-5.5.4.dist-info/WHEEL
+Filename: pyxll-5.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyxll-5.5.4.dist-info/RECORD
+Filename: pyxll-5.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyxll/__init__.py

```diff
@@ -25,15 +25,15 @@
 import traceback
 import datetime
 import logging
 import sys
 
 _log = logging.getLogger(__name__)
 
-__version__ = "5.5.4"
+__version__ = "5.6.0"
 
 nan = 1e10000 * 0
 
 xlCalculationAutomatic = 1
 xlCalculationSemiAutomatic = 2
 xlCalculationManual = 3
 
@@ -384,53 +384,14 @@
             if exc_type is None:
                 return "No error"
 
             return "".join(traceback.format_exception_only(exc_type, exc_value))
     """
     raise Exception("Not supported when running outside of Excel")
 
-def load_image(filename):
-    # type: (str) -> _COMObject
-    """
-    Loads an image file and returns it as a COM IPicture object suitable for use when
-    customizing the ribbon.
-
-    This function can be set at the Ribbon image handler by setting the loadImage attribute on
-    the customUI element in the ribbon XML file.
-
-    .. code-block:: xml
-        :emphasize-lines: 2, 11
-
-        <customUI xmlns="http://schemas.microsoft.com/office/2006/01/customui"
-                    loadImage="pyxll.load_image">
-            <ribbon>
-                <tabs>
-                    <tab id="CustomTab" label="Custom Tab">
-                        <group id="Tools" label="Tools">
-                            <button id="Reload"
-                                    size="large"
-                                    label="Reload PyXLL"
-                                    onAction="pyxll.reload"
-                                    image="reload.png"/>
-                        </group>
-                    </tab>
-                </tabs>
-            </ribbon>
-        </customUI>
-
-    Or it can be used when returning an image from a getImage callback.
-
-    :param string filename: Filename of the image file to load. This may be an absolute path or relative to
-                            the ribbon XML file.
-
-    :return: A COM IPicture object (the exact type depends
-                on the com_package setting in the config file.
-    """
-    raise Exception("Not supported when running outside of Excel")
-
 def cached_object_count():
     # type: () -> int
     """Return the number of objects cached in the internal object cache"""
     return 0
 
 def message_box(message, caption="", flags=0):
     # type: (str, str, int) -> None
@@ -1199,14 +1160,84 @@
             updated = True
 
     if not updated:
         return False
 
     set_ribbon_xml(new_xml, reload=reload, keep_merged_attrs=True)
 
+_ribbon_xml = None
+
+def load_image(filename):
+    # type: (str) -> _COMObject
+    """
+    Loads an image file and returns it as a COM IPicture object suitable for use when
+    customizing the ribbon.
+
+    This function can be set at the Ribbon image handler by setting the loadImage attribute on
+    the customUI element in the ribbon XML file.
+
+    .. code-block:: xml
+        :emphasize-lines: 2, 11
+
+        <customUI xmlns="http://schemas.microsoft.com/office/2006/01/customui"
+                    loadImage="pyxll.load_image">
+            <ribbon>
+                <tabs>
+                    <tab id="CustomTab" label="Custom Tab">
+                        <group id="Tools" label="Tools">
+                            <button id="Reload"
+                                    size="large"
+                                    label="Reload PyXLL"
+                                    onAction="pyxll.reload"
+                                    image="reload.png"/>
+                        </group>
+                    </tab>
+                </tabs>
+            </ribbon>
+        </customUI>
+
+    Or it can be used when returning an image from a getImage callback.
+
+    :param string filename: Filename of the image file to load. This may be an absolute path or relative to
+                            the ribbon XML file.
+
+    :return: A COM IPicture object (the exact type depends
+                on the com_package setting in the config file.
+    """
+    raise Exception("Not supported when running outside of Excel")
+
+def get_ribbon_xml():
+    # type: () -> str
+    """Returns the ribbon XML currenly in use by PyXLL."""
+    return _ribbon_xml
+
+def set_ribbon_xml(xml, reload=True, keep_merged_attrs=False):
+    # type: (Union[str, minidom.Document], bool) -> None
+    """
+    Sets the XML used by PyXLL for customizing the ribbon.
+
+    :param xml: XML document to set as the current ribbon
+    :param reload: If true the ribbon will be refreshed immediately.
+    """
+
+    _validate_ribbon_xml(xml)
+
+    if _have_minidom:
+        if isinstance(xml, minidom.Document):
+            xml = xml.toxml()
+
+    global _ribbon_xml
+    _ribbon_xml = xml
+
+def get_ribbon_ui():
+    # type: (str) -> _COMObject
+    """Returns the Ribbon COM object.
+    """
+    raise Exception("Not supported when running outside of Excel")
+
 class ErrorContext:
     """Context object passed to the PyXLL error handler."""
 
     class Type:
         """Type to indicate the origination of the error."""
         UDF = "udf"
         MACRO = "macro"
@@ -1310,14 +1341,28 @@
     # This will work but won't add constants to win32com.client.constants.
     import win32com
     _log.warning("win32com.client.Dispatch failed. win32com.client.dynamic.Dispatch will be used instead.")
     _log.warning("Delete your gen_py folder '%s' as it may have become corrupted" % win32com.__gen_path__)
     from win32com.client.dynamic import Dispatch as DynamicDispatch
     return DynamicDispatch(disp)
 
+def _get_iunknown_package(unk):
+    """Return the com package the object is most likely to be from"""
+    try:
+        package = unk.__class__.__module__.split(".", 1)[0]
+        if package in ("comtypes", "xlwings"):
+            return package
+    except AttributeError:
+        pass
+
+    if hasattr(unk, "_oleobj_"):
+        return "win32com"
+
+    return "pythoncom"
+
 class BaseFormatter(object):
     """Base class used for formatting Excel ranges.
     """
     @classmethod
     def __get_numpy(cls):
         try:
             return cls.__np
```

## pyxll/_utils.py

```diff
@@ -402,15 +402,15 @@
 
 def _get_xll_version_info(dll_path):
     """Return tuple (name, version, py version)"""
     internal_name = _get_dll_file_info(dll_path, "InternalName")
 
     # InternalName should be in the form "pyxll-<version>-<py version>"
     # but older versions of PyXLL (< 4.6) do not have this.
-    match = re.match(r"^([a-z]+)\-(.+)\-(py\d{2})$", internal_name, re.IGNORECASE)
+    match = re.match(r"^([a-z]+)\-(.+)\-(py\d{2,3})$", internal_name, re.IGNORECASE)
     if not match:
         _log.debug("Could not extract version information from InternalName '%s'." % internal_name)
         return None
 
     return match.group(1), match.group(2), match.group(3)
 
 def _get_xll_file_version(dll_path):
@@ -1227,8 +1227,52 @@
         try:
             _log.debug("Removing Zone.Identifier information from '%s'." % filename)
             os.remove(filename + ":Zone.Identifier")
         except:
             _log.warning("Error unblocking '%s'." % filename, exc_info=_log.getEffectiveLevel() <= logging.DEBUG)
             _log.warning("Excel will not be able to load '%s' until it is unblocked." % filename)
             _log.warning("To unblock the file right click on it in Explorer and go to Properties, then "
-                         "check the 'Unblock' checkbox next to 'Security' in the 'General' tab.")
+                         "check the 'Unblock' checkbox next to 'Security' in the 'General' tab.")
+
+def _is_admin():
+    try:
+        from ._admin import process_user_is_admin
+        kernel32 = ctypes.windll.kernel32
+        kernel32.GetCurrentProcessId.argtypes = []
+        kernel32.GetCurrentProcessId.rettype = ctypes.wintypes.DWORD
+        pid = kernel32.GetCurrentProcessId()
+        return process_user_is_admin(pid)
+    except:
+        _log.warning("Checking if current user is admin failed", exc_info=_log.getEffectiveLevel() <= logging.DEBUG)
+        return False
+
+def _find_and_check_excel():
+    excel_exe = _find_excel_path()
+    if not excel_exe:
+        if _is_admin():
+            _log.warning("It looks like you are running this command as an administrator user. "
+                         "Excel may not be installed for your admin user.")
+            _log.warning("You should run this command using the same user Excel is installed for.")
+        raise Error(("Excel does not appear to be installed.\n\n"
+                     "Please ensure that Excel is installed correctly and try again."))
+
+    # Check the bitness of Excel matches Python
+    excel_bits = _get_exe_bitness(excel_exe)
+    python_bits = _get_exe_bitness(sys.executable)
+    if python_bits != excel_bits:
+        raise Error(("Excel is %(excel_bits)s but Python is %(python_bits)s.\n\n"
+                     "Please check the version of Office you have installed and either install "
+                     "the %(python_bits)s version of Excel or install a %(excel_bits)s version of Python.")
+                    % {"excel_bits": excel_bits, "python_bits": python_bits})
+
+    xl_version_info = _find_excel_version_info(python_bits)
+    if xl_version_info is None:
+        if _is_admin():
+            _log.warning("It looks like you are running this command as an administrator user. "
+                         "Excel may not be installed for your admin user.")
+            _log.warning("You should run this command using the same user Excel is installed for.")
+        raise Error(("Excel does not appear to be installed.\n\n"
+                     "Please ensure that Excel is installed correctly and try again."))
+
+    excel_version, hkey_root, excel_subkey, flags = xl_version_info
+    _log.debug("Found %s Excel %s installed: %s" % (excel_bits, excel_version, excel_exe))
+    return excel_exe, excel_bits, xl_version_info
```

## pyxll/_check.py

```diff
@@ -4,21 +4,20 @@
 THIS CODE AND INFORMATION ARE PROVIDED "AS IS" WITHOUT WARRANTY OF ANY
 KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND/OR FITNESS FOR A
 PARTICULAR PURPOSE.
 """
 from ._cli import Error, Help
 from ._utils import (
-    _get_exe_bitness,
+    _find_and_check_excel,
     _get_dll_bitness,
+    _get_exe_bitness,
     _get_xll_version_info,
     _get_xll_file_version,
     _find_pyxll_config,
-    _find_excel_version_info,
-    _find_excel_path,
     _find_pyxll_addin,
     _load_config_file
 )
 import logging
 import sys
 import os
 
@@ -142,40 +141,16 @@
     return True
 
 def check(*args):
     if args:
         raise Help("Unexpected arguments '%s' to command 'check'." % ", ".join(args))
 
     # Check Excel is installed and exists
-    excel_exe = _find_excel_path()
-    if not excel_exe:
-        raise Error(("Excel does not appear to be installed.\n\n"
-                    "Please ensure that Excel is installed correctly and try again."))
-
-    _log.debug("Found Excel executable '%s'." % excel_exe)
-
-    # Check the bitness of Excel matches Python
-    excel_bits = _get_exe_bitness(excel_exe)
-    python_bits = _get_exe_bitness(sys.executable)
-    _log.debug("Excel is %s and Python is %s." % (excel_bits, python_bits))
-
-    if python_bits != excel_bits:
-        raise Error(("Excel is %(excel_bits)s but Python is %(python_bits)s.\n\n"
-                     "Please check the version of Office you have installed and either install "
-                     "the %(python_bits)s version of Excel or install a %(excel_bits)s version of Python.")
-                        % {"excel_bits": excel_bits, "python_bits": python_bits})
-
-    # Find the excel options in the registry
-    excel_version_info = _find_excel_version_info(excel_bits)
-    if not excel_version_info:
-        raise Error(("Unable to locate the Excel settings in the registry.\n\n"
-                     "Please ensure that Excel is installed correctly and try again."))
-
-    excel_version, hkey_root, excel_subkey, flags = excel_version_info
-    _log.debug("Found Excel version '%s'." % excel_version)
+    excel_exe, excel_bits, xl_version_info = _find_and_check_excel()
+    excel_version, hkey_root, excel_subkey, flags = xl_version_info
 
     # Look to see if PyXLL is installed and check the file exists
     pyxll_path = _find_pyxll_addin(hkey_root, excel_subkey, flags)
     if not pyxll_path:
         raise Error(("PyXLL is not installed.\n\n"
                      "You can install PyXLL by running:\n\n"
                      "pyxll install\n\n"
@@ -196,16 +171,17 @@
                      pyxll_path + "\n\n"
                                   "You can re-install PyXLL by running:\n\n"
                                   "pyxll install\n\n"
                                   "or see the PyXLL website https://www.pyxll.com for installation instructions."))
 
     # Check the installed version of PyXLL is the correct bitness
     pyxll_bits = _get_dll_bitness(pyxll_path)
+    python_bits = _get_exe_bitness(sys.executable)
     if pyxll_bits != python_bits:
-        raise Error(("Excel and Python are %(excel_bits)s but the installed PyXLL add-in is %(pyxll_bits)s.\n\n"
+        raise Error(("Excel is Python are %(excel_bits)s but the installed PyXLL add-in is %(pyxll_bits)s.\n\n"
                      "You should download the %(excel_bits)s version of PyXLL and install that, or "
                      "you can use the following command to re-install PyXLL:\n\n"
                      "pyxll install\n\n"
                      "See the PyXLL website https://www.pyxll.com for detailed installation instructions.")
                     % {"excel_bits": excel_bits, "python_bits": python_bits, "pyxll_bits": pyxll_bits})
 
     _log.debug("The installed PyXLL add-in is %s." % pyxll_bits)
```

## pyxll/_install.py

```diff
@@ -9,18 +9,17 @@
 from ._errors import Help, Error
 from ._cert import _install_certificate
 from ._utils import (
     AutoDeleteFile,
     AutoDeleteFolder,
     _print,
     _input,
-    _find_excel_version_info,
-    _find_excel_path,
-    _get_exe_bitness,
+    _find_and_check_excel,
     _get_dll_bitness,
+    _get_exe_bitness,
     _check_excel_is_not_running,
     _check_python_exe,
     _find_pyxll_addin,
     _uninstall_pyxll_addin,
     _get_xll_version_info,
     _get_xll_file_version,
     _unzip_pyxll,
@@ -77,50 +76,31 @@
     if unexpected_args:
         raise Help("Unexpected arguments '%s' to command 'install'." % ", ".join(unexpected_args))
 
     _check_python_exe()
     _check_excel_is_not_running()
 
     # Check Excel is installed and exists
-    excel_exe = _find_excel_path()
-    if not excel_exe:
-        raise Error(("Excel does not appear to be installed.\n\n"
-                     "Please ensure that Excel is installed correctly and try again."))
-
-    bits = platform.architecture()[0]
-    xl_version_info = _find_excel_version_info(bits)
-    if xl_version_info is None:
-        raise Error(("Excel does not appear to be installed.\n\n"
-                     "Please ensure that Excel is installed correctly and try again."))
-
+    excel_exe, excel_bits, xl_version_info = _find_and_check_excel()
     xl_version, root_hkey, subkey, flags = xl_version_info
-    print(("Found Excel %s installed" % xl_version))
+    python_bits = _get_exe_bitness(sys.executable)
 
     # See if PyXLL is already installed
     existing_pyxll_path = _find_pyxll_addin(root_hkey, subkey, flags)
     if existing_pyxll_path and os.path.exists(existing_pyxll_path):
-        print(("\nA previously installed PyXLL add-in was found '%s'" % existing_pyxll_path))
-        print("You can use 'pyxll update' to update PyXLL rather than re-install it.")
+        _print("\nA previously installed PyXLL add-in was found '%s'" % existing_pyxll_path)
+        _print("You can use 'pyxll update' to update PyXLL rather than re-install it.")
         response = None
         while response not in ("y", "n"):
-            response = _input("Do you want to continue ([y]/n)? ").strip().lower()
+            response = _input("Do you want to continue ([y]/n)? ", default="y").strip().lower()
             if not response:
                 response = "y"
         if response != "y":
             return 1
 
-    # Check the bitness of Excel matches Python
-    excel_bits = _get_exe_bitness(excel_exe)
-    python_bits = _get_exe_bitness(sys.executable)
-    if python_bits != excel_bits:
-        raise Error(("Excel is %(excel_bits)s but Python is %(python_bits)s.\n\n"
-                     "Please check the version of Office you have installed and either install "
-                     "the %(python_bits)s version of Excel or install a %(excel_bits)s version of Python.")
-                    % {"excel_bits": excel_bits, "python_bits": python_bits})
-
     # Look for pyxll in the current directory if we don't already have the download path
     if not pyxll_download_path:
         cwd = os.getcwd()
         if os.path.exists(os.path.join(cwd, "pyxll.xll")) and os.path.exists(os.path.join(cwd, "pyxll.cfg")):
             response = None
             _print("\nA PyXLL add-in was found in the current folder.")
             while response not in ("y", "n"):
```

## pyxll/_update.py

```diff
@@ -9,31 +9,29 @@
 from ._errors import Help, Error
 from ._cert import _install_certificate
 from ._utils import (
     AutoDeleteFile,
     AutoDeleteFolder,
     _print,
     _input,
-    _find_excel_version_info,
+    _find_and_check_excel,
     _get_latest_pyxll_version,
     _compare_pyxll_versions,
-    _find_excel_path,
-    _get_exe_bitness,
     _get_dll_bitness,
+    _get_exe_bitness,
     _check_excel_is_not_running,
     _check_python_exe,
     _find_pyxll_addin,
     _get_xll_version_info,
     _get_xll_file_version,
     _download_pyxll,
     _unzip_pyxll,
     _backup_files,
     _clear_zone_identifier
 )
-import platform
 import tempfile
 import logging
 import shutil
 import glob
 import sys
 import os
 
@@ -75,27 +73,17 @@
     if unexpected_args:
         raise Help("Unexpected arguments '%s' to command 'update'." % ", ".join(unexpected_args))
 
     _check_python_exe()
     _check_excel_is_not_running()
 
     # Check Excel is installed and exists
-    excel_exe = _find_excel_path()
-    if not excel_exe:
-        raise Error(("Excel does not appear to be installed.\n\n"
-                     "Please ensure that Excel is installed correctly and try again."))
-
-    bits = platform.architecture()[0]
-    xl_version_info = _find_excel_version_info(bits)
-    if xl_version_info is None:
-        raise Error(("Excel does not appear to be installed.\n\n"
-                     "Please ensure that Excel is installed correctly and try again."))
-
+    excel_exe, excel_bits, xl_version_info = _find_and_check_excel()
     xl_version, root_hkey, subkey, flags = xl_version_info
-    print(("Found Excel %s installed" % xl_version))
+    python_bits = _get_exe_bitness(sys.executable)
 
     # Check PyXLL is already installed
     pyxll_path = _find_pyxll_addin(root_hkey, subkey, flags)
     if not pyxll_path or not os.path.exists(pyxll_path):
         raise Error(("No existing install of PyXLL was found.\n\n"
                      "Please use the 'pyxll install' to install PyXLL instead."))
 
@@ -113,23 +101,14 @@
     _print("\nPyXLL is installed in '%s'." % os.path.dirname(pyxll_path))
     _print("\nYour existing PyXLL add-in will be backed up before updating.")
     _print("\nYour existing pyxll.cfg file will *not* be changed and any new "
             "examples will not be installed.")
     _print("\nIf you want to try out a new version before updating use 'pyxll install' "
             "and install PyXLL into a different folder than your current installation.")
 
-    # Check the bitness of Excel matches Python
-    excel_bits = _get_exe_bitness(excel_exe)
-    python_bits = _get_exe_bitness(sys.executable)
-    if python_bits != excel_bits:
-        raise Error(("Excel is %(excel_bits)s but Python is %(python_bits)s.\n\n"
-                     "Please check the version of Office you have installed and either install "
-                     "the %(python_bits)s version of Excel or install a %(excel_bits)s version of Python.")
-                    % {"excel_bits": excel_bits, "python_bits": python_bits})
-
     # Find or download PyXLL
     pyxll_install_path = os.path.dirname(pyxll_path)
 
     # Look for pyxll in the current directory (if it's not the folder PyXLL is installed in)
     if not pyxll_download_path:
         cwd = os.getcwd()
         if os.path.normpath(pyxll_install_path) != os.path.normpath(cwd) \
```

## pyxll/_activate.py

```diff
@@ -6,27 +6,25 @@
 IMPLIED WARRANTIES OF MERCHANTABILITY AND/OR FITNESS FOR A
 PARTICULAR PURPOSE.
 """
 from ._cli import Help, Error, _print
 from ._cert import _install_certificate
 from ._utils import (
     _input,
-    _find_excel_version_info,
-    _find_excel_path,
-    _get_exe_bitness,
+    _find_and_check_excel,
     _get_dll_bitness,
+    _get_exe_bitness,
     _check_excel_is_not_running,
     _find_pyxll_addin,
     _get_xll_version_info,
     _get_xll_file_version,
     _uninstall_pyxll_addin,
     _install_pyxll_addin,
     _clear_zone_identifier
 )
-import platform
 import logging
 import sys
 import os
 
 _log = logging.getLogger(__name__)
 
 def activate(*args):
@@ -40,36 +38,16 @@
 
     if unexpected_args:
         raise Help("Unexpected arguments '%s' to command 'activate'." % ", ".join(unexpected_args))
 
     _check_excel_is_not_running()
 
     # Check Excel is installed and exists
-    excel_exe = _find_excel_path()
-    if not excel_exe:
-        raise Error(("Excel does not appear to be installed.\n\n"
-                     "Please ensure that Excel is installed correctly and try again."))
-
-    bits = platform.architecture()[0]
-    xl_version_info = _find_excel_version_info(bits)
-    if xl_version_info is None:
-        raise Error(("Excel does not appear to be installed.\n\n"
-                     "Please ensure that Excel is installed correctly and try again."))
-
+    excel_exe, excel_bits, xl_version_info = _find_and_check_excel()
     xl_version, root_hkey, subkey, flags = xl_version_info
-    print(("Found Excel %s installed" % xl_version))
-
-    # Check the bitness of Excel matches Python
-    excel_bits = _get_exe_bitness(excel_exe)
-    python_bits = _get_exe_bitness(sys.executable)
-    if python_bits != excel_bits:
-        raise Error(("Excel is %(excel_bits)s but Python is %(python_bits)s.\n\n"
-                     "Please check the version of Office you have installed and either install "
-                     "the %(python_bits)s version of Excel or install a %(excel_bits)s version of Python.")
-                    % {"excel_bits": excel_bits, "python_bits": python_bits})
 
     # Look for pyxll in the current directory
     if not pyxll_install_path:
         cwd = os.getcwd()
         if os.path.exists(os.path.join(cwd, "pyxll.xll")) and os.path.exists(os.path.join(cwd, "pyxll.cfg")):
             response = None
             _print("\nA PyXLL add-in was found in the current folder.")
@@ -85,29 +63,29 @@
         _print("")
         while True:
             pyxll_install_path = _input("Enter the path where PyXLL is located: ", is_path=True).strip()
             if not pyxll_install_path:
                 continue
 
             if not os.path.exists(pyxll_install_path):
-                print("The path entered does not exist. Please try again.")
+                _print("The path entered does not exist. Please try again.")
                 continue
 
             if os.path.isfile(pyxll_install_path):
                 if os.path.basename(pyxll_install_path).lower() == "pyxll.xll":
                     pyxll_install_path = os.path.dirname(pyxll_install_path)
                     break
 
-                print("The entered path does not look like a PyXLL add-in. Please try again.")
+                _print("The entered path does not look like a PyXLL add-in. Please try again.")
                 continue
 
             elif os.path.isdir(pyxll_install_path):
                 if os.path.exists(os.path.join(pyxll_install_path, "pyxll.xll")):
                     break
-                print("pyxll.xll is missing from the folder specified. Please try again.")
+                _print("pyxll.xll is missing from the folder specified. Please try again.")
                 continue
 
     # Check the install path looks ok
     if not os.path.exists(pyxll_install_path):
         raise Error("The path '%s' does not exist." % pyxll_install_path)
 
     if os.path.isfile(pyxll_install_path):
@@ -119,14 +97,15 @@
     pyxll_install_path = os.path.abspath(pyxll_install_path)
     pyxll_xll_path = os.path.join(pyxll_install_path, "pyxll.xll")
     if not os.path.exists(pyxll_xll_path):
         raise Error("Couldn't find pyxll.xll file in '%s'" % pyxll_install_path)
 
     # Check the installed version of PyXLL is the correct bitness
     pyxll_bits = _get_dll_bitness(pyxll_xll_path)
+    python_bits = _get_exe_bitness(sys.executable)
     if pyxll_bits != python_bits:
         raise Error(("Excel and Python are %(excel_bits)s but the PyXLL add-in is %(python_bits)s.\n\n"
                      "You should download the %(excel_bits)s version of PyXLL and install that, or "
                      "you can use the following command to re-install PyXLL:\n\n"
                      "pyxll install\n\n"
                      "See the PyXLL website https://www.pyxll.com for detailed installation instructions.")
                     % {"excel_bits": excel_bits, "python_bits": python_bits, "pyxll_bits": pyxll_bits})
```

## pyxll/_uninstall.py

```diff
@@ -4,14 +4,15 @@
 THIS CODE AND INFORMATION ARE PROVIDED "AS IS" WITHOUT WARRANTY OF ANY
 KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND/OR FITNESS FOR A
 PARTICULAR PURPOSE.
 """
 from ._errors import Help
 from ._utils import (
+    _print,
     _input,
     _find_excel_version_info,
     _find_pyxll_addin,
     _uninstall_pyxll_addin,
     _check_excel_is_not_running,
     _wow64_flags
 )
@@ -50,27 +51,27 @@
 
         xl_version, root_hkey, subkey, flags = xl_version_info
         pyxll_path = _find_pyxll_addin(root_hkey, subkey, flags)
         if pyxll_path:
             break
 
     if not pyxll_path:
-        print("The PyXLL Excel add-in is not installed.")
+        _print("The PyXLL Excel add-in is not installed.")
         return 0
 
     xl_version, root_hkey, subkey, flags = xl_version_info
-    print(("Found PyXLL installed in Excel %s" % xl_version))
-    print(("The PyXLL add-in location is '%s'" % pyxll_path))
+    _print("Found PyXLL installed in Excel %s" % xl_version)
+    _print("The PyXLL add-in location is '%s'" % pyxll_path)
 
     if not force:
         response = None
         while response not in ("y", "n"):
             response = _input("Do you want to uninstall this add-in ([y]/n)? ", default="y").strip().lower()
             if not response:
                 response = "y"
 
         if response != "y":
-            print("Uninstalling has been cancelled")
+            _print("Uninstalling has been cancelled")
             return 1
 
     _uninstall_pyxll_addin(root_hkey, subkey, flags, pyxll_path, dry_run)
-    print("Uninstall of the PyXLL Excel add-in is complete.")
+    _print("Uninstall of the PyXLL Excel add-in is complete.")
```

## Comparing `pyxll-5.5.4.dist-info/METADATA` & `pyxll-5.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxll
-Version: 5.5.4
+Version: 5.6.0
 Summary: Write Microsoft Excel Add-Ins in Python
 Home-page: https://www.pyxll.com
 Author: PyXLL Ltd
 Author-email: info@pyxll.com
 License: Other/Proprietary License
 Platform: Windows
 Classifier: Development Status :: 6 - Mature
```

## Comparing `pyxll-5.5.4.dist-info/metadata.json` & `pyxll-5.6.0.dist-info/metadata.json`

 * *Files 25% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'version'": "'5.6.0'"}*

```diff
@@ -17,9 +17,9 @@
         }
     },
     "generator": "pyxll_makewheel",
     "license": "Commercial",
     "metadata_version": "2.0",
     "name": "PyXLL",
     "summary": "Write Microsoft Excel Add-Ins in Python",
-    "version": "5.5.4"
+    "version": "5.6.0"
 }
```

