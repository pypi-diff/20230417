# Comparing `tmp/pep508_rs-0.1.1.tar.gz` & `tmp/pep508_rs-0.1.5.tar.gz`

## Comparing `pep508_rs-0.1.1.tar` & `pep508_rs-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,10 @@
--rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 pep508_rs-0.1.1/Cargo.toml
--rw-r--r--   0      501       20     4558 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/.github/workflows/release.yml
--rw-r--r--   0      501       20      976 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/.github/workflows/test.yml
--rw-r--r--   0      501       20      115 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/.gitignore
--rw-r--r--   0      501       20     3035 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/README.md
--rw-r--r--   0      501       20     3035 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/Readme.md
--rw-r--r--   0      501       20       10 2023-04-04 17:13:30.000000 pep508_rs-0.1.1/dist/pep508_rs-0.1.1.tar.gz
--rw-r--r--   0      501       20    33906 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/poetry.lock
--rw-r--r--   0      501       20    17837 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/pypi_analysis/bigquery.ipynb
--rw-r--r--   0      501       20     2440 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/pypi_analysis/bigquery_entirety.ipynb
--rw-r--r--   0      501       20     1115 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/pypi_analysis/download.py
--rw-r--r--   0      501       20      664 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/pyproject.toml
--rw-r--r--   0      501       20    44234 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/src/lib.rs
--rw-r--r--   0      501       20    59695 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/src/marker.rs
--rw-r--r--   0      501       20    14606 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/src/modern.rs
--rw-r--r--   0      501       20     2250 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/test/test_pep508.py
--rw-r--r--   0      501       20    17700 2023-04-04 17:13:08.000000 pep508_rs-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     3334 1970-01-01 00:00:00.000000 pep508_rs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1430 1970-01-01 00:00:00.000000 pep508_rs-0.1.5/Cargo.toml
+-rw-r--r--   0      501       20    10173 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/License-Apache
+-rw-r--r--   0      501       20     1293 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/License-BSD
+-rw-r--r--   0      501       20     3039 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/Readme.md
+-rw-r--r--   0      501       20      664 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/pyproject.toml
+-rw-r--r--   0      501       20    44277 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/src/lib.rs
+-rw-r--r--   0      501       20    62829 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/src/marker.rs
+-rw-r--r--   0      501       20    14606 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/src/modern.rs
+-rw-r--r--   0      501       20    16967 2023-04-17 09:59:46.000000 pep508_rs-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 pep508_rs-0.1.5/PKG-INFO
```

### Comparing `pep508_rs-0.1.1/Cargo.toml` & `pep508_rs-0.1.5/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [package]
 name = "pep508_rs"
-version = "0.1.3-beta.1"
+version = "0.1.5"
 description = "A library for python dependency specifiers, better known as PEP 508"
 edition = "2021"
+include = ["/src", "Changelog.md", "License-Apache", "License-BSD", "Readme.md", "pyproject.toml"]
 # Same license as pypa/packaging where the tests are from
 license = "Apache-2.0 OR BSD-2-Clause"
+readme = "Readme.md"
 repository = "https://github.com/konstin/pep508_rs"
 
-# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
-
 [dependencies]
 anyhow = { version = "1.0.69", optional = true }
 once_cell = "1.17.1"
 pep440_rs = "0.3.1"
 pyo3 = { version = "0.18.2", optional = true, features = ["abi3", "extension-module"] }
 pyo3-log = { version = "0.8.0", optional = true }
 regex = { version = "1.7.1", default-features = false, features = ["std"] }
```

### Comparing `pep508_rs-0.1.1/README.md` & `pep508_rs-0.1.5/Readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Dependency specifiers (PEP 508) in Rust
 
-[![Crates.io](https://img.shields.io/crates/v/pep508_rs.svg?logo=rust&style=flat-square)](https://crates.io/crates/maturin)
-[![PyPI](https://img.shields.io/pypi/v/pep508_rs.svg?logo=python&style=flat-square)](https://pypi.org/project/maturin)
+[![Crates.io](https://img.shields.io/crates/v/pep508_rs.svg?logo=rust&style=flat-square)](https://crates.io/crates/pep508_rs)
+[![PyPI](https://img.shields.io/pypi/v/pep508_rs.svg?logo=python&style=flat-square)](https://pypi.org/project/pep508_rs)
 
 A library for python [dependency specifiers](https://packaging.python.org/en/latest/specifications/dependency-specifiers/), better known as [PEP 508](https://peps.python.org/pep-0508/).
 
 ## Usage
 
 **In Rust**
```

### Comparing `pep508_rs-0.1.1/Readme.md` & `pep508_rs-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,19 @@
+Metadata-Version: 2.1
+Name: pep508_rs
+Version: 0.1.5
+Summary: A library for python dependency specifiers, better known as PEP 508
+License: Apache-2.0 OR BSD-2-Clause
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/konstin/pep508_rs
+
 # Dependency specifiers (PEP 508) in Rust
 
-[![Crates.io](https://img.shields.io/crates/v/pep508_rs.svg?logo=rust&style=flat-square)](https://crates.io/crates/maturin)
-[![PyPI](https://img.shields.io/pypi/v/pep508_rs.svg?logo=python&style=flat-square)](https://pypi.org/project/maturin)
+[![Crates.io](https://img.shields.io/crates/v/pep508_rs.svg?logo=rust&style=flat-square)](https://crates.io/crates/pep508_rs)
+[![PyPI](https://img.shields.io/pypi/v/pep508_rs.svg?logo=python&style=flat-square)](https://pypi.org/project/pep508_rs)
 
 A library for python [dependency specifiers](https://packaging.python.org/en/latest/specifications/dependency-specifiers/), better known as [PEP 508](https://peps.python.org/pep-0508/).
 
 ## Usage
 
 **In Rust**
 
@@ -62,7 +70,8 @@
 
 env = MarkerEnvironment.current()
 Requirement("numpy; python_version >= '3.9.'").evaluate_markers(env, [])
 # This will log: 
 # "Expected PEP 440 version to compare with python_version, found '3.9.', "
 # "evaluating to false: Version `3.9.` doesn't match PEP 440 rules"
 ```
+
```

### Comparing `pep508_rs-0.1.1/pyproject.toml` & `pep508_rs-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pep508_rs"
-version = "0.1.1"
+version = "0.1.5"
 description = "A library for python dependency specifiers, better known as PEP 508"
 readme = "Readme.md"
 
 [tool.poetry]
 name = "pep508_rs"
 version = "0.1.1"
 description = ""
```

### Comparing `pep508_rs-0.1.1/src/lib.rs` & `pep508_rs-0.1.5/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 #![deny(missing_docs)]
 
 mod marker;
 #[cfg(feature = "modern")]
 pub mod modern;
 
 pub use marker::{
-    MarkerEnvironment, MarkerExpression, MarkerOperator, MarkerTree, MarkerValue, MarkerWarningKind,
+    MarkerEnvironment, MarkerExpression, MarkerOperator, MarkerTree, MarkerValue,
+    MarkerValueString, MarkerValueVersion, MarkerWarningKind,
 };
 #[cfg(feature = "pyo3")]
 use pep440_rs::PyVersion;
 use pep440_rs::{Version, VersionSpecifier, VersionSpecifiers};
 #[cfg(feature = "pyo3")]
 use pyo3::{
     basic::CompareOp, create_exception, exceptions::PyNotImplementedError, pyclass, pymethods,
```

### Comparing `pep508_rs-0.1.1/src/marker.rs` & `pep508_rs-0.1.5/src/marker.rs`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 use std::collections::HashSet;
 use std::fmt::{Display, Formatter};
 use std::str::FromStr;
 use tracing::warn;
 
 /// Ways in which marker evaluation can fail
 #[cfg_attr(feature = "pyo3", pyclass(module = "pep508"))]
-#[derive(Debug, Eq, Ord, PartialOrd, PartialEq, Clone, Copy)]
+#[derive(Debug, Eq, Hash, Ord, PartialOrd, PartialEq, Clone, Copy)]
 pub enum MarkerWarningKind {
     /// Using an old name from PEP 345 instead of the modern equivalent
     /// <https://peps.python.org/pep-0345/#environment-markers>
     DeprecatedMarkerName,
     /// Doing an operation other than `==` and `!=` on a quoted string with `extra`, such as
     /// `extra > "perf"` or `extra == os_name`
     ExtraInvalidComparison,
@@ -589,15 +589,15 @@
                     MarkerValue::QuotedString(r_value_string) => r_value_string,
                 };
                 self.marker_compare(r_value_string, extras, reporter)
             }
             // This is either MarkerEnvVersion, MarkerEnvString or Extra inverted
             MarkerValue::QuotedString(l_string) => {
                 match &self.r_value {
-                    // The only sound choice for this is `<version key> <version op> <quoted PEP 440 version>`
+                    // The only sound choice for this is `<quoted PEP 440 version> <version op>` <version key>
                     MarkerValue::MarkerEnvVersion(r_key) => {
                         let l_version = match Version::from_str(l_string) {
                             Ok(l_version) => l_version,
                             Err(err) => {
                                 reporter(MarkerWarningKind::Pep440Error, format!(
                                     "Expected double quoted PEP 440 version to compare with {}, found {}, evaluating to false: {}",
                                     l_string, self.r_value, err
@@ -826,14 +826,36 @@
                 reporter(MarkerWarningKind::ExtraInvalidComparison, "Comparing extra with something other than equal (`==`) or unequal (`!=`) is wrong, evaluating to false".to_string(), self);
                 false
             }
         }
     }
 }
 
+impl FromStr for MarkerExpression {
+    type Err = Pep508Error;
+
+    fn from_str(s: &str) -> Result<Self, Self::Err> {
+        let mut chars = CharIter::new(s);
+        let expression = parse_marker_key_op_value(&mut chars)?;
+        chars.eat_whitespace();
+        if let Some((pos, unexpected)) = chars.next() {
+            return Err(Pep508Error {
+                message: Pep508ErrorSource::String(format!(
+                    "Unexpected character '{}', expected end of input",
+                    unexpected
+                )),
+                start: pos,
+                len: chars.chars.clone().count(),
+                input: chars.copy_chars(),
+            });
+        }
+        Ok(expression)
+    }
+}
+
 impl Display for MarkerExpression {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{} {} {}", self.l_value, self.operator, self.r_value)
     }
 }
 
 /// Represents one of the nested marker expressions with and/or/parentheses
@@ -1137,43 +1159,43 @@
         }
     }
 }
 
 /// ```text
 /// marker_var:l marker_op:o marker_var:r
 /// ```
-fn parse_marker_key_op_value(chars: &mut CharIter) -> Result<MarkerTree, Pep508Error> {
+fn parse_marker_key_op_value(chars: &mut CharIter) -> Result<MarkerExpression, Pep508Error> {
     chars.eat_whitespace();
     let lvalue = parse_marker_value(chars)?;
     chars.eat_whitespace();
     // "not in" and "in" must be preceded by whitespace. We must already have matched a whitespace
     // when we're here because other `parse_marker_key` would have pulled the characters in and
     // errored
     let operator = parse_marker_operator(chars)?;
     chars.eat_whitespace();
     let rvalue = parse_marker_value(chars)?;
-    Ok(MarkerTree::Expression(MarkerExpression {
+    Ok(MarkerExpression {
         l_value: lvalue,
         operator,
         r_value: rvalue,
-    }))
+    })
 }
 
 /// ```text
 /// marker_expr   = marker_var:l marker_op:o marker_var:r -> (o, l, r)
 ///               | wsp* '(' marker:m wsp* ')' -> m
 /// ```
 fn parse_marker_expr(chars: &mut CharIter) -> Result<MarkerTree, Pep508Error> {
     chars.eat_whitespace();
     if let Some(start_pos) = chars.eat('(') {
         let marker = parse_marker_or(chars)?;
         chars.next_expect_char(')', start_pos)?;
         Ok(marker)
     } else {
-        parse_marker_key_op_value(chars)
+        Ok(MarkerTree::Expression(parse_marker_key_op_value(chars)?))
     }
 }
 
 /// ```text
 /// marker_and    = marker_expr:l wsp* 'and' marker_expr:r -> ('and', l, r)
 ///               | marker_expr:m -> m
 /// ```
@@ -1230,31 +1252,52 @@
     }
 }
 
 /// ```text
 /// marker        = marker_or
 /// ```
 pub(crate) fn parse_markers_impl(chars: &mut CharIter) -> Result<MarkerTree, Pep508Error> {
-    parse_marker_or(chars)
+    let marker = parse_marker_or(chars)?;
+    chars.eat_whitespace();
+    if let Some((pos, unexpected)) = chars.next() {
+        // If we're here, both parse_marker_or and parse_marker_and returned because the next
+        // character was neither "and" nor "or"
+        return Err(Pep508Error {
+            message: Pep508ErrorSource::String(format!(
+                "Unexpected character '{}', expected 'and', 'or' or end of input",
+                unexpected
+            )),
+            start: pos,
+            len: chars.chars.clone().count(),
+            input: chars.copy_chars(),
+        });
+    };
+    Ok(marker)
 }
 
 /// Parses markers such as `python_version < '3.8'` or
 /// `python_version == "3.10" and (sys_platform == "win32" or (os_name == "linux" and implementation_name == 'cpython'))`
 fn parse_markers(markers: &str) -> Result<MarkerTree, Pep508Error> {
-    parse_markers_impl(&mut CharIter::new(markers))
+    let mut chars = CharIter::new(markers);
+    parse_markers_impl(&mut chars)
 }
 
 #[cfg(test)]
 mod test {
     use crate::marker::MarkerEnvironment;
-    use crate::MarkerTree;
+    use crate::{MarkerExpression, MarkerOperator, MarkerTree, MarkerValue, MarkerValueString};
+    use indoc::indoc;
     use log::Level;
     use pep440_rs::Version;
     use std::str::FromStr;
 
+    fn assert_err(input: &str, error: &str) {
+        assert_eq!(MarkerTree::from_str(input).unwrap_err().to_string(), error);
+    }
+
     fn env37() -> MarkerEnvironment {
         let v37 = Version::from_str("3.7").unwrap();
 
         MarkerEnvironment {
             implementation_name: "".to_string(),
             implementation_version: ("3.7".to_string(), v37.clone()),
             os_name: "linux".to_string(),
@@ -1421,8 +1464,54 @@
         assert!(result);
     }
 
     #[test]
     fn test_closing_parentheses() {
         MarkerTree::from_str(r#"( "linux" in sys_platform) and extra == 'all'"#).unwrap();
     }
+
+    #[test]
+    fn wrong_quotes_dot_star() {
+        assert_err(
+            r#"python_version == "3.8".* and python_version >= "3.8""#,
+            indoc! {r#"
+                Unexpected character '.', expected 'and', 'or' or end of input
+                python_version == "3.8".* and python_version >= "3.8"
+                                       ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^"#
+            },
+        );
+        assert_err(
+            r#"python_version == "3.8".*"#,
+            indoc! {r#"
+                Unexpected character '.', expected 'and', 'or' or end of input
+                python_version == "3.8".*
+                                       ^"#
+            },
+        );
+    }
+
+    #[test]
+    fn test_marker_expression() {
+        assert_eq!(
+            MarkerExpression::from_str(r#"os_name == "nt""#).unwrap(),
+            MarkerExpression {
+                l_value: MarkerValue::MarkerEnvString(MarkerValueString::OsName),
+                operator: MarkerOperator::Equal,
+                r_value: MarkerValue::QuotedString("nt".to_string()),
+            }
+        );
+    }
+
+    #[test]
+    fn test_marker_expression_to_long() {
+        assert_eq!(
+            MarkerExpression::from_str(r#"os_name == "nt" and python_version >= "3.8""#)
+                .unwrap_err()
+                .to_string(),
+            indoc! {r#"
+                Unexpected character 'a', expected end of input
+                os_name == "nt" and python_version >= "3.8"
+                                ^^^^^^^^^^^^^^^^^^^^^^^^^^"#
+            },
+        );
+    }
 }
```

### Comparing `pep508_rs-0.1.1/src/modern.rs` & `pep508_rs-0.1.5/src/modern.rs`

 * *Files identical despite different names*

### Comparing `pep508_rs-0.1.1/Cargo.lock` & `pep508_rs-0.1.5/Cargo.lock`

 * *Files 5% similar despite different names*

```diff
@@ -38,44 +38,23 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
-name = "ctor"
-version = "0.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd4056f63fce3b82d852c3da92b08ea59959890813a7f4ce9c0ff85b10cf301b"
-dependencies = [
- "quote",
- "syn 2.0.13",
-]
-
-[[package]]
 name = "form_urlencoded"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
-name = "ghost"
-version = "0.1.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.13",
-]
-
-[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "idna"
@@ -106,24 +85,14 @@
 [[package]]
 name = "indoc"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f2cb48b81b1dc9f39676bf99f5499babfec7cd8fe14307f7b3d747208fb5690"
 
 [[package]]
-name = "inventory"
-version = "0.3.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7741301a6d6a9b28ce77c0fb77a4eb116b6bc8f3bef09923f7743d059c4157d3"
-dependencies = [
- "ctor",
- "ghost",
-]
-
-[[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "lazy_static"
@@ -198,29 +167,29 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "pep440_rs"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da289d74d9a9bceb0b22695f40da57a6489969f9d8790b52f823767a2c8ade"
+checksum = "aac177a025c60a4dd25d638bf33e746d1ead5f7123f6650f35b4394c7ce1a104"
 dependencies = [
  "lazy_static",
  "pyo3",
  "regex",
  "serde",
  "tracing",
  "unicode-width",
 ]
 
 [[package]]
 name = "pep508_rs"
-version = "0.1.3-beta.1"
+version = "0.1.5"
 dependencies = [
  "anyhow",
  "indoc 2.0.1",
  "log",
  "once_cell",
  "pep440_rs",
  "pyo3",
@@ -255,45 +224,44 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc 1.0.9",
- "inventory",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
@@ -304,29 +272,29 @@
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -374,37 +342,37 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -431,17 +399,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.13"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -472,15 +440,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
```

