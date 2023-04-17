# Comparing `tmp/OpenGeode_Geosciences-7.0.1-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_Geosciences-7.0.2-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 4264 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       98 b- defN 23-Apr-14 13:30 opengeode_geosciences/__init__.py
--rw-rw-rw-  2.0 fat     1239 b- defN 23-Apr-14 13:30 opengeode_geosciences/explicit.py
--rw-rw-rw-  2.0 fat     1239 b- defN 23-Apr-14 13:30 opengeode_geosciences/implicit.py
--rw-rw-rw-  2.0 fat     3232 b- defN 23-Apr-14 13:33 OpenGeode_Geosciences-7.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-14 13:33 OpenGeode_Geosciences-7.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-14 13:33 OpenGeode_Geosciences-7.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      623 b- defN 23-Apr-14 13:33 OpenGeode_Geosciences-7.0.1.dist-info/RECORD
-7 files, 6553 bytes uncompressed, 3144 bytes compressed:  52.0%
+Zip file size: 819460 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       94 b- defN 23-Apr-17 12:26 opengeode_geosciences/__init__.py
+-rw-r--r--  2.0 unx     1216 b- defN 23-Apr-17 12:26 opengeode_geosciences/explicit.py
+-rw-r--r--  2.0 unx     1216 b- defN 23-Apr-17 12:26 opengeode_geosciences/implicit.py
+-rwxr-xr-x  2.0 unx  1883784 b- defN 23-Apr-17 12:27 opengeode_geosciences/lib64/libOpenGeode-Geosciences_explicit.so
+-rwxr-xr-x  2.0 unx   846632 b- defN 23-Apr-17 12:27 opengeode_geosciences/lib64/libOpenGeode-Geosciences_implicit.so
+-rwxr-xr-x  2.0 unx   483904 b- defN 23-Apr-17 12:27 opengeode_geosciences/lib64/opengeode_geosciences_py_explicit.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   475376 b- defN 23-Apr-17 12:27 opengeode_geosciences/lib64/opengeode_geosciences_py_implicit.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     3137 b- defN 23-Apr-17 12:27 OpenGeode_Geosciences-7.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-17 12:27 OpenGeode_Geosciences-7.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-17 12:27 OpenGeode_Geosciences-7.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1172 b- defN 23-Apr-17 12:27 OpenGeode_Geosciences-7.0.2.dist-info/RECORD
+11 files, 3696656 bytes uncompressed, 817412 bytes compressed:  77.9%
```

## zipnote {}

```diff
@@ -3,20 +3,32 @@
 
 Filename: opengeode_geosciences/explicit.py
 Comment: 
 
 Filename: opengeode_geosciences/implicit.py
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.0.1.dist-info/METADATA
+Filename: opengeode_geosciences/lib64/libOpenGeode-Geosciences_explicit.so
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.0.1.dist-info/WHEEL
+Filename: opengeode_geosciences/lib64/libOpenGeode-Geosciences_implicit.so
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.0.1.dist-info/top_level.txt
+Filename: opengeode_geosciences/lib64/opengeode_geosciences_py_explicit.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.0.1.dist-info/RECORD
+Filename: opengeode_geosciences/lib64/opengeode_geosciences_py_implicit.cpython-39-x86_64-linux-gnu.so
+Comment: 
+
+Filename: OpenGeode_Geosciences-7.0.2.dist-info/METADATA
+Comment: 
+
+Filename: OpenGeode_Geosciences-7.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: OpenGeode_Geosciences-7.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: OpenGeode_Geosciences-7.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_geosciences/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-from .explicit import *
-from .implicit import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .explicit import *
+from .implicit import *
```

## opengeode_geosciences/explicit.py

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2019 - 2023 Geode-solutions
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-import opengeode
-
-from .bin.opengeode_geosciences_py_explicit import *
-
-GeosciencesExplicitLibrary.initialize()
+# Copyright (c) 2019 - 2023 Geode-solutions
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import opengeode
+
+from .lib64.opengeode_geosciences_py_explicit import *
+
+GeosciencesExplicitLibrary.initialize()
```

## opengeode_geosciences/implicit.py

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2019 - 2023 Geode-solutions
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-import opengeode
-
-from .bin.opengeode_geosciences_py_implicit import *
-
-GeosciencesImplicitLibrary.initialize()
+# Copyright (c) 2019 - 2023 Geode-solutions
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import opengeode
+
+from .lib64.opengeode_geosciences_py_implicit import *
+
+GeosciencesImplicitLibrary.initialize()
```

## Comparing `OpenGeode_Geosciences-7.0.1.dist-info/METADATA` & `OpenGeode_Geosciences-7.0.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,72 @@
-Metadata-Version: 2.1
-Name: OpenGeode-Geosciences
-Version: 7.0.1
-Summary: OpenGeode module for Geosciences
-Home-page: https://github.com/Geode-solutions/OpenGeode-Geosciences
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.0.0)
-
-<h1 align="center">OpenGeode-Geosciences<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">OpenGeode module for Geosciences</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/OpenGeode-Geosciences/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/OpenGeode-Geosciences.svg" alt="Version">
-  <img src="https://img.shields.io/pypi/v/opengeode-geosciences" alt="PyPI" >
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://opengeode-slack-invite.herokuapp.com">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-  <a href="https://doi.org/10.5281/zenodo.3610370">
-    <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3610370.svg" alt="DOI">
-  </a>
-</p>
-
----
-
-## Introduction
-
-OpenGeode-Geosciences is a module of [OpenGeode] provides data structures for geological models and geological objects.
-
-[OpenGeode]: https://github.com/Geode-solutions/OpenGeode
-
-
-## Documentation
-
-To check out our live documentation, visit [docs.geode-solutions.com](https://docs.geode-solutions.com).
-
-Installing OpenGeode-Geosciences is done:
- * either, by compiling the C++ source.
- * or, by using pip command ```pip install OpenGeode-Geosciences``` and add ```import opengeode_geosciences``` in your Python script.
-
-
-## Questions
-For questions and support please use the official [slack](https://opengeode-slack-invite.herokuapp.com) and go to the channel #geosciences. The issue list of this repo is exclusively for bug reports and feature requests. 
-
-
-## Changelog
-
-Detailed changes for each release are documented in the [release notes](https://github.com/Geode-solutions/OpenGeode-Geosciences/releases).
-
-
-## License
-
-[MIT](https://opensource.org/licenses/MIT)
-
-Copyright (c) 2019 - 2023, Geode-solutions
-
-
+Metadata-Version: 2.1
+Name: OpenGeode-Geosciences
+Version: 7.0.2
+Summary: OpenGeode module for Geosciences
+Home-page: https://github.com/Geode-solutions/OpenGeode-Geosciences
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: MIT
+Description-Content-Type: text/markdown
+Requires-Dist: opengeode-core (==14.*,>=14.0.0)
+
+<h1 align="center">OpenGeode-Geosciences<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">OpenGeode module for Geosciences</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/OpenGeode-Geosciences/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/OpenGeode-Geosciences.svg" alt="Version">
+  <img src="https://img.shields.io/pypi/v/opengeode-geosciences" alt="PyPI" >
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://opengeode-slack-invite.herokuapp.com">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+  <a href="https://doi.org/10.5281/zenodo.3610370">
+    <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3610370.svg" alt="DOI">
+  </a>
+</p>
+
+---
+
+## Introduction
+
+OpenGeode-Geosciences is a module of [OpenGeode] provides data structures for geological models and geological objects.
+
+[OpenGeode]: https://github.com/Geode-solutions/OpenGeode
+
+
+## Documentation
+
+To check out our live documentation, visit [docs.geode-solutions.com](https://docs.geode-solutions.com).
+
+Installing OpenGeode-Geosciences is done:
+ * either, by compiling the C++ source.
+ * or, by using pip command ```pip install OpenGeode-Geosciences``` and add ```import opengeode_geosciences``` in your Python script.
+
+
+## Questions
+For questions and support please use the official [slack](https://opengeode-slack-invite.herokuapp.com) and go to the channel #geosciences. The issue list of this repo is exclusively for bug reports and feature requests. 
+
+
+## Changelog
+
+Detailed changes for each release are documented in the [release notes](https://github.com/Geode-solutions/OpenGeode-Geosciences/releases).
+
+
+## License
+
+[MIT](https://opensource.org/licenses/MIT)
+
+Copyright (c) 2019 - 2023, Geode-solutions
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 7.0.1 Summary:
+Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 7.0.2 Summary:
 OpenGeode module for Geosciences Home-page: https://github.com/Geode-solutions/
 OpenGeode-Geosciences Author: Geode-solutions Author-email: contact@geode-
-solutions.com License: MIT Platform: UNKNOWN Description-Content-Type: text/
-markdown Requires-Dist: opengeode-core (==14.*,>=14.0.0)
+solutions.com License: MIT Description-Content-Type: text/markdown Requires-
+Dist: opengeode-core (==14.*,>=14.0.0)
              ****** OpenGeode-Geosciencesby Geode-solutions ******
                   **** OpenGeode module for Geosciences ****
        [Build Status] [Deploy Status] [Coverage Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
          [Language] [License] [Semantic-release] [Slack_invite] [DOI]
 --- ## Introduction OpenGeode-Geosciences is a module of [OpenGeode] provides
 data structures for geological models and geological objects. [OpenGeode]:
```

