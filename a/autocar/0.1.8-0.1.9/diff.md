# Comparing `tmp/autocar-0.1.8.tar.gz` & `tmp/autocar-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocar-0.1.8.tar", last modified: Mon Mar 13 01:47:50 2023, max compression
+gzip compressed data, was "autocar-0.1.9.tar", last modified: Wed Mar 15 00:44:04 2023, max compression
```

## Comparing `autocar-0.1.8.tar` & `autocar-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       66 2023-03-13 01:34:08.955908 autocar-0.1.8/.gitattributes
--rw-r--r--   0        0        0     2763 2023-03-13 01:34:08.955908 autocar-0.1.8/.gitignore
--rw-r--r--   0        0        0     1056 2023-03-13 01:34:08.955908 autocar-0.1.8/LICENSE
--rw-r--r--   0        0        0       12 2023-03-13 01:34:08.955908 autocar-0.1.8/README.md
--rw-r--r--   0        0        0       39 2023-03-13 01:45:48.271745 autocar-0.1.8/autocar/__init__.py
--rw-r--r--   0        0        0    27883 2023-03-13 01:34:08.955908 autocar-0.1.8/autocar/automate_po_process.py
--rw-r--r--   0        0        0    34333 2023-03-13 01:34:08.955908 autocar-0.1.8/autocar/ava.py
--rw-r--r--   0        0        0     1421 2023-03-13 01:34:08.955908 autocar-0.1.8/autocar/merge_pdf.py
--rw-r--r--   0        0        0    16280 2023-03-13 01:34:08.955908 autocar-0.1.8/autocar/print_pdf.py
--rw-r--r--   0        0        0     2141 2023-03-13 01:34:08.955908 autocar-0.1.8/autocar/print_po.py
--rw-r--r--   0        0        0    13170 2023-03-13 01:34:08.955908 autocar-0.1.8/autocar/qad_keyboard_automation.py
--rw-r--r--   0        0        0     2854 2023-03-13 01:34:08.955908 autocar-0.1.8/autocar/update_standard_pricelist.py
--rw-r--r--   0        0        0     3753 2023-03-13 01:43:19.042314 autocar-0.1.8/autocar/voucher_maintenance.py
--rw-r--r--   0        0        0      582 2023-03-13 01:34:08.955908 autocar-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       86 2023-03-13 01:34:08.955908 autocar-0.1.8/requirements.txt
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 autocar-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-03-15 00:41:27.763067 autocar-0.1.9/.gitattributes
+-rw-r--r--   0        0        0     2763 2023-03-15 00:41:27.763067 autocar-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1056 2023-03-15 00:41:27.763067 autocar-0.1.9/LICENSE
+-rw-r--r--   0        0        0       12 2023-03-15 00:41:27.763067 autocar-0.1.9/README.md
+-rw-r--r--   0        0        0       39 2023-03-15 00:43:21.850978 autocar-0.1.9/autocar/__init__.py
+-rw-r--r--   0        0        0    27883 2023-03-15 00:41:27.767067 autocar-0.1.9/autocar/automate_po_process.py
+-rw-r--r--   0        0        0    34333 2023-03-15 00:41:27.767067 autocar-0.1.9/autocar/ava.py
+-rw-r--r--   0        0        0     1421 2023-03-15 00:41:27.767067 autocar-0.1.9/autocar/merge_pdf.py
+-rw-r--r--   0        0        0    16280 2023-03-15 00:41:27.767067 autocar-0.1.9/autocar/print_pdf.py
+-rw-r--r--   0        0        0     2141 2023-03-15 00:41:27.767067 autocar-0.1.9/autocar/print_po.py
+-rw-r--r--   0        0        0    13170 2023-03-15 00:41:27.767067 autocar-0.1.9/autocar/qad_keyboard_automation.py
+-rw-r--r--   0        0        0     2854 2023-03-15 00:41:27.767067 autocar-0.1.9/autocar/update_standard_pricelist.py
+-rw-r--r--   0        0        0     3947 2023-03-15 00:43:01.046995 autocar-0.1.9/autocar/voucher_maintenance.py
+-rw-r--r--   0        0        0      582 2023-03-15 00:41:27.767067 autocar-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-03-15 00:41:27.767067 autocar-0.1.9/requirements.txt
+-rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 autocar-0.1.9/PKG-INFO
```

### Comparing `autocar-0.1.8/.gitignore` & `autocar-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `autocar-0.1.8/LICENSE` & `autocar-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autocar-0.1.8/autocar/automate_po_process.py` & `autocar-0.1.9/autocar/automate_po_process.py`

 * *Files identical despite different names*

### Comparing `autocar-0.1.8/autocar/ava.py` & `autocar-0.1.9/autocar/ava.py`

 * *Files identical despite different names*

### Comparing `autocar-0.1.8/autocar/merge_pdf.py` & `autocar-0.1.9/autocar/merge_pdf.py`

 * *Files identical despite different names*

### Comparing `autocar-0.1.8/autocar/print_pdf.py` & `autocar-0.1.9/autocar/print_pdf.py`

 * *Files identical despite different names*

### Comparing `autocar-0.1.8/autocar/print_po.py` & `autocar-0.1.9/autocar/print_po.py`

 * *Files identical despite different names*

### Comparing `autocar-0.1.8/autocar/qad_keyboard_automation.py` & `autocar-0.1.9/autocar/qad_keyboard_automation.py`

 * *Files identical despite different names*

### Comparing `autocar-0.1.8/autocar/update_standard_pricelist.py` & `autocar-0.1.9/autocar/update_standard_pricelist.py`

 * *Files identical despite different names*

### Comparing `autocar-0.1.8/autocar/voucher_maintenance.py` & `autocar-0.1.9/autocar/voucher_maintenance.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,16 @@
         'Sub-Acct_1',
         'CC_1',
         'Project_1',
         'Enty_1',
         'Amount_1',
     ])
 
+    df_vouch_export['Date'] = df_vouch_export['Date'].dt.strftime('%m/%d/%y')
+
     dttime_now = datetime.datetime.now()
     file_date = dttime_now.strftime('%m%d%y%H%M')
     supplier_nr = str(df_vouch_export['Supplier'].iloc[0])
     file_name_csv = 'vouch-' + user_name + '-' + file_date + '-' + supplier_nr + '.csv'
     file_name_excel = 'vouch-' + user_name + '-' + file_date + '-' + supplier_nr + '.xlsx'
 
     msgbox_return = xl_app.alert('Are you ready to continue?', title='Ready', mode='info', buttons='yes_no')
@@ -85,11 +87,13 @@
 if __name__ == "__main__":
     # To debug:
     # ------------------------------------------------------------------
     # xw.Book('Voucher Maintenance.xlsb').set_mock_caller()
     # wb: xw.Book = xw.Book.caller()
     # ws_voucher_maint: xw.Sheet = wb.sheets['Voucher Maintenance']
     # ws_settings: xw.Sheet = wb.sheets['Settings']
+    # ws_summary: xw.Sheet = wb.sheets['Summary']
     # vouch_import_path = Path(ws_settings['c_vouch_import'].value)
     # shortpay_path = Path(ws_settings['c_shortpay_req'].value)
+    # vouch_maint_path = Path(ws_settings['c_vouchMaint'].value)
     # ------------------------------------------------------------------
     button_export()
```

### Comparing `autocar-0.1.8/pyproject.toml` & `autocar-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autocar-0.1.8/PKG-INFO` & `autocar-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocar
-Version: 0.1.8
+Version: 0.1.9
 Summary: autocar
 Author-email: Jean Henstock <63672596+jjhenstock@users.noreply.github.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: extract-msg
 Requires-Dist: keyboard
 Requires-Dist: numpy
```

