# Comparing `tmp/whoisdomain-1.20230417.2.tar.gz` & `tmp/whoisdomain-1.20230417.5.tar.gz`

## Comparing `whoisdomain-1.20230417.2.tar` & `whoisdomain-1.20230417.5.tar`

### file list

```diff
@@ -1,196 +1,196 @@
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Historical.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/MANIFEST.in
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/license
--rwxr-xr-x   0        0        0     1052 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/pypi-test.sh
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/pypi.sh
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/pyproject.toml-template
--rwxr-xr-x   0        0        0    15950 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/test2.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   190007 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    55638 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    19473 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    21664 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    62946 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1146965 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   126768 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   115786 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0   147473 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0    95073 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0   136157 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    23854 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    88645 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    92150 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    47582 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    37124 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    80882 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   151599 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    29543 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    52507 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   175017 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   150518 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    46067 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   254545 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   446688 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    54794 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    92867 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   390721 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   135868 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25468 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    62332 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    32673 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    73584 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    68120 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    95559 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12461 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16666 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    15557 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   369261 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json
--rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_1_query.data.json
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_1_query.meta.json
--rw-r--r--   0        0        0    14086 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_2_parse.data.json
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json
--rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json
--rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/__init__.data.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/__init__.meta.json
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/exceptions.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/exceptions.meta.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/DONE
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/TODO
--rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/analize_patterns.py
--rwxr-xr-x   0        0        0     2623 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/compare_known_tld.py
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/convert_to_dict.sh
--rwxr-xr-x   0        0        0     6984 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/makeTestdataAll.sh
--rwxr-xr-x   0        0        0     8753 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/test.py
--rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/test.sh
--rwxr-xr-x   0        0        0    11070 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/test3.py
--rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/testExtend.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/bin/find_input_no_output.sh
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/tests/failed-parsing.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/tests/invalid-tld.txt
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/tests/new-test.txt
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/tests/ok-domains.txt
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/tests/private-reg.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/Old/tests/unknown-dateformat.txt
--rwxr-xr-x   0        0        0     1796 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/make_testdata.sh
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/example.com/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/example.com/nameservers
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/example.com/output
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/example.net/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/example.net/nameservers
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/example.net/output
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/example.org/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/example.org/nameservers
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/example.org/output
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/google.com/input
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/google.com/nameservers
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/google.com/output
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/hello.xyz/input
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/hello.xyz/nameservers
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/hello.xyz/output
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.co.jp/input
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.co.jp/nameservers
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.co.jp/output
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.co.uk/input
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.co.uk/nameservers
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.co.uk/output
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.com/input
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.com/nameservers
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.com/output
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.com.sg/input
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.com.sg/nameservers
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.com.sg/output
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.com.tr/input
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.com.tr/nameservers
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.com.tr/output
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.jp/input
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.jp/nameservers
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.jp/output
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.kr/input
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.kr/nameservers
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/meta.kr/output
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/xs4all.nl/input
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/xs4all.nl/nameservers
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/testdata/xs4all.nl/output
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/whoisdomain/_0_init_tld.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/whoisdomain/_1_query.py
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/whoisdomain/_2_parse.py
--rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/whoisdomain/_3_adjust.py
--rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/whoisdomain/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/whoisdomain/exceptions.py
--rw-r--r--   0        0        0   104536 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/whoisdomain/tld_regexpr.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.gitignore
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/.hgignore
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/README.md
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/pyproject.toml
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.2/PKG-INFO
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Historical.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/MANIFEST.in
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/license
+-rwxr-xr-x   0        0        0     1341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/pypi-test.sh
+-rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/pypi.sh
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/pyproject.toml-template
+-rwxr-xr-x   0        0        0    15950 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/test2.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   190007 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    55638 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    19473 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    21664 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    62946 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1146965 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   126768 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   115786 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0   147473 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0    95073 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0   136157 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    23854 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0    88645 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    92150 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    47582 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    37124 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    80882 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   151599 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    29543 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    52507 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   175017 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   150518 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    46067 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   254545 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   446688 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    54794 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    92867 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   390721 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   135868 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25468 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    62332 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    32673 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    73584 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    68120 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    95559 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12461 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    16666 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    15557 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   369261 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json
+-rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_1_query.data.json
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_1_query.meta.json
+-rw-r--r--   0        0        0    14086 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_2_parse.data.json
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json
+-rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json
+-rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/__init__.data.json
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/__init__.meta.json
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/exceptions.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/exceptions.meta.json
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/DONE
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/TODO
+-rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/analize_patterns.py
+-rwxr-xr-x   0        0        0     2623 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/compare_known_tld.py
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/convert_to_dict.sh
+-rwxr-xr-x   0        0        0     6984 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/makeTestdataAll.sh
+-rwxr-xr-x   0        0        0     8753 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/test.py
+-rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/test.sh
+-rwxr-xr-x   0        0        0    11070 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/test3.py
+-rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/testExtend.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/bin/find_input_no_output.sh
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/failed-parsing.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/invalid-tld.txt
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/new-test.txt
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/ok-domains.txt
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/private-reg.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/unknown-dateformat.txt
+-rwxr-xr-x   0        0        0     1796 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/make_testdata.sh
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.com/input
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.com/nameservers
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.com/output
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.net/input
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.net/nameservers
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.net/output
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.org/input
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.org/nameservers
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.org/output
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/google.com/input
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/google.com/nameservers
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/google.com/output
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/hello.xyz/input
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/hello.xyz/nameservers
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/hello.xyz/output
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.jp/input
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.jp/nameservers
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.jp/output
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.uk/input
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.uk/nameservers
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.uk/output
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com/input
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com/nameservers
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com/output
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.sg/input
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.sg/nameservers
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.sg/output
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.tr/input
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.tr/nameservers
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.tr/output
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.jp/input
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.jp/nameservers
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.jp/output
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.kr/input
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.kr/nameservers
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.kr/output
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/xs4all.nl/input
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/xs4all.nl/nameservers
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/xs4all.nl/output
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/_0_init_tld.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/_1_query.py
+-rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/_2_parse.py
+-rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/_3_adjust.py
+-rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/exceptions.py
+-rw-r--r--   0        0        0   104536 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/tld_regexpr.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.gitignore
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.hgignore
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/README.md
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/pyproject.toml
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/PKG-INFO
```

### Comparing `whoisdomain-1.20230417.2/Historical.txt` & `whoisdomain-1.20230417.5/Historical.txt`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/pypi-test.sh` & `whoisdomain-1.20230417.5/pypi-test.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-#! /usr/bin/env bash
+#! /bin/bash
+
 DATE=$( date +%Y%m%d )
 
 setupVersionNumberToday()
 {
-    VERSION="1"
+    VERSION="1" # we start with version 1, only breaking changes will increment the first digit
+
+    # while preparing the test.pypi we increment the day sequence if needed,
+    # only a last version actually later will get published to the actual pypi (non test)
 
     TODAY_SEQ=$(
         ls dist/*${DATE}*.whl 2>/dev/null |
         awk -F\- '{ print $2 }' |
-        awk -F\. '{ print $3 }'
+        awk -F\. '{ print $3 }' |
+        awk '{ if ($1 > a) { a = $1 }} END { print a }'
     )
 
     if [ -z "${TODAY_SEQ}" ]
     then
         TODAY_SEQ="1"
     else
         TODAY_SEQ=$(( TODAY_SEQ + 1))
     fi
 
-    echo "version=${VERSION} date=${DATE} seq=${TODAY_SEQ}"
+    # keep track of the latest version string
+    echo "${VERSION}.${DATE}.${TODAY_SEQ}" >./work/version
 }
 
 makeTomlFile()
 {
     cat pyproject.toml-template |
     awk -vversion="${VERSION}" -vdate="${DATE}" -vseq="${TODAY_SEQ}" '
     /@VERSION@/  { sub(/@VERSION@/,version) }
@@ -42,15 +48,15 @@
 {
     twine upload -r testpypi dist/*"${VERSION}.${DATE}.${TODAY_SEQ}"*
 }
 
 main()
 {
     ./reformat-code.sh
-    mypy --implicit-optional --install-types --non-interactive --namespace-packages whoisdomain
+    mypy --implicit-optional whoisdomain
 
     setupVersionNumberToday
     makeTomlFile
     buildDist
     uploadTwineTest
 }
```

### Comparing `whoisdomain-1.20230417.2/pyproject.toml-template` & `whoisdomain-1.20230417.5/pyproject.toml-template`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/test2.py` & `whoisdomain-1.20230417.5/test2.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.github/ISSUE_TEMPLATE/bug_report.md` & `whoisdomain-1.20230417.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.github/workflows/lint.yml` & `whoisdomain-1.20230417.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.github/workflows/python-publish.yml` & `whoisdomain-1.20230417.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/_ast.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/_ast.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/_ast.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1,
         1,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/_codecs.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/_codecs.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/_codecs.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         4,
         1,
         2,
         3,
         5,
         6,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/_collections_abc.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/_collections_abc.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         32,
         1,
         1
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/_ctypes.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/_ctypes.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1,
         1,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/abc.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/abc.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/abc.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         1
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/array.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/array.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/array.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         3,
         1,
         2,
         6,
         7,
         1,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/builtins.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/builtins.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/builtins.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         30,
         1,
         2,
         3,
         4,
         5,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/codecs.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/codecs.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/codecs.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         5,
         1,
         2,
         3,
         4,
         6,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/contextlib.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/contextlib.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/contextlib.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9555555555555555%*

 * *Differences: {"'data_mtime'": '1681721902',*

 * * "'dep_lines'": '{delete: [7]}',*

 * * "'dep_prios'": '{delete: [8]}',*

 * * "'dependencies'": '{delete: [8]}'}*

```diff
@@ -1,41 +1,38 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         5,
         1,
         2,
         3,
         6,
         7,
         8,
-        1,
         1
     ],
     "dep_prios": [
         5,
         5,
         10,
         5,
         5,
         5,
         5,
-        5,
-        30
+        5
     ],
     "dependencies": [
         "collections.abc",
         "abc",
         "sys",
         "_typeshed",
         "types",
         "typing",
         "typing_extensions",
-        "builtins",
-        "os"
+        "builtins"
     ],
     "hash": "48bd9c84f4093e39fcb915605fadeae2429be6aabd9f355f9f72a7690dc6ac5f",
     "id": "contextlib",
     "ignore_all": true,
     "interface_hash": "5904cd9eeb9e37e86b43a16512510d8944642aa6774cf55c704437c00acf1d19",
     "mtime": 1676537402,
     "options": {
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/datetime.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/datetime.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/datetime.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         4,
         5,
         6,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/enum.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/enum.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/enum.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         6,
         1,
         2,
         3,
         4,
         5,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/functools.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/functools.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/functools.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         4,
         1,
         2,
         3,
         5,
         6,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/genericpath.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/genericpath.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/genericpath.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         1,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/io.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/io.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/io.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         6,
         1,
         2,
         3,
         4,
         5,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/mmap.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/mmap.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/mmap.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         3,
         1,
         2,
         4,
         1,
         1,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/pathlib.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/pathlib.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/pathlib.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         13,
         1,
         2,
         14,
         15,
         16,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/pickle.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/pickle.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/pickle.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         1,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/platform.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/platform.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/platform.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         7,
         1,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/posixpath.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/posixpath.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/posixpath.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         3,
         1,
         2,
         4,
         17,
         18,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/re.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/re.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/re.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         5,
         1,
         2,
         3,
         4,
         6,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_compile.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_compile.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         4,
         5,
         1,
         1
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_constants.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_constants.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_parse.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/sre_parse.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         2,
         1,
         3,
         4,
         6,
         7,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/subprocess.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/subprocess.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/subprocess.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         6,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/sys.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/sys.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/sys.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         4,
         5,
         6,
         2,
         3,
         7,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/time.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/time.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/time.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         4,
         1,
         1
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/types.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/types.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/types.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         3,
         16,
         1,
         2,
         19,
         20,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/typing.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/typing.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/typing.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         4,
         6,
         7,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/typing_extensions.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/typing_extensions.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         8,
         1,
         2,
         3,
         4,
         5,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/_typeshed/__init__.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         10,
         5,
         6,
         7,
         8,
         9,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/collections/__init__.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/collections/__init__.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         11,
         1,
         2,
         3,
         4,
         5,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/collections/abc.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/collections/abc.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/ctypes/__init__.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/ctypes/__init__.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         5,
         1,
         2,
         3,
         4,
         6,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/__init__.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/__init__.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         4,
         5,
         1,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/charset.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/charset.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/charset.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/contentmanager.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/contentmanager.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/errors.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/errors.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/errors.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         1,
         1,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/header.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/header.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/header.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/message.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/message.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/message.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         2,
         4,
         5,
         6,
         7,
         1,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/policy.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/email/policy.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/policy.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         2,
         3,
         4,
         5,
         6,
         1,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/__init__.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/__init__.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1,
         1
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/abc.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/abc.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         12,
         13,
         1,
         2,
         3,
         11,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/machinery.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/machinery.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         5,
         9,
         1,
         2,
         3,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         30,
         5,
         6,
         7,
         1,
         2,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         1,
         1
     ],
     "dep_prios": [
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/json/__init__.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/json/__init__.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         2,
         5,
         6,
         1,
         3,
         1,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/json/decoder.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/json/decoder.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         1,
         1
     ],
     "dep_prios": [
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/json/encoder.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/json/encoder.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/os/__init__.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/os/__init__.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         23,
         30,
         1,
         2,
         21,
         22,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/os/path.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/os/path.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/os/path.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         7,
         1,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9600000000000001%*

 * *Differences: {"'data_mtime'": '1681721902',*

 * * "'dep_lines'": '{insert: [(5, 1)]}',*

 * * "'dep_prios'": '{insert: [(6, 30)]}',*

 * * "'dependencies'": "{insert: [(14, 'types')]}"}*

```diff
@@ -1,23 +1,24 @@
 {
-    "data_mtime": 1681721013,
+    "data_mtime": 1681721902,
     "dep_lines": [
         10,
         11,
         1,
         2,
         4,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         5,
         10,
         10,
@@ -26,14 +27,15 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
+        30,
         30
     ],
     "dependencies": [
         "whoisdomain.tld_regexpr",
         "whoisdomain.exceptions",
         "re",
         "sys",
@@ -42,15 +44,16 @@
         "_collections_abc",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "enum",
         "mmap",
-        "pickle"
+        "pickle",
+        "types"
     ],
     "hash": "beb0fbfc8849a98adea48266a50473f40e26cc8a6038150caaefe352248dfcba",
     "id": "whoisdomain._0_init_tld",
     "ignore_all": false,
     "interface_hash": "97f7005623fab9ee3542c1d4377173245fe43a98ebb829ffb42c271b9432eb75",
     "mtime": 1681288053,
     "options": {
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_1_query.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_1_query.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_1_query.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_1_query.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721013,
+    "data_mtime": 1681721902,
     "dep_lines": [
         7,
         1,
         2,
         3,
         4,
         5,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_2_parse.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_2_parse.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9604166666666667%*

 * *Differences: {"'data_mtime'": '1681721902',*

 * * "'dep_lines'": '{insert: [(5, 1)]}',*

 * * "'dep_prios'": '{insert: [(6, 30)]}',*

 * * "'dependencies'": "{insert: [(14, 'types')]}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721013,
+    "data_mtime": 1681721902,
     "dep_lines": [
         12,
         14,
         1,
         2,
         4,
         1,
@@ -11,14 +11,15 @@
         1,
         1,
         1,
         1,
         1,
         1,
         1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         5,
         10,
         10,
@@ -28,14 +29,15 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
+        30,
         30
     ],
     "dependencies": [
         "whoisdomain._0_init_tld",
         "whoisdomain.exceptions",
         "re",
         "sys",
@@ -45,14 +47,15 @@
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "enum",
         "mmap",
         "pickle",
+        "types",
         "typing_extensions"
     ],
     "hash": "45e6e9e386cc90dc0b2e1660189f63759bc2038cda06a63637d71f01d3244b0d",
     "id": "whoisdomain._2_parse",
     "ignore_all": false,
     "interface_hash": "e49d2f96d2efa686d2ddb0dfa389f5635aadeae321b3e3ba4797cf02ef5951a7",
     "mtime": 1681288053,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9533333333333334%*

 * *Differences: {"'data_mtime'": '1681721902',*

 * * "'dep_lines'": '{insert: [(5, 1), (6, 1)]}',*

 * * "'dep_prios'": '{insert: [(6, 30), (7, 30)]}',*

 * * "'dependencies'": "{insert: [(10, 'enum'), (13, 'types')]}"}*

```diff
@@ -1,22 +1,24 @@
 {
-    "data_mtime": 1681721013,
+    "data_mtime": 1681721902,
     "dep_lines": [
         4,
         1,
         2,
         3,
         6,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         10,
         10,
         10,
@@ -24,29 +26,33 @@
         5,
         30,
         30,
         30,
         30,
         30,
         30,
+        30,
+        30,
         30
     ],
     "dependencies": [
         "whoisdomain.exceptions",
         "re",
         "sys",
         "datetime",
         "typing",
         "builtins",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
+        "enum",
         "mmap",
         "pickle",
+        "types",
         "typing_extensions"
     ],
     "hash": "5f32028396919758635db05cd5c0936905af566011ef0360deb69de8dc22e006",
     "id": "whoisdomain._3_adjust",
     "ignore_all": false,
     "interface_hash": "0b5adf5388d2b9fcf64d59ec8edd3b69ad3c421c7882289e42454c662e5d9b4d",
     "mtime": 1681288053,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/__init__.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/__init__.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/__init__.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721098,
+    "data_mtime": 1681721902,
     "dep_lines": [
         10,
         11,
         19,
         20,
         28,
         1,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/exceptions.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/exceptions.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/exceptions.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
```

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json` & `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1681721902'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721012,
+    "data_mtime": 1681721902,
     "dep_lines": [
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
```

### Comparing `whoisdomain-1.20230417.2/Old/DONE` & `whoisdomain-1.20230417.5/Old/DONE`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/Old/analize_patterns.py` & `whoisdomain-1.20230417.5/Old/analize_patterns.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/Old/compare_known_tld.py` & `whoisdomain-1.20230417.5/Old/compare_known_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/Old/makeTestdataAll.sh` & `whoisdomain-1.20230417.5/Old/makeTestdataAll.sh`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/Old/test.py` & `whoisdomain-1.20230417.5/Old/test.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/Old/test.sh` & `whoisdomain-1.20230417.5/Old/test.sh`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/Old/test3.py` & `whoisdomain-1.20230417.5/Old/test3.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/Old/testExtend.py` & `whoisdomain-1.20230417.5/Old/testExtend.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/Old/tests/new-test.txt` & `whoisdomain-1.20230417.5/Old/tests/new-test.txt`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/Old/tests/ok-domains.txt` & `whoisdomain-1.20230417.5/Old/tests/ok-domains.txt`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/make_testdata.sh` & `whoisdomain-1.20230417.5/testdata/make_testdata.sh`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/example.com/output` & `whoisdomain-1.20230417.5/testdata/example.com/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/example.net/output` & `whoisdomain-1.20230417.5/testdata/example.net/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/example.org/input` & `whoisdomain-1.20230417.5/testdata/example.org/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/example.org/output` & `whoisdomain-1.20230417.5/testdata/example.org/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/google.com/input` & `whoisdomain-1.20230417.5/testdata/google.com/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/google.com/output` & `whoisdomain-1.20230417.5/testdata/google.com/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/hello.xyz/input` & `whoisdomain-1.20230417.5/testdata/hello.xyz/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/hello.xyz/output` & `whoisdomain-1.20230417.5/testdata/hello.xyz/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.co.jp/input` & `whoisdomain-1.20230417.5/testdata/meta.co.jp/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.co.jp/output` & `whoisdomain-1.20230417.5/testdata/meta.co.jp/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.co.uk/input` & `whoisdomain-1.20230417.5/testdata/meta.co.uk/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.co.uk/output` & `whoisdomain-1.20230417.5/testdata/meta.co.uk/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.com/input` & `whoisdomain-1.20230417.5/testdata/meta.com/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.com/output` & `whoisdomain-1.20230417.5/testdata/meta.com/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.com.sg/input` & `whoisdomain-1.20230417.5/testdata/meta.com.sg/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.com.sg/output` & `whoisdomain-1.20230417.5/testdata/meta.com.sg/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.com.tr/input` & `whoisdomain-1.20230417.5/testdata/meta.com.tr/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.com.tr/output` & `whoisdomain-1.20230417.5/testdata/meta.com.tr/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.jp/input` & `whoisdomain-1.20230417.5/testdata/meta.jp/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.jp/output` & `whoisdomain-1.20230417.5/testdata/meta.jp/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.kr/input` & `whoisdomain-1.20230417.5/testdata/meta.kr/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/meta.kr/output` & `whoisdomain-1.20230417.5/testdata/meta.kr/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/xs4all.nl/input` & `whoisdomain-1.20230417.5/testdata/xs4all.nl/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/testdata/xs4all.nl/output` & `whoisdomain-1.20230417.5/testdata/xs4all.nl/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230417.5/whoisdomain/_0_init_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/whoisdomain/_1_query.py` & `whoisdomain-1.20230417.5/whoisdomain/_1_query.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/whoisdomain/_2_parse.py` & `whoisdomain-1.20230417.5/whoisdomain/_2_parse.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/whoisdomain/_3_adjust.py` & `whoisdomain-1.20230417.5/whoisdomain/_3_adjust.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/whoisdomain/__init__.py` & `whoisdomain-1.20230417.5/whoisdomain/__init__.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/whoisdomain/exceptions.py` & `whoisdomain-1.20230417.5/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230417.5/whoisdomain/tld_regexpr.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/.gitignore` & `whoisdomain-1.20230417.5/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/README.md` & `whoisdomain-1.20230417.5/README.md`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.2/pyproject.toml` & `whoisdomain-1.20230417.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "whoisdomain"
-version = "1.20230417.2"
+version = "1.20230417.5"
 authors = [
   { name="DannyCork"},
 ]
 
 maintainers = [
   { name="Maarten Boot", email="mboot.github@gmail.com" },
 ]
```

### Comparing `whoisdomain-1.20230417.2/PKG-INFO` & `whoisdomain-1.20230417.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230417.2
+Version: 1.20230417.5
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <mboot.github@gmail.com>
 License-Expression: MIT
```

