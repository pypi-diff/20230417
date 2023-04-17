# Comparing `tmp/whoisdomain-1.20230417.5.tar.gz` & `tmp/whoisdomain-1.20230417.6.tar.gz`

## Comparing `whoisdomain-1.20230417.5.tar` & `whoisdomain-1.20230417.6.tar`

### file list

```diff
@@ -1,196 +1,198 @@
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Historical.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/MANIFEST.in
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/license
--rwxr-xr-x   0        0        0     1341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/pypi-test.sh
--rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/pypi.sh
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/pyproject.toml-template
--rwxr-xr-x   0        0        0    15950 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/test2.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   190007 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    55638 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    19473 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    21664 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    62946 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1146965 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   126768 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   115786 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0   147473 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0    95073 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0   136157 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    23854 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    88645 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    92150 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    47582 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    37124 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    80882 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   151599 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    29543 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    52507 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   175017 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   150518 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    46067 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   254545 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   446688 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    54794 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    92867 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   390721 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   135868 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25468 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    62332 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    32673 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    73584 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    68120 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    95559 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12461 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16666 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    15557 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   369261 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json
--rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_1_query.data.json
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_1_query.meta.json
--rw-r--r--   0        0        0    14086 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_2_parse.data.json
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json
--rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json
--rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/__init__.data.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/__init__.meta.json
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/exceptions.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/exceptions.meta.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/DONE
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/TODO
--rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/analize_patterns.py
--rwxr-xr-x   0        0        0     2623 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/compare_known_tld.py
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/convert_to_dict.sh
--rwxr-xr-x   0        0        0     6984 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/makeTestdataAll.sh
--rwxr-xr-x   0        0        0     8753 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/test.py
--rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/test.sh
--rwxr-xr-x   0        0        0    11070 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/test3.py
--rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/testExtend.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/bin/find_input_no_output.sh
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/failed-parsing.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/invalid-tld.txt
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/new-test.txt
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/ok-domains.txt
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/private-reg.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/Old/tests/unknown-dateformat.txt
--rwxr-xr-x   0        0        0     1796 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/make_testdata.sh
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.com/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.com/nameservers
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.com/output
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.net/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.net/nameservers
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.net/output
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.org/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.org/nameservers
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/example.org/output
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/google.com/input
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/google.com/nameservers
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/google.com/output
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/hello.xyz/input
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/hello.xyz/nameservers
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/hello.xyz/output
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.jp/input
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.jp/nameservers
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.jp/output
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.uk/input
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.uk/nameservers
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.co.uk/output
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com/input
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com/nameservers
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com/output
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.sg/input
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.sg/nameservers
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.sg/output
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.tr/input
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.tr/nameservers
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.com.tr/output
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.jp/input
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.jp/nameservers
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.jp/output
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.kr/input
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.kr/nameservers
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/meta.kr/output
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/xs4all.nl/input
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/xs4all.nl/nameservers
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/testdata/xs4all.nl/output
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/_0_init_tld.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/_1_query.py
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/_2_parse.py
--rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/_3_adjust.py
--rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/exceptions.py
--rw-r--r--   0        0        0   104536 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/whoisdomain/tld_regexpr.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.gitignore
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/.hgignore
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/README.md
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/pyproject.toml
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.5/PKG-INFO
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Historical.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/MANIFEST.in
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/license
+-rwxr-xr-x   0        0        0     1341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/pypi-test.sh
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/pypi.sh
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/pyproject.toml-template
+-rwxr-xr-x   0        0        0     2288 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/test.py
+-rwxr-xr-x   0        0        0    15950 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/test2.py
+-rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/test_adjust.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   190007 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    55638 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    19473 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    21664 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    62946 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1146965 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   126768 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   115786 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0   147473 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0    95073 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0   136157 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    23854 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0    88645 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    92150 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    47582 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    37124 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    80882 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   151599 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    29543 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    52507 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   175017 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   150518 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    46067 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   254545 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   446688 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    54794 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    92867 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   390721 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   135868 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25468 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    62332 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    32673 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    73584 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    68120 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    95559 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12461 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    16666 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    15557 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   369261 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json
+-rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_1_query.data.json
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_1_query.meta.json
+-rw-r--r--   0        0        0    14086 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_2_parse.data.json
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json
+-rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json
+-rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/__init__.data.json
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/__init__.meta.json
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/exceptions.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/exceptions.meta.json
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/DONE
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/TODO
+-rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/analize_patterns.py
+-rwxr-xr-x   0        0        0     2623 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/compare_known_tld.py
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/convert_to_dict.sh
+-rwxr-xr-x   0        0        0     6984 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/makeTestdataAll.sh
+-rwxr-xr-x   0        0        0     8753 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/test.py
+-rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/test.sh
+-rwxr-xr-x   0        0        0    11070 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/test3.py
+-rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/testExtend.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/bin/find_input_no_output.sh
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/failed-parsing.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/invalid-tld.txt
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/new-test.txt
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/ok-domains.txt
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/private-reg.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/unknown-dateformat.txt
+-rwxr-xr-x   0        0        0     1796 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/make_testdata.sh
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.com/input
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.com/nameservers
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.com/output
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.net/input
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.net/nameservers
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.net/output
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.org/input
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.org/nameservers
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.org/output
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/google.com/input
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/google.com/nameservers
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/google.com/output
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/hello.xyz/input
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/hello.xyz/nameservers
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/hello.xyz/output
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.jp/input
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.jp/nameservers
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.jp/output
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.uk/input
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.uk/nameservers
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.uk/output
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com/input
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com/nameservers
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com/output
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.sg/input
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.sg/nameservers
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.sg/output
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.tr/input
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.tr/nameservers
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.tr/output
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.jp/input
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.jp/nameservers
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.jp/output
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.kr/input
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.kr/nameservers
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.kr/output
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/xs4all.nl/input
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/xs4all.nl/nameservers
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/xs4all.nl/output
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/_0_init_tld.py
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/_1_query.py
+-rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/_2_parse.py
+-rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/_3_adjust.py
+-rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/exceptions.py
+-rw-r--r--   0        0        0   104888 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/tld_regexpr.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.gitignore
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.hgignore
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/README.md
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/pyproject.toml
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/PKG-INFO
```

### Comparing `whoisdomain-1.20230417.5/pypi-test.sh` & `whoisdomain-1.20230417.6/pypi-test.sh`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/pyproject.toml-template` & `whoisdomain-1.20230417.6/pyproject.toml-template`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/test2.py` & `whoisdomain-1.20230417.6/test2.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.github/ISSUE_TEMPLATE/bug_report.md` & `whoisdomain-1.20230417.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.github/workflows/lint.yml` & `whoisdomain-1.20230417.6/.github/workflows/lint.yml`

 * *Files 21% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         with:
           python-version: 3.x
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install mypy
       - name: Run mypy
-        run: mypy --implicit-optional --install-types --non-interactive --namespace-packages whois
+        run: mypy --implicit-optional --install-types --non-interactive --namespace-packages whoisdomain
```

### Comparing `whoisdomain-1.20230417.5/.github/workflows/python-publish.yml` & `whoisdomain-1.20230417.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/_ast.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/_ast.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/_codecs.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/_codecs.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/_collections_abc.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/_collections_abc.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/_ctypes.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/_ctypes.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/abc.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/abc.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/array.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/array.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/builtins.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/builtins.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/codecs.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/codecs.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/contextlib.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/contextlib.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/datetime.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/datetime.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/enum.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/enum.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/functools.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/functools.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/genericpath.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/genericpath.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/io.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/io.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/mmap.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/mmap.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/pathlib.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/pathlib.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/pickle.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/pickle.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/platform.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/platform.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/platform.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/posixpath.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/posixpath.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/re.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/re.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_compile.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_compile.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_constants.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_constants.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_parse.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/sre_parse.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/subprocess.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/subprocess.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/sys.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/sys.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/time.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/time.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/types.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/types.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/typing.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/typing.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/typing_extensions.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/typing_extensions.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/_typeshed/__init__.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/__init__.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/__init__.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/abc.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/collections/abc.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/ctypes/__init__.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/ctypes/__init__.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/__init__.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/__init__.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/charset.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/charset.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/contentmanager.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/contentmanager.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/errors.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/errors.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/header.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/header.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/message.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/message.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/policy.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/email/policy.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/__init__.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/__init__.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/abc.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/abc.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/machinery.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/machinery.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/__init__.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/__init__.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/decoder.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/decoder.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/encoder.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/json/encoder.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/os/__init__.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/os/__init__.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/os/path.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/os/path.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_1_query.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_1_query.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_1_query.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7571196919023006%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 12), (1, 14)], delete: [9, 8, 7, 6, 5, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 5)], delete: [10, 9, 4, 3, 2, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'whoisdomain._0_init_tld'), (2, 're'), (6, '_collections_abc'), "*

 * *                   "(11, 'enum'), (14, 'types')], delete: [19, 16, 15, 14, 13, 6, 5, 4, 2, 1]}",*

 * * "'hash'": "'45e6e9e386cc90dc0b2e1660189f63759bc2038cda06a63637d71f01d3244b0d'",*

 * * "'id'": "'whoisdomain._2_parse'",*

 * * "'interface_hash'": "'e49d2f96d2efa686d2ddb0dfa389f5 […]*

```diff
@@ -1,83 +1,68 @@
 {
     "data_mtime": 1681721902,
     "dep_lines": [
-        7,
+        12,
+        14,
         1,
         2,
-        3,
         4,
-        5,
-        6,
-        9,
-        1,
-        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        10,
-        10,
-        10,
+        5,
         10,
         10,
         5,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
         30
     ],
     "dependencies": [
+        "whoisdomain._0_init_tld",
         "whoisdomain.exceptions",
-        "subprocess",
-        "time",
+        "re",
         "sys",
-        "os",
-        "platform",
-        "json",
         "typing",
         "builtins",
+        "_collections_abc",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
-        "genericpath",
-        "io",
-        "json.decoder",
-        "json.encoder",
+        "enum",
         "mmap",
         "pickle",
-        "posixpath",
+        "types",
         "typing_extensions"
     ],
-    "hash": "0d226c0e6439d6e0f74e8c8122cd79552c713300c603115577f301540f8e7b34",
-    "id": "whoisdomain._1_query",
+    "hash": "45e6e9e386cc90dc0b2e1660189f63759bc2038cda06a63637d71f01d3244b0d",
+    "id": "whoisdomain._2_parse",
     "ignore_all": false,
-    "interface_hash": "5d9f218e895566945384cc21d442853ccc57cc47776484c5716ecc773fe7d3f4",
-    "mtime": 1681720940,
+    "interface_hash": "e49d2f96d2efa686d2ddb0dfa389f5635aadeae321b3e3ba4797cf02ef5951a7",
+    "mtime": 1681288053,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -111,13 +96,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "whoisdomain/_1_query.py",
+    "path": "whoisdomain/_2_parse.py",
     "plugin_data": null,
-    "size": 5608,
+    "size": 8571,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_2_parse.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_2_parse.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_1_query.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7625%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 7), (3, 3), (5, 5), (6, 6), (7, 9)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (2, 10), (3, 10), (4, 10)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(1, 'subprocess'), (2, 'time'), (4, 'os'), (5, 'platform'), (6, "*

 * *                   "'json'), (13, 'io'), (14, 'json.decoder'), (15, 'json.encoder')], delete: [14, "*

 * *                   '11, 6, 2, 0]}',*

 * * "'hash'": "'343e77056a215375f7380992e01b3e5d349c6f7dbd38b207a3aef5e7a545a127'",*

 * * "'id'": "'whoisdomain._1_query'" […]*

```diff
@@ -1,30 +1,36 @@
 {
     "data_mtime": 1681721902,
     "dep_lines": [
-        12,
-        14,
+        7,
         1,
         2,
+        3,
         4,
+        5,
+        6,
+        9,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
+        10,
+        10,
+        10,
+        10,
         10,
         10,
         5,
         5,
         30,
         30,
         30,
@@ -33,36 +39,39 @@
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "whoisdomain._0_init_tld",
         "whoisdomain.exceptions",
-        "re",
+        "subprocess",
+        "time",
         "sys",
+        "os",
+        "platform",
+        "json",
         "typing",
         "builtins",
-        "_collections_abc",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
-        "enum",
+        "io",
+        "json.decoder",
+        "json.encoder",
         "mmap",
         "pickle",
-        "types",
         "typing_extensions"
     ],
-    "hash": "45e6e9e386cc90dc0b2e1660189f63759bc2038cda06a63637d71f01d3244b0d",
-    "id": "whoisdomain._2_parse",
+    "hash": "343e77056a215375f7380992e01b3e5d349c6f7dbd38b207a3aef5e7a545a127",
+    "id": "whoisdomain._1_query",
     "ignore_all": false,
-    "interface_hash": "e49d2f96d2efa686d2ddb0dfa389f5635aadeae321b3e3ba4797cf02ef5951a7",
-    "mtime": 1681288053,
+    "interface_hash": "5d9f218e895566945384cc21d442853ccc57cc47776484c5716ecc773fe7d3f4",
+    "mtime": 1681731613,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -96,13 +105,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "whoisdomain/_2_parse.py",
+    "path": "whoisdomain/_1_query.py",
     "plugin_data": null,
-    "size": 8571,
+    "size": 5759,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'hash'": "'aaa2898a60970d5207f0dfdb5ffb9302f197e36f8c9a3b880c1d69b08d90833f'",*

 * * "'mtime'": '1681742061',*

 * * "'size'": '8534'}*

```diff
@@ -47,19 +47,19 @@
         "ctypes",
         "enum",
         "mmap",
         "pickle",
         "types",
         "typing_extensions"
     ],
-    "hash": "5f32028396919758635db05cd5c0936905af566011ef0360deb69de8dc22e006",
+    "hash": "aaa2898a60970d5207f0dfdb5ffb9302f197e36f8c9a3b880c1d69b08d90833f",
     "id": "whoisdomain._3_adjust",
     "ignore_all": false,
     "interface_hash": "0b5adf5388d2b9fcf64d59ec8edd3b69ad3c421c7882289e42454c662e5d9b4d",
-    "mtime": 1681288053,
+    "mtime": 1681742061,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -95,11 +95,11 @@
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "whoisdomain/_3_adjust.py",
     "plugin_data": null,
-    "size": 8445,
+    "size": 8534,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/__init__.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/__init__.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/exceptions.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/exceptions.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json` & `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'hash'": "'8acc57a8a0aa84441542714dfef5903f5066551b5a508c631744465debaaa182'",*

 * * "'mtime'": '1681740226',*

 * * "'size'": '104888'}*

```diff
@@ -11,19 +11,19 @@
         30
     ],
     "dependencies": [
         "typing",
         "builtins",
         "abc"
     ],
-    "hash": "e079b5a1e387e9a40b9759acb14f41c19214e14d2f0308857203be26214d5229",
+    "hash": "8acc57a8a0aa84441542714dfef5903f5066551b5a508c631744465debaaa182",
     "id": "whoisdomain.tld_regexpr",
     "ignore_all": false,
     "interface_hash": "bf7372147a4626bd2dd8b6ab9bf5efa08c63feda6d91f0c0719cbdc05d64fe46",
-    "mtime": 1681720941,
+    "mtime": 1681740226,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -59,11 +59,11 @@
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "whoisdomain/tld_regexpr.py",
     "plugin_data": null,
-    "size": 104536,
+    "size": 104888,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.5/Old/DONE` & `whoisdomain-1.20230417.6/Old/DONE`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/Old/analize_patterns.py` & `whoisdomain-1.20230417.6/Old/analize_patterns.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/Old/compare_known_tld.py` & `whoisdomain-1.20230417.6/Old/compare_known_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/Old/makeTestdataAll.sh` & `whoisdomain-1.20230417.6/Old/makeTestdataAll.sh`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/Old/test.py` & `whoisdomain-1.20230417.6/Old/test.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/Old/test.sh` & `whoisdomain-1.20230417.6/Old/test.sh`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/Old/test3.py` & `whoisdomain-1.20230417.6/Old/test3.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/Old/testExtend.py` & `whoisdomain-1.20230417.6/Old/testExtend.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/Old/tests/new-test.txt` & `whoisdomain-1.20230417.6/Old/tests/new-test.txt`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/Old/tests/ok-domains.txt` & `whoisdomain-1.20230417.6/Old/tests/ok-domains.txt`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/make_testdata.sh` & `whoisdomain-1.20230417.6/testdata/make_testdata.sh`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/example.com/output` & `whoisdomain-1.20230417.6/testdata/example.com/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/example.net/output` & `whoisdomain-1.20230417.6/testdata/example.net/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/example.org/input` & `whoisdomain-1.20230417.6/testdata/example.org/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/example.org/output` & `whoisdomain-1.20230417.6/testdata/example.org/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/google.com/input` & `whoisdomain-1.20230417.6/testdata/google.com/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/google.com/output` & `whoisdomain-1.20230417.6/testdata/google.com/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/hello.xyz/input` & `whoisdomain-1.20230417.6/testdata/hello.xyz/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/hello.xyz/output` & `whoisdomain-1.20230417.6/testdata/hello.xyz/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.co.jp/input` & `whoisdomain-1.20230417.6/testdata/meta.co.jp/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.co.jp/output` & `whoisdomain-1.20230417.6/testdata/meta.co.jp/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.co.uk/input` & `whoisdomain-1.20230417.6/testdata/meta.co.uk/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.co.uk/output` & `whoisdomain-1.20230417.6/testdata/meta.co.uk/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.com/input` & `whoisdomain-1.20230417.6/testdata/meta.com/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.com/output` & `whoisdomain-1.20230417.6/testdata/meta.com/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.com.sg/input` & `whoisdomain-1.20230417.6/testdata/meta.com.sg/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.com.sg/output` & `whoisdomain-1.20230417.6/testdata/meta.com.sg/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.com.tr/input` & `whoisdomain-1.20230417.6/testdata/meta.com.tr/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.com.tr/output` & `whoisdomain-1.20230417.6/testdata/meta.com.tr/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.jp/input` & `whoisdomain-1.20230417.6/testdata/meta.jp/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.jp/output` & `whoisdomain-1.20230417.6/testdata/meta.jp/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.kr/input` & `whoisdomain-1.20230417.6/testdata/meta.kr/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/meta.kr/output` & `whoisdomain-1.20230417.6/testdata/meta.kr/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/xs4all.nl/input` & `whoisdomain-1.20230417.6/testdata/xs4all.nl/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/testdata/xs4all.nl/output` & `whoisdomain-1.20230417.6/testdata/xs4all.nl/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230417.6/whoisdomain/_0_init_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/whoisdomain/_1_query.py` & `whoisdomain-1.20230417.6/whoisdomain/_1_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,11 +193,14 @@
     if verbose:
         print(r, file=sys.stderr)
 
     if ignore_returncode is False and p.returncode not in [0, 1]:
         # network error, "fgets: Connection reset by peer" fix, ignore
         if "fgets: Connection reset by peer" in r:
             return r.replace("fgets: Connection reset by peer", "")
+        # connect: Connection refused
+        elif "connect: Connection refused" in r:
+            return r.replace("connect: Connection refused", "")
 
         raise WhoisCommandFailed(r)
 
     return r
```

### Comparing `whoisdomain-1.20230417.5/whoisdomain/_2_parse.py` & `whoisdomain-1.20230417.6/whoisdomain/_2_parse.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/whoisdomain/_3_adjust.py` & `whoisdomain-1.20230417.6/whoisdomain/_3_adjust.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     "%d-%b-%Y",  # 02-jan-2000
     "%d-%m-%Y",  # 02-01-2000
     "%d.%m.%Y",  # 02.02.2000
     "%d/%m/%Y",  # 01/06/2011
     "%Y-%m-%d",  # 2000-01-02
     "%Y.%m.%d",  # 2000.01.02
     "%Y/%m/%d",  # 2005/05/30
+    "%b-%Y",  # aug-1996
     "before %b-%Y",  # before aug-1996
     "before %Y%m%d",  # before 19950101
     "%Y.%m.%d %H:%M:%S",  # 2002.09.19 13:00:00
     "%Y%m%d %H:%M:%S",  # 20110908 14:44:51
     "%Y-%m-%d %H:%M:%S",  # 2011-09-08 14:44:51
     "%Y-%m-%d %H:%M:%S%z",  # 2025-04-27 02:54:19+03:00
     "%Y-%m-%d %H:%M:%S %z",  # 2020-05-18 01:30:25 +0200
@@ -173,14 +174,15 @@
     "%d %b %Y",  # 28 jan 2021
     "%d-%b-%Y %H:%M:%S",  # 30-nov-2009 17:00:58
     "%Y%m%d%H%M%S",  # 20071224102432 used in edu_ua
     "%Y-%m-%d %H:%M:%S (%Z%z)",  # .tw uses (UTC+8) but we need (UTC+0800) for %z match
     "%d %B %Y at %H:%M:%S.%f",  # 07 january 2020 at 23:38:30.772
     "%Y-%m-%d %H:%M:%S.%f %Z",  # 2022-09-18 22:38:18.0 UTC (sn Senegal),
     "%a %b %d %H:%M:%S %Y",  # Thu Oct 21 05:54:20 2032 (kg Kyrgyzstan)
+    "%m-%d-%Y",  # 03-28-2013 # is ambivalent for all days <=12
 ]
 
 CUSTOM_DATE_FORMATS = {
     "ml": "%m/%d/%Y",
 }
```

### Comparing `whoisdomain-1.20230417.5/whoisdomain/__init__.py` & `whoisdomain-1.20230417.6/whoisdomain/__init__.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/whoisdomain/exceptions.py` & `whoisdomain-1.20230417.6/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230417.6/whoisdomain/tld_regexpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -894,17 +894,26 @@
     "name_servers": r"\nnserver:\s*(.+)",
     "status": r"\nstate:\s*(.+)",
 }
 
 # Rossíyskaya Federátsiya) is the Cyrillic country code top-level domain for the Russian Federation,
 # In the Domain Name System it has the ASCII DNS name xn--p1ai.
 
-ZZ["ru.rf"] = {"extend": "ru", "_server": "whois.tcinet.ru"}
-ZZ["рф"] = {"extend": "ru", "_server": "whois.tcinet.ru"}
-ZZ["xn--p1ai"] = {"extend": "ru", "_server": "whois.tcinet.ru"}
+ZZ["ru.rf"] = {
+    "extend": "ru",
+    "_server": "whois.tcinet.ru",
+}
+ZZ["рф"] = {
+    "extend": "ru",
+    "_server": "whois.tcinet.ru",
+}
+ZZ["xn--p1ai"] = {
+    "extend": "ru",
+    "_server": "whois.tcinet.ru",
+}
 
 ZZ["sa"] = {
     "extend": "com",
     "domain_name": r"Domain Name:\s*(.+\.sa)\s",
     "registrant": r"Registrant:\n*(.+)\n",
     "name_servers": r"Name Servers:\s*(.+)\s*(.+)?",
     "registrant_country": None,
@@ -2139,17 +2148,17 @@
 
 ZZ["ph"] = {"extend": "_privateReg"}
 
 ZZ["vc"] = {"extend": "com"}
 ZZ["cm"] = {"extend": "com"}
 
 # russian speaking community
-ZZ["xn--p1acf"] = {"extend": "ru", "_server": "whois.nic.xn--p1acf"}
-ZZ["РУС"] = {"extend": "ru", "_server": "whois.nic.xn--p1acf"}
-ZZ["рус"] = {"extend": "ru", "_server": "whois.nic.xn--p1acf"}
+ZZ["xn--p1acf"] = {"extend": "com"}
+ZZ["РУС"] = {"extend": "com"}
+ZZ["рус"] = {"extend": "com"}
 
 ZZ["vig"] = {"extend": "com", "_server": "whois.afilias-srs.net"}
 
 # autodetect via compare_known_tld.py via IANA tld list and https://github.com/jophy/iana_tld_list
 ZZ["aarp"] = {"_server": "whois.nic.aarp", "extend": "com"}
 ZZ["abbvie"] = {"_server": "whois.nic.abbvie", "extend": "com"}
 ZZ["abc"] = {"_server": "whois.nic.abc", "extend": "com"}
@@ -2736,7 +2745,23 @@
     "domain_name": r"Domain Name:\s+(.+)",
     "status": r"Status:\s(.+)",
     "name_servers": r"DNS Servers:\s+(.+)",
 }
 ZZ["et"] = {"extend": "com", "_server": "whois.ethiotelecom.et"}
 ZZ["mq"] = {"extend": "si", "_server": "whois.mediaserv.net"}
 ZZ["gf"] = {"extend": "si", "_server": "whois.mediaserv.net"}
+
+#    elif domain.endswith('.онлайн') or domain.endswith('.xn--80asehdb'):
+#        tld = 'ru_online'
+
+ZZ["ru_online"] = {
+    "extend": "com",
+    # "expiration_date": r"Registry Expiry Date:\s?(.+)",
+}
+ZZ["xn--80asehdb"] = {
+    "extend": "com",
+    # "expiration_date": r"Registry Expiry Date:\s?(.+)",
+}
+ZZ["онлайн"] = {
+    "extend": "com",
+    # "expiration_date": r"Registry Expiry Date:\s?(.+)",
+}
```

### Comparing `whoisdomain-1.20230417.5/.gitignore` & `whoisdomain-1.20230417.6/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/README.md` & `whoisdomain-1.20230417.6/README.md`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.5/pyproject.toml` & `whoisdomain-1.20230417.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "whoisdomain"
-version = "1.20230417.5"
+version = "1.20230417.6"
 authors = [
   { name="DannyCork"},
 ]
 
 maintainers = [
   { name="Maarten Boot", email="mboot.github@gmail.com" },
 ]
```

### Comparing `whoisdomain-1.20230417.5/PKG-INFO` & `whoisdomain-1.20230417.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230417.5
+Version: 1.20230417.6
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <mboot.github@gmail.com>
 License-Expression: MIT
```

