# Comparing `tmp/soupsieve-2.4.tar.gz` & `tmp/soupsieve-2.4.1.tar.gz`

## Comparing `soupsieve-2.4.tar` & `soupsieve-2.4.1.tar`

### file list

```diff
@@ -1,131 +1,132 @@
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 soupsieve-2.4/.pyspelling.yml
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 soupsieve-2.4/mkdocs.yml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 soupsieve-2.4/tox.ini
--rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/api.md
--rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/differences.md
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/faq.md
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/.snippets/abbr.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/.snippets/links.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/.snippets/refs.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/.snippets/selector_styles.md
--rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/about/changelog.md
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/about/contributing.md
--rw-r--r--   0        0        0    15891 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/about/development.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/about/license.md
--rw-r--r--   0        0        0    18083 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/selectors/basic.md
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/selectors/combinators.md
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/selectors/index.md
--rw-r--r--   0        0        0    52057 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/selectors/pseudo-classes.md
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/src/markdown/selectors/unsupported.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 soupsieve-2.4/docs/theme/announce.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 soupsieve-2.4/requirements/docs.txt
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 soupsieve-2.4/requirements/lint.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 soupsieve-2.4/requirements/project.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 soupsieve-2.4/requirements/tests-nohtml5lib.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 soupsieve-2.4/requirements/tests-nolxml.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 soupsieve-2.4/requirements/tests.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 soupsieve-2.4/requirements/tools.txt
--rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 soupsieve-2.4/soupsieve/__init__.py
--rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 soupsieve-2.4/soupsieve/__meta__.py
--rw-r--r--   0        0        0    58240 2020-02-02 00:00:00.000000 soupsieve-2.4/soupsieve/css_match.py
--rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 soupsieve-2.4/soupsieve/css_parser.py
--rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 soupsieve-2.4/soupsieve/css_types.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 soupsieve-2.4/soupsieve/pretty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 soupsieve-2.4/soupsieve/py.typed
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 soupsieve-2.4/soupsieve/util.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/__init__.py
--rw-r--r--   0        0        0    19587 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_api.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_bs4_cases.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_quirks.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_versions.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/util.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_extra/__init__.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_extra/test_attribute.py
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_extra/test_custom.py
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_extra/test_soup_contains.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_extra/test_soup_contains_own.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_active.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_at_rule.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_class.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_comments.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_descendant.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_escapes.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_id.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_link.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_list.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_pseudo_class.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_pseudo_element.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_type.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level1/test_visited.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level2/__init__.py
--rw-r--r--   0        0        0    12181 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level2/test_attribute.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level2/test_child.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level2/test_first_child.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level2/test_focus.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level2/test_hover.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level2/test_lang.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level2/test_next_sibling.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level2/test_universal_type.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/__init__.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_attribute.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_checked.py
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_disabled.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_empty.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_enabled.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_first_of_type.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_last_child.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_last_of_type.py
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_namespace.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_not.py
--rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_nth_child.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_nth_last_child.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_nth_last_of_type.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_nth_of_type.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_only_child.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_only_of_type.py
--rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_root.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_subsequent_sibling.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level3/test_target.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/__init__.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_any_link.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_attribute.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_current.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_default.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_defined.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_dir.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_focus_visible.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_focus_within.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_future.py
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_has.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_host.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_host_context.py
--rw-r--r--   0        0        0    10963 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_in_range.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_indeterminate.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_is.py
--rw-r--r--   0        0        0    10126 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_lang.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_local_link.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_matches.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_not.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_nth_child.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_nth_last_child.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_optional.py
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_out_of_range.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_past.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_paused.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_placeholder_shown.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_playing.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_read_only.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_read_write.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_required.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_scope.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_target_within.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_user_invalid.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 soupsieve-2.4/tests/test_level4/test_where.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 soupsieve-2.4/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 soupsieve-2.4/LICENSE.md
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 soupsieve-2.4/README.md
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 soupsieve-2.4/hatch_build.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 soupsieve-2.4/pyproject.toml
--rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 soupsieve-2.4/PKG-INFO
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 soupsieve-2.4.1/.pyspelling.yml
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 soupsieve-2.4.1/mkdocs.yml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tox.ini
+-rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/api.md
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/differences.md
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/faq.md
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/.snippets/abbr.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/.snippets/links.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/.snippets/refs.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/.snippets/selector_styles.md
+-rw-r--r--   0        0        0    15111 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/about/changelog.md
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/about/contributing.md
+-rw-r--r--   0        0        0    15891 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/about/development.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/about/license.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/about/security.md
+-rw-r--r--   0        0        0    18083 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/selectors/basic.md
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/selectors/combinators.md
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/selectors/index.md
+-rw-r--r--   0        0        0    52057 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/selectors/pseudo-classes.md
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/src/markdown/selectors/unsupported.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 soupsieve-2.4.1/docs/theme/announce.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 soupsieve-2.4.1/requirements/docs.txt
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 soupsieve-2.4.1/requirements/lint.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 soupsieve-2.4.1/requirements/project.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 soupsieve-2.4.1/requirements/tests-nohtml5lib.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 soupsieve-2.4.1/requirements/tests-nolxml.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 soupsieve-2.4.1/requirements/tests.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 soupsieve-2.4.1/requirements/tools.txt
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 soupsieve-2.4.1/soupsieve/__init__.py
+-rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 soupsieve-2.4.1/soupsieve/__meta__.py
+-rw-r--r--   0        0        0    58152 2020-02-02 00:00:00.000000 soupsieve-2.4.1/soupsieve/css_match.py
+-rw-r--r--   0        0        0    47063 2020-02-02 00:00:00.000000 soupsieve-2.4.1/soupsieve/css_parser.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 soupsieve-2.4.1/soupsieve/css_types.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 soupsieve-2.4.1/soupsieve/pretty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 soupsieve-2.4.1/soupsieve/py.typed
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 soupsieve-2.4.1/soupsieve/util.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/__init__.py
+-rw-r--r--   0        0        0    19587 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_api.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_bs4_cases.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_quirks.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_versions.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/util.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_extra/__init__.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_extra/test_attribute.py
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_extra/test_custom.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_extra/test_soup_contains.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_extra/test_soup_contains_own.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_active.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_at_rule.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_class.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_comments.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_descendant.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_escapes.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_id.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_link.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_list.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_pseudo_class.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_pseudo_element.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_type.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level1/test_visited.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level2/__init__.py
+-rw-r--r--   0        0        0    12181 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level2/test_attribute.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level2/test_child.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level2/test_first_child.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level2/test_focus.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level2/test_hover.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level2/test_lang.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level2/test_next_sibling.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level2/test_universal_type.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/__init__.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_attribute.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_checked.py
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_disabled.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_empty.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_enabled.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_first_of_type.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_last_child.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_last_of_type.py
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_namespace.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_not.py
+-rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_nth_child.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_nth_last_child.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_nth_last_of_type.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_nth_of_type.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_only_child.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_only_of_type.py
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_root.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_subsequent_sibling.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level3/test_target.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/__init__.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_any_link.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_attribute.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_current.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_default.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_defined.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_dir.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_focus_visible.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_focus_within.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_future.py
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_has.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_host.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_host_context.py
+-rw-r--r--   0        0        0    10963 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_in_range.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_indeterminate.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_is.py
+-rw-r--r--   0        0        0    10126 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_lang.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_local_link.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_matches.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_not.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_nth_child.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_nth_last_child.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_optional.py
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_out_of_range.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_past.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_paused.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_placeholder_shown.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_playing.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_read_only.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_read_write.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_required.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_scope.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_target_within.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_user_invalid.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 soupsieve-2.4.1/tests/test_level4/test_where.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 soupsieve-2.4.1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 soupsieve-2.4.1/LICENSE.md
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 soupsieve-2.4.1/README.md
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 soupsieve-2.4.1/hatch_build.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 soupsieve-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 soupsieve-2.4.1/PKG-INFO
```

### Comparing `soupsieve-2.4/.pyspelling.yml` & `soupsieve-2.4.1/.pyspelling.yml`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/mkdocs.yml` & `soupsieve-2.4.1/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 site_name: Soup Sieve
 site_url: https://facelessuser.github.io/soupsieve
 repo_url: https://github.com/facelessuser/soupsieve
 edit_uri: tree/main/docs/src/markdown
 site_description: A modern CSS selector library for Beautiful Soup.
 copyright: |
-  Copyright &copy; 2018 - 2022 <a href="https://github.com/facelessuser"  target="_blank" rel="noopener">Isaac Muse</a>
+  Copyright &copy; 2018 - 2023 <a href="https://github.com/facelessuser"  target="_blank" rel="noopener">Isaac Muse</a>
 
 docs_dir: docs/src/markdown
 theme:
   name: material
   custom_dir: docs/theme
   icon:
     logo: material/book-open-page-variant
@@ -18,15 +18,22 @@
     accent: deep purple
   font:
     text: Roboto
     code: Roboto Mono
   features:
     - navigation.tabs
     - navigation.top
-    - naviagtion.instant
+    - navigation.instant
+    - navigation.indexes
+    - toc.follow
+    - content.code.copy
+    - navigation.footer
+    - search.share
+    - search.highlight
+    - search.suggest
   pymdownx:
     sponsor: "https://github.com/sponsors/facelessuser"
 
 nav:
   - Home:
     - Quick Start: index.md
     - API: api.md
@@ -37,14 +44,15 @@
     - Basic Selectors: selectors/basic.md
     - Combinators and Lists: selectors/combinators.md
     - Pseudo Classes: selectors/pseudo-classes.md
     - Non-Applicable Pseudo Classes: selectors/unsupported.md
   - About:
     - Contributing &amp; Support: about/contributing.md
     - Development: about/development.md
+    - Security Vulnerabilities: about/security.md
     - Changelog: about/changelog.md
     - License: about/license.md
 
 markdown_extensions:
   - markdown.extensions.toc:
       slugify: !!python/object/apply:pymdownx.slugs.slugify {kwds: {case: lower}}
       permalink: ""
@@ -85,14 +93,15 @@
   - pymdownx.progressbar:
   - pymdownx.mark:
   - pymdownx.striphtml:
   - pymdownx.snippets:
       base_path:
       - docs/src/markdown/.snippets
       - LICENSE.md
+      - SECURITY.md
       auto_append:
       - refs.md
   - pymdownx.keys:
       separator: "\uff0b"
   - pymdownx.details:
   - pymdownx.tabbed:
       alternate_style: true
```

#### html2text {}

```diff
@@ -1,37 +1,39 @@
 site_name: Soup Sieve site_url: https://facelessuser.github.io/soupsieve
 repo_url: https://github.com/facelessuser/soupsieve edit_uri: tree/main/docs/
 src/markdown site_description: A modern CSS selector library for Beautiful
-Soup. copyright: | Copyright © 2018 - 2022 Isaac_Muse docs_dir: docs/src/
+Soup. copyright: | Copyright © 2018 - 2023 Isaac_Muse docs_dir: docs/src/
 markdown theme: name: material custom_dir: docs/theme icon: logo: material/
 book-open-page-variant palette: scheme: dracula primary: deep purple accent:
 deep purple font: text: Roboto code: Roboto Mono features: - navigation.tabs -
-navigation.top - naviagtion.instant pymdownx: sponsor: "https://github.com/
-sponsors/facelessuser" nav: - Home: - Quick Start: index.md - API: api.md -
-F.A.Q.: faq.md - Beautiful Soup Differences: differences.md - CSS Selectors: -
-General Details: selectors/index.md - Basic Selectors: selectors/basic.md -
-Combinators and Lists: selectors/combinators.md - Pseudo Classes: selectors/
-pseudo-classes.md - Non-Applicable Pseudo Classes: selectors/unsupported.md -
-About: - Contributing & Support: about/contributing.md - Development: about/
-development.md - Changelog: about/changelog.md - License: about/license.md
-markdown_extensions: - markdown.extensions.toc: slugify: !!python/object/apply:
-pymdownx.slugs.slugify {kwds: {case: lower}} permalink: "" -
-markdown.extensions.admonition: - markdown.extensions.smarty: smart_quotes:
-false - pymdownx.betterem: - markdown.extensions.attr_list: -
+navigation.top - navigation.instant - navigation.indexes - toc.follow -
+content.code.copy - navigation.footer - search.share - search.highlight -
+search.suggest pymdownx: sponsor: "https://github.com/sponsors/facelessuser"
+nav: - Home: - Quick Start: index.md - API: api.md - F.A.Q.: faq.md - Beautiful
+Soup Differences: differences.md - CSS Selectors: - General Details: selectors/
+index.md - Basic Selectors: selectors/basic.md - Combinators and Lists:
+selectors/combinators.md - Pseudo Classes: selectors/pseudo-classes.md - Non-
+Applicable Pseudo Classes: selectors/unsupported.md - About: - Contributing &
+Support: about/contributing.md - Development: about/development.md - Security
+Vulnerabilities: about/security.md - Changelog: about/changelog.md - License:
+about/license.md markdown_extensions: - markdown.extensions.toc: slugify:
+!!python/object/apply:pymdownx.slugs.slugify {kwds: {case: lower}} permalink:
+"" - markdown.extensions.admonition: - markdown.extensions.smarty:
+smart_quotes: false - pymdownx.betterem: - markdown.extensions.attr_list: -
 markdown.extensions.def_list: - markdown.extensions.tables: -
 markdown.extensions.abbr: - markdown.extensions.md_in_html: -
 pymdownx.superfences: - pymdownx.highlight: extend_pygments_lang: - name:
 pycon3 lang: pycon options: python3: true - pymdownx.inlinehilite: -
 pymdownx.magiclink: repo_url_shortener: true repo_url_shorthand: true
 social_url_shorthand: true user: facelessuser repo: soupsieve - pymdownx.tilde:
 - pymdownx.caret: - pymdownx.smartsymbols: - pymdownx.emoji: emoji_index:
 !!python/name:materialx.emoji.twemoji emoji_generator: !!python/name:
 materialx.emoji.to_svg - pymdownx.escapeall: hardbreak: True nbsp: True -
 pymdownx.tasklist: custom_checkbox: true - pymdownx.progressbar: -
 pymdownx.mark: - pymdownx.striphtml: - pymdownx.snippets: base_path: - docs/
-src/markdown/.snippets - LICENSE.md auto_append: - refs.md - pymdownx.keys:
-separator: "\uff0b" - pymdownx.details: - pymdownx.tabbed: alternate_style:
-true - pymdownx.saneheaders: extra: social: - icon: fontawesome/brands/github
-link: https://github.com/facelessuser - icon: fontawesome/brands/discord link:
-https://discord.gg/XBnPUZF plugins: - search: separator: '[:\s\-]+' - git-
-revision-date-localized - minify: minify_html: true -
-mkdocs_pymdownx_material_extras
+src/markdown/.snippets - LICENSE.md - SECURITY.md auto_append: - refs.md -
+pymdownx.keys: separator: "\uff0b" - pymdownx.details: - pymdownx.tabbed:
+alternate_style: true - pymdownx.saneheaders: extra: social: - icon:
+fontawesome/brands/github link: https://github.com/facelessuser - icon:
+fontawesome/brands/discord link: https://discord.gg/XBnPUZF plugins: - search:
+separator: '[:\s\-]+' - git-revision-date-localized - minify: minify_html: true
+- mkdocs_pymdownx_material_extras
```

### Comparing `soupsieve-2.4/tox.ini` & `soupsieve-2.4.1/tox.ini`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/src/markdown/api.md` & `soupsieve-2.4.1/docs/src/markdown/api.md`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/src/markdown/differences.md` & `soupsieve-2.4.1/docs/src/markdown/differences.md`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/src/markdown/faq.md` & `soupsieve-2.4.1/docs/src/markdown/faq.md`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/src/markdown/index.md` & `soupsieve-2.4.1/docs/src/markdown/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -126,17 +126,17 @@
 [<p class="a">Cat</p>, <p class="c">Mouse</p>]
 ```
 
 You can match a single tag:
 
 ```pycon3
 >>> els = sv.select('p:is(.a, .b, .c)', soup)
->>> sv.match(els[0], 'p:not(.b)')
+>>> sv.match('p:not(.b)', els[0])
 True
->>> sv.match(els[1], 'p:not(.b)')
+>>> sv.match('p:not(.b)', els[1])
 False
 ```
 
 Or even just extract comments:
 
 ```pycon3
 >>> sv.comments(soup)
```

### Comparing `soupsieve-2.4/docs/src/markdown/.snippets/links.md` & `soupsieve-2.4.1/docs/src/markdown/.snippets/links.md`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/src/markdown/about/changelog.md` & `soupsieve-2.4.1/docs/src/markdown/about/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 2.4.1
+
+- **FIX**: Attribute syntax for case insensitive flag optionally allows a space, it does not require one.
+
 ## 2.4
 
 - **NEW**: Update to support changes related to `:lang()` in the official CSS spec. `:lang("")` should match unspecified
   languages, e.g. `lang=""`, but not `lang=und`.
 - **NEW**: Only `:is()` and `:where()` should allow forgiving selector lists according to latest CSS (as far as Soup
   Sieve supports "forgiving" which is limited to empty selectors).
 - **NEW**: Formally drop Python 3.6.
```

### Comparing `soupsieve-2.4/docs/src/markdown/about/contributing.md` & `soupsieve-2.4.1/docs/src/markdown/about/contributing.md`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/src/markdown/about/development.md` & `soupsieve-2.4.1/docs/src/markdown/about/development.md`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/src/markdown/selectors/basic.md` & `soupsieve-2.4.1/docs/src/markdown/selectors/basic.md`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/src/markdown/selectors/combinators.md` & `soupsieve-2.4.1/docs/src/markdown/selectors/combinators.md`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/src/markdown/selectors/index.md` & `soupsieve-2.4.1/docs/src/markdown/selectors/index.md`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/src/markdown/selectors/pseudo-classes.md` & `soupsieve-2.4.1/docs/src/markdown/selectors/pseudo-classes.md`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/src/markdown/selectors/unsupported.md` & `soupsieve-2.4.1/docs/src/markdown/selectors/unsupported.md`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/docs/theme/announce.html` & `soupsieve-2.4.1/docs/theme/announce.html`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/soupsieve/__init__.py` & `soupsieve-2.4.1/soupsieve/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,31 +28,31 @@
 from __future__ import annotations
 from .__meta__ import __version__, __version_info__  # noqa: F401
 from . import css_parser as cp
 from . import css_match as cm
 from . import css_types as ct
 from .util import DEBUG, SelectorSyntaxError  # noqa: F401
 import bs4  # type: ignore[import]
-from typing import Optional, Any, Iterator, Iterable
+from typing import Any, Iterator, Iterable
 
 __all__ = (
     'DEBUG', 'SelectorSyntaxError', 'SoupSieve',
     'closest', 'compile', 'filter', 'iselect',
     'match', 'select', 'select_one'
 )
 
 SoupSieve = cm.SoupSieve
 
 
 def compile(  # noqa: A001
     pattern: str,
-    namespaces: Optional[dict[str, str]] = None,
+    namespaces: dict[str, str] | None = None,
     flags: int = 0,
     *,
-    custom: Optional[dict[str, str]] = None,
+    custom: dict[str, str] | None = None,
     **kwargs: Any
 ) -> cm.SoupSieve:
     """Compile CSS pattern."""
 
     if isinstance(pattern, SoupSieve):
         if flags:
             raise ValueError("Cannot process 'flags' argument on a compiled selector list")
@@ -75,90 +75,90 @@
 
     cp._purge_cache()
 
 
 def closest(
     select: str,
     tag: 'bs4.Tag',
-    namespaces: Optional[dict[str, str]] = None,
+    namespaces: dict[str, str] | None = None,
     flags: int = 0,
     *,
-    custom: Optional[dict[str, str]] = None,
+    custom: dict[str, str] | None = None,
     **kwargs: Any
 ) -> 'bs4.Tag':
     """Match closest ancestor."""
 
     return compile(select, namespaces, flags, **kwargs).closest(tag)
 
 
 def match(
     select: str,
     tag: 'bs4.Tag',
-    namespaces: Optional[dict[str, str]] = None,
+    namespaces: dict[str, str] | None = None,
     flags: int = 0,
     *,
-    custom: Optional[dict[str, str]] = None,
+    custom: dict[str, str] | None = None,
     **kwargs: Any
 ) -> bool:
     """Match node."""
 
     return compile(select, namespaces, flags, **kwargs).match(tag)
 
 
 def filter(  # noqa: A001
     select: str,
     iterable: Iterable['bs4.Tag'],
-    namespaces: Optional[dict[str, str]] = None,
+    namespaces: dict[str, str] | None = None,
     flags: int = 0,
     *,
-    custom: Optional[dict[str, str]] = None,
+    custom: dict[str, str] | None = None,
     **kwargs: Any
 ) -> list['bs4.Tag']:
     """Filter list of nodes."""
 
     return compile(select, namespaces, flags, **kwargs).filter(iterable)
 
 
 def select_one(
     select: str,
     tag: 'bs4.Tag',
-    namespaces: Optional[dict[str, str]] = None,
+    namespaces: dict[str, str] | None = None,
     flags: int = 0,
     *,
-    custom: Optional[dict[str, str]] = None,
+    custom: dict[str, str] | None = None,
     **kwargs: Any
 ) -> 'bs4.Tag':
     """Select a single tag."""
 
     return compile(select, namespaces, flags, **kwargs).select_one(tag)
 
 
 def select(
     select: str,
     tag: 'bs4.Tag',
-    namespaces: Optional[dict[str, str]] = None,
+    namespaces: dict[str, str] | None = None,
     limit: int = 0,
     flags: int = 0,
     *,
-    custom: Optional[dict[str, str]] = None,
+    custom: dict[str, str] | None = None,
     **kwargs: Any
 ) -> list['bs4.Tag']:
     """Select the specified tags."""
 
     return compile(select, namespaces, flags, **kwargs).select(tag, limit)
 
 
 def iselect(
     select: str,
     tag: 'bs4.Tag',
-    namespaces: Optional[dict[str, str]] = None,
+    namespaces: dict[str, str] | None = None,
     limit: int = 0,
     flags: int = 0,
     *,
-    custom: Optional[dict[str, str]] = None,
+    custom: dict[str, str] | None = None,
     **kwargs: Any
 ) -> Iterator['bs4.Tag']:
     """Iterate the specified tags."""
 
     for el in compile(select, namespaces, flags, **kwargs).iselect(tag, limit):
         yield el
```

### Comparing `soupsieve-2.4/soupsieve/__meta__.py` & `soupsieve-2.4.1/soupsieve/__meta__.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,9 +189,9 @@
 
     # Handle post
     post = int(m.group('post')) if m.group('post') else 0
 
     return Version(major, minor, micro, release, pre, post, dev)
 
 
-__version_info__ = Version(2, 4, 0, "final")
+__version_info__ = Version(2, 4, 1, "final")
 __version__ = __version_info__._get_canonical()
```

### Comparing `soupsieve-2.4/soupsieve/css_match.py` & `soupsieve-2.4.1/soupsieve/css_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 from datetime import datetime
 from . import util
 import re
 from . import css_types as ct
 import unicodedata
 import bs4  # type: ignore[import]
-from typing import Iterator, Iterable, Any, Optional, Callable, Sequence, cast  # noqa: F401
+from typing import Iterator, Iterable, Any, Callable, Sequence, cast  # noqa: F401
 
 # Empty tag pattern (whitespace okay)
 RE_NOT_EMPTY = re.compile('[^ \t\r\n\f]')
 
 RE_NOT_WS = re.compile('[^ \t\r\n\f]+')
 
 # Relationships
@@ -167,15 +167,15 @@
         if not no_iframe or not self.is_iframe(el):
             for content in el.contents:
                 yield content
 
     def get_children(
         self,
         el: bs4.Tag,
-        start: Optional[int] = None,
+        start: int | None = None,
         reverse: bool = False,
         tags: bool = True,
         no_iframe: bool = False
     ) -> Iterator[bs4.PageElement]:
         """Get children."""
 
         if not no_iframe or not self.is_iframe(el):
@@ -235,30 +235,30 @@
 
         parent = el.parent
         if no_iframe and parent is not None and self.is_iframe(parent):
             parent = None
         return parent
 
     @staticmethod
-    def get_tag_name(el: bs4.Tag) -> Optional[str]:
+    def get_tag_name(el: bs4.Tag) -> str | None:
         """Get tag."""
 
-        return cast(Optional[str], el.name)
+        return cast('str | None', el.name)
 
     @staticmethod
-    def get_prefix_name(el: bs4.Tag) -> Optional[str]:
+    def get_prefix_name(el: bs4.Tag) -> str | None:
         """Get prefix."""
 
-        return cast(Optional[str], el.prefix)
+        return cast('str | None', el.prefix)
 
     @staticmethod
-    def get_uri(el: bs4.Tag) -> Optional[str]:
+    def get_uri(el: bs4.Tag) -> str | None:
         """Get namespace `URI`."""
 
-        return cast(Optional[str], el.namespace)
+        return cast('str | None', el.namespace)
 
     @classmethod
     def get_next(cls, el: bs4.Tag, tags: bool = True) -> bs4.PageElement:
         """Get next sibling tag."""
 
         sibling = el.next_sibling
         while tags and not cls.is_tag(sibling) and sibling is not None:
@@ -283,15 +283,15 @@
         like we do in the case of `is_html_tag`.
         """
 
         ns = getattr(el, 'namespace') if el else None
         return bool(ns and ns == NS_XHTML)
 
     @staticmethod
-    def split_namespace(el: bs4.Tag, attr_name: str) -> tuple[Optional[str], Optional[str]]:
+    def split_namespace(el: bs4.Tag, attr_name: str) -> tuple[str | None, str | None]:
         """Return namespace and attribute name without the prefix."""
 
         return getattr(attr_name, 'namespace', None), getattr(attr_name, 'name', None)
 
     @classmethod
     def normalize_value(cls, value: Any) -> str | Sequence[str]:
         """Normalize the value to be a string or list of strings."""
@@ -326,16 +326,16 @@
         return str(value)
 
     @classmethod
     def get_attribute_by_name(
         cls,
         el: bs4.Tag,
         name: str,
-        default: Optional[str | Sequence[str]] = None
-    ) -> Optional[str | Sequence[str]]:
+        default: str | Sequence[str] | None = None
+    ) -> str | Sequence[str] | None:
         """Get attribute by name."""
 
         value = default
         if el._is_xml:
             try:
                 value = cls.normalize_value(el.attrs[name])
             except KeyError:
@@ -344,15 +344,15 @@
             for k, v in el.attrs.items():
                 if util.lower(k) == name:
                     value = cls.normalize_value(v)
                     break
         return value
 
     @classmethod
-    def iter_attributes(cls, el: bs4.Tag) -> Iterator[tuple[str, Optional[str | Sequence[str]]]]:
+    def iter_attributes(cls, el: bs4.Tag) -> Iterator[tuple[str, str | Sequence[str] | None]]:
         """Iterate attributes."""
 
         for k, v in el.attrs.items():
             yield k, cls.normalize_value(v)
 
     @classmethod
     def get_classes(cls, el: bs4.Tag) -> Sequence[str]:
@@ -420,18 +420,18 @@
     @staticmethod
     def validate_minutes(minutes: int) -> bool:
         """Validate minutes."""
 
         return 0 <= minutes <= 59
 
     @classmethod
-    def parse_value(cls, itype: str, value: Optional[str]) -> Optional[tuple[float, ...]]:
+    def parse_value(cls, itype: str, value: str | None) -> tuple[float, ...] | None:
         """Parse the input value."""
 
-        parsed = None  # type: Optional[tuple[float, ...]]
+        parsed = None  # type: tuple[float, ...] | None
         if value is None:
             return value
         if itype == "date":
             m = RE_DATE.match(value)
             if m:
                 year = int(m.group('year'), 10)
                 month = int(m.group('month'), 10)
@@ -482,15 +482,15 @@
 class CSSMatch(_DocumentNav):
     """Perform CSS matching."""
 
     def __init__(
         self,
         selectors: ct.SelectorList,
         scope: bs4.Tag,
-        namespaces: Optional[ct.Namespaces],
+        namespaces: ct.Namespaces | None,
         flags: int
     ) -> None:
         """Initialize."""
 
         self.assert_valid_input(scope)
         self.tag = scope
         self.cached_meta_lang = []  # type: list[tuple[str, str]]
@@ -541,27 +541,27 @@
         return namespace
 
     def is_html_tag(self, el: bs4.Tag) -> bool:
         """Check if tag is in HTML namespace."""
 
         return self.get_tag_ns(el) == NS_XHTML
 
-    def get_tag(self, el: bs4.Tag) -> Optional[str]:
+    def get_tag(self, el: bs4.Tag) -> str | None:
         """Get tag."""
 
         name = self.get_tag_name(el)
         return util.lower(name) if name is not None and not self.is_xml else name
 
-    def get_prefix(self, el: bs4.Tag) -> Optional[str]:
+    def get_prefix(self, el: bs4.Tag) -> str | None:
         """Get prefix."""
 
         prefix = self.get_prefix_name(el)
         return util.lower(prefix) if prefix is not None and not self.is_xml else prefix
 
-    def find_bidi(self, el: bs4.Tag) -> Optional[int]:
+    def find_bidi(self, el: bs4.Tag) -> int | None:
         """Get directionality from element text."""
 
         for node in self.get_children(el, tags=False):
 
             # Analyze child text nodes
             if self.is_tag(node):
 
@@ -649,16 +649,16 @@
 
         return match
 
     def match_attribute_name(
         self,
         el: bs4.Tag,
         attr: str,
-        prefix: Optional[str]
-    ) -> Optional[str | Sequence[str]]:
+        prefix: str | None
+    ) -> str | Sequence[str] | None:
         """Match attribute name and return value if it exists."""
 
         value = None
         if self.supports_namespaces():
             value = None
             # If we have not defined namespaces, we can't very well find them, so don't bother trying.
             if prefix:
@@ -747,15 +747,15 @@
 
         name = (util.lower(tag.name) if not self.is_xml and tag.name is not None else tag.name)
         return not (
             name is not None and
             name not in (self.get_tag(el), '*')
         )
 
-    def match_tag(self, el: bs4.Tag, tag: Optional[ct.SelectorTag]) -> bool:
+    def match_tag(self, el: bs4.Tag, tag: ct.SelectorTag | None) -> bool:
         """Match the tag."""
 
         match = True
         if tag is not None:
             # Verify namespace
             if not self.match_namespace(el, tag):
                 match = False
@@ -1026,15 +1026,15 @@
                 match = False
         return match
 
     def match_contains(self, el: bs4.Tag, contains: tuple[ct.SelectorContains, ...]) -> bool:
         """Match element if it contains text."""
 
         match = True
-        content = None  # type: Optional[str | Sequence[str]]
+        content = None  # type: str | Sequence[str] | None
         for contain_list in contains:
             if content is None:
                 if contain_list.own:
                     content = self.get_own_text(el, no_iframe=self.is_html)
                 else:
                     content = self.get_text(el, no_iframe=self.is_html)
             found = False
@@ -1095,15 +1095,15 @@
 
     def match_indeterminate(self, el: bs4.Tag) -> bool:
         """Match default."""
 
         match = False
         name = cast(str, self.get_attribute_by_name(el, 'name'))
 
-        def get_parent_form(el: bs4.Tag) -> Optional[bs4.Tag]:
+        def get_parent_form(el: bs4.Tag) -> bs4.Tag | None:
             """Find this input's form."""
             form = None
             parent = self.get_parent(el, no_iframe=True)
             while form is None:
                 if self.get_tag(parent) == 'form' and self.is_html_tag(parent):
                     form = parent
                     break
@@ -1474,15 +1474,15 @@
             if self.match(child):
                 yield child
                 if lim is not None:
                     lim -= 1
                     if lim < 1:
                         break
 
-    def closest(self) -> Optional[bs4.Tag]:
+    def closest(self) -> bs4.Tag | None:
         """Match closest ancestor."""
 
         current = self.tag
         closest = None
         while closest is None and current is not None:
             if self.match(current):
                 closest = current
@@ -1502,26 +1502,26 @@
 
 
 class SoupSieve(ct.Immutable):
     """Compiled Soup Sieve selector matching object."""
 
     pattern: str
     selectors: ct.SelectorList
-    namespaces: Optional[ct.Namespaces]
+    namespaces: ct.Namespaces | None
     custom: dict[str, str]
     flags: int
 
     __slots__ = ("pattern", "selectors", "namespaces", "custom", "flags", "_hash")
 
     def __init__(
         self,
         pattern: str,
         selectors: ct.SelectorList,
-        namespaces: Optional[ct.Namespaces],
-        custom: Optional[ct.CustomSelectors],
+        namespaces: ct.Namespaces | None,
+        custom: ct.CustomSelectors | None,
         flags: int
     ):
         """Initialize."""
 
         super().__init__(
             pattern=pattern,
             selectors=selectors,
```

### Comparing `soupsieve-2.4/soupsieve/css_parser.py` & `soupsieve-2.4.1/soupsieve/css_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 from functools import lru_cache
 from . import util
 from . import css_match as cm
 from . import css_types as ct
 from .util import SelectorSyntaxError
 import warnings
-from typing import Optional, Match, Any, Iterator, cast
+from typing import Match, Any, Iterator, cast
 
 UNICODE_REPLACEMENT_CHAR = 0xFFFD
 
 # Simple pseudo classes that take no parameters
 PSEUDO_SIMPLE = {
     ":any-link",
     ":empty",
@@ -109,15 +109,15 @@
 NTH = r'(?:[-+])?(?:[0-9]+n?|n)(?:(?<=n){ws}*(?:[-+]){ws}*(?:[0-9]+))?'.format(ws=WSC)
 # Value: quoted string or identifier
 VALUE = r'''
 (?:"(?:\\(?:.|{nl})|[^\\"\r\n\f]+)*?"|'(?:\\(?:.|{nl})|[^\\'\r\n\f]+)*?'|{ident}+)
 '''.format(nl=NEWLINE, ident=IDENTIFIER)
 # Attribute value comparison. `!=` is handled special as it is non-standard.
 ATTR = r'''
-(?:{ws}*(?P<cmp>[!~^|*$]?=){ws}*(?P<value>{value})(?:{ws}+(?P<case>[is]))?)?{ws}*\]
+(?:{ws}*(?P<cmp>[!~^|*$]?=){ws}*(?P<value>{value})(?:{ws}*(?P<case>[is]))?)?{ws}*\]
 '''.format(ws=WSC, value=VALUE)
 
 # Selector patterns
 # IDs (`#id`)
 PAT_ID = r'\#{ident}'.format(ident=IDENTIFIER)
 # Classes (`.class`)
 PAT_CLASS = r'\.{ident}'.format(ident=IDENTIFIER)
@@ -203,16 +203,16 @@
 # Maximum cached patterns to store
 _MAXCACHE = 500
 
 
 @lru_cache(maxsize=_MAXCACHE)
 def _cached_css_compile(
     pattern: str,
-    namespaces: Optional[ct.Namespaces],
-    custom: Optional[ct.CustomSelectors],
+    namespaces: ct.Namespaces | None,
+    custom: ct.CustomSelectors | None,
     flags: int
 ) -> cm.SoupSieve:
     """Cached CSS compile."""
 
     custom_selectors = process_custom(custom)
     return cm.SoupSieve(
         pattern,
@@ -229,15 +229,15 @@
 
 def _purge_cache() -> None:
     """Purge the cache."""
 
     _cached_css_compile.cache_clear()
 
 
-def process_custom(custom: Optional[ct.CustomSelectors]) -> dict[str, str | ct.SelectorList]:
+def process_custom(custom: ct.CustomSelectors | None) -> dict[str, str | ct.SelectorList]:
     """Process custom."""
 
     custom_selectors = {}
     if custom is not None:
         for key, value in custom.items():
             name = util.lower(key)
             if RE_CUSTOM.match(name) is None:
@@ -313,15 +313,15 @@
         self.re_pattern = re.compile(pattern, re.I | re.X | re.U)
 
     def get_name(self) -> str:
         """Get name."""
 
         return self.name
 
-    def match(self, selector: str, index: int, flags: int) -> Optional[Match[str]]:
+    def match(self, selector: str, index: int, flags: int) -> Match[str] | None:
         """Match the selector."""
 
         return self.re_pattern.match(selector, index)
 
 
 class SpecialPseudoPattern(SelectorPattern):
     """Selector pattern."""
@@ -332,23 +332,23 @@
         self.patterns = {}
         for p in patterns:
             name = p[0]
             pattern = p[3](name, p[2])
             for pseudo in p[1]:
                 self.patterns[pseudo] = pattern
 
-        self.matched_name = None  # type: Optional[SelectorPattern]
+        self.matched_name = None  # type: SelectorPattern | None
         self.re_pseudo_name = re.compile(PAT_PSEUDO_CLASS_SPECIAL, re.I | re.X | re.U)
 
     def get_name(self) -> str:
         """Get name."""
 
         return '' if self.matched_name is None else self.matched_name.get_name()
 
-    def match(self, selector: str, index: int, flags: int) -> Optional[Match[str]]:
+    def match(self, selector: str, index: int, flags: int) -> Match[str] | None:
         """Match the selector."""
 
         pseudo = None
         m = self.re_pseudo_name.match(selector, index)
         if m:
             name = util.lower(css_unescape(m.group('name')))
             pattern = self.patterns.get(name)
@@ -368,22 +368,22 @@
     Once we are done collecting the data for a compound selector, we freeze
     the data in an object that can be pickled and hashed.
     """
 
     def __init__(self, **kwargs: Any) -> None:
         """Initialize."""
 
-        self.tag = kwargs.get('tag', None)  # type: Optional[ct.SelectorTag]
+        self.tag = kwargs.get('tag', None)  # type: ct.SelectorTag | None
         self.ids = kwargs.get('ids', [])  # type: list[str]
         self.classes = kwargs.get('classes', [])  # type: list[str]
         self.attributes = kwargs.get('attributes', [])  # type: list[ct.SelectorAttribute]
         self.nth = kwargs.get('nth', [])  # type: list[ct.SelectorNth]
         self.selectors = kwargs.get('selectors', [])  # type: list[ct.SelectorList]
         self.relations = kwargs.get('relations', [])  # type: list[_Selector]
-        self.rel_type = kwargs.get('rel_type', None)  # type: Optional[str]
+        self.rel_type = kwargs.get('rel_type', None)  # type: str | None
         self.contains = kwargs.get('contains', [])  # type: list[ct.SelectorContains]
         self.lang = kwargs.get('lang', [])  # type: list[ct.SelectorLang]
         self.flags = kwargs.get('flags', 0)  # type: int
         self.no_match = kwargs.get('no_match', False)  # type: bool
 
     def _freeze_relations(self, relations: list[_Selector]) -> ct.SelectorList:
         """Freeze relation."""
@@ -458,15 +458,15 @@
         SelectorPattern("attribute", PAT_ATTR),
         SelectorPattern("combine", PAT_COMBINE)
     )
 
     def __init__(
         self,
         selector: str,
-        custom: Optional[dict[str, str | ct.SelectorList]] = None,
+        custom: dict[str, str | ct.SelectorList] | None = None,
         flags: int = 0
     ) -> None:
         """Initialize."""
 
         self.pattern = selector.replace('\x00', '\ufffd')
         self.flags = flags
         self.debug = self.flags & util.DEBUG
```

### Comparing `soupsieve-2.4/soupsieve/css_types.py` & `soupsieve-2.4.1/soupsieve/css_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """CSS selector structure items."""
 from __future__ import annotations
 import copyreg
 from .pretty import pretty
-from typing import Any, Iterator, Hashable, Optional, Pattern, Iterable, Mapping
+from typing import Any, Iterator, Hashable, Pattern, Iterable, Mapping
 
 __all__ = (
     'Selector',
     'SelectorNull',
     'SelectorTag',
     'SelectorAttribute',
     'SelectorContains',
@@ -185,36 +185,36 @@
     """Selector."""
 
     __slots__ = (
         'tag', 'ids', 'classes', 'attributes', 'nth', 'selectors',
         'relation', 'rel_type', 'contains', 'lang', 'flags', '_hash'
     )
 
-    tag: Optional[SelectorTag]
+    tag: SelectorTag | None
     ids: tuple[str, ...]
     classes: tuple[str, ...]
     attributes: tuple[SelectorAttribute, ...]
     nth: tuple[SelectorNth, ...]
     selectors: tuple[SelectorList, ...]
     relation: SelectorList
-    rel_type: Optional[str]
+    rel_type: str | None
     contains: tuple[SelectorContains, ...]
     lang: tuple[SelectorLang, ...]
     flags: int
 
     def __init__(
         self,
-        tag: Optional[SelectorTag],
+        tag: SelectorTag | None,
         ids: tuple[str, ...],
         classes: tuple[str, ...],
         attributes: tuple[SelectorAttribute, ...],
         nth: tuple[SelectorNth, ...],
         selectors: tuple[SelectorList, ...],
         relation: SelectorList,
-        rel_type: Optional[str],
+        rel_type: str | None,
         contains: tuple[SelectorContains, ...],
         lang: tuple[SelectorLang, ...],
         flags: int
     ):
         """Initialize."""
 
         super().__init__(
@@ -243,38 +243,38 @@
 
 class SelectorTag(Immutable):
     """Selector tag."""
 
     __slots__ = ("name", "prefix", "_hash")
 
     name: str
-    prefix: Optional[str]
+    prefix: str | None
 
-    def __init__(self, name: str, prefix: Optional[str]) -> None:
+    def __init__(self, name: str, prefix: str | None) -> None:
         """Initialize."""
 
         super().__init__(name=name, prefix=prefix)
 
 
 class SelectorAttribute(Immutable):
     """Selector attribute rule."""
 
     __slots__ = ("attribute", "prefix", "pattern", "xml_type_pattern", "_hash")
 
     attribute: str
     prefix: str
-    pattern: Optional[Pattern[str]]
-    xml_type_pattern: Optional[Pattern[str]]
+    pattern: Pattern[str] | None
+    xml_type_pattern: Pattern[str] | None
 
     def __init__(
         self,
         attribute: str,
         prefix: str,
-        pattern: Optional[Pattern[str]],
-        xml_type_pattern: Optional[Pattern[str]]
+        pattern: Pattern[str] | None,
+        xml_type_pattern: Pattern[str] | None
     ) -> None:
         """Initialize."""
 
         super().__init__(
             attribute=attribute,
             prefix=prefix,
             pattern=pattern,
@@ -356,15 +356,15 @@
 
     selectors: tuple[Selector | SelectorNull, ...]
     is_not: bool
     is_html: bool
 
     def __init__(
         self,
-        selectors: Optional[Iterable[Selector | SelectorNull]] = None,
+        selectors: Iterable[Selector | SelectorNull] | None = None,
         is_not: bool = False,
         is_html: bool = False
     ) -> None:
         """Initialize."""
 
         super().__init__(
             selectors=tuple(selectors) if selectors is not None else tuple(),
```

### Comparing `soupsieve-2.4/soupsieve/pretty.py` & `soupsieve-2.4.1/soupsieve/pretty.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/soupsieve/util.py` & `soupsieve-2.4.1/soupsieve/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utility."""
 from __future__ import annotations
 from functools import wraps, lru_cache
 import warnings
 import re
-from typing import Callable, Any, Optional
+from typing import Callable, Any
 
 DEBUG = 0x00001
 
 RE_PATTERN_LINE_SPLIT = re.compile(r'(?:\r\n|(?!\r\n)[\n\r])|$')
 
 UC_A = ord('A')
 UC_Z = ord('Z')
@@ -23,15 +23,15 @@
         new_string.append(chr(o + 32) if UC_A <= o <= UC_Z else c)
     return ''.join(new_string)
 
 
 class SelectorSyntaxError(Exception):
     """Syntax error in a CSS selector."""
 
-    def __init__(self, msg: str, pattern: Optional[str] = None, index: Optional[int] = None) -> None:
+    def __init__(self, msg: str, pattern: str | None = None, index: int | None = None) -> None:
         """Initialize."""
 
         self.line = None
         self.col = None
         self.context = None
 
         if pattern is not None and index is not None:
@@ -80,15 +80,15 @@
     """Get the pattern context."""
 
     last = 0
     current_line = 1
     col = 1
     text = []  # type: list[str]
     line = 1
-    offset = None  # type: Optional[int]
+    offset = None  # type: int | None
 
     # Split pattern by newline and handle the text before the newline
     for m in RE_PATTERN_LINE_SPLIT.finditer(pattern):
         linetext = pattern[last:m.start(0)]
         if not len(m.group(0)) and not len(text):
             indent = ''
             offset = -1
```

### Comparing `soupsieve-2.4/tests/test_api.py` & `soupsieve-2.4.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_bs4_cases.py` & `soupsieve-2.4.1/tests/test_bs4_cases.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_quirks.py` & `soupsieve-2.4.1/tests/test_quirks.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_versions.py` & `soupsieve-2.4.1/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/util.py` & `soupsieve-2.4.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_extra/test_attribute.py` & `soupsieve-2.4.1/tests/test_extra/test_attribute.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_extra/test_custom.py` & `soupsieve-2.4.1/tests/test_extra/test_custom.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_extra/test_soup_contains.py` & `soupsieve-2.4.1/tests/test_extra/test_soup_contains.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_extra/test_soup_contains_own.py` & `soupsieve-2.4.1/tests/test_extra/test_soup_contains_own.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level1/test_active.py` & `soupsieve-2.4.1/tests/test_level1/test_active.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level1/test_class.py` & `soupsieve-2.4.1/tests/test_level1/test_class.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level1/test_comments.py` & `soupsieve-2.4.1/tests/test_level1/test_comments.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level1/test_descendant.py` & `soupsieve-2.4.1/tests/test_level1/test_descendant.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level1/test_escapes.py` & `soupsieve-2.4.1/tests/test_level1/test_escapes.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level1/test_id.py` & `soupsieve-2.4.1/tests/test_level1/test_id.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level1/test_link.py` & `soupsieve-2.4.1/tests/test_level1/test_link.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level1/test_list.py` & `soupsieve-2.4.1/tests/test_level1/test_list.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level1/test_type.py` & `soupsieve-2.4.1/tests/test_level1/test_type.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level1/test_visited.py` & `soupsieve-2.4.1/tests/test_level1/test_visited.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level2/test_attribute.py` & `soupsieve-2.4.1/tests/test_level2/test_attribute.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level2/test_child.py` & `soupsieve-2.4.1/tests/test_level2/test_child.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level2/test_first_child.py` & `soupsieve-2.4.1/tests/test_level2/test_first_child.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level2/test_focus.py` & `soupsieve-2.4.1/tests/test_level2/test_focus.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level2/test_hover.py` & `soupsieve-2.4.1/tests/test_level2/test_hover.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level2/test_lang.py` & `soupsieve-2.4.1/tests/test_level2/test_lang.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level2/test_next_sibling.py` & `soupsieve-2.4.1/tests/test_level2/test_next_sibling.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level2/test_universal_type.py` & `soupsieve-2.4.1/tests/test_level2/test_universal_type.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_attribute.py` & `soupsieve-2.4.1/tests/test_level3/test_attribute.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_checked.py` & `soupsieve-2.4.1/tests/test_level3/test_checked.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_disabled.py` & `soupsieve-2.4.1/tests/test_level3/test_disabled.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_empty.py` & `soupsieve-2.4.1/tests/test_level3/test_empty.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_enabled.py` & `soupsieve-2.4.1/tests/test_level3/test_enabled.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_first_of_type.py` & `soupsieve-2.4.1/tests/test_level3/test_first_of_type.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_last_child.py` & `soupsieve-2.4.1/tests/test_level3/test_last_child.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_last_of_type.py` & `soupsieve-2.4.1/tests/test_level3/test_last_of_type.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_namespace.py` & `soupsieve-2.4.1/tests/test_level3/test_namespace.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_not.py` & `soupsieve-2.4.1/tests/test_level3/test_not.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_nth_child.py` & `soupsieve-2.4.1/tests/test_level3/test_nth_child.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_nth_last_child.py` & `soupsieve-2.4.1/tests/test_level3/test_nth_last_child.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_nth_last_of_type.py` & `soupsieve-2.4.1/tests/test_level3/test_nth_last_of_type.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_nth_of_type.py` & `soupsieve-2.4.1/tests/test_level3/test_nth_of_type.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_only_child.py` & `soupsieve-2.4.1/tests/test_level3/test_only_child.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_only_of_type.py` & `soupsieve-2.4.1/tests/test_level3/test_only_of_type.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_root.py` & `soupsieve-2.4.1/tests/test_level3/test_root.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_subsequent_sibling.py` & `soupsieve-2.4.1/tests/test_level3/test_subsequent_sibling.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level3/test_target.py` & `soupsieve-2.4.1/tests/test_level3/test_target.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_any_link.py` & `soupsieve-2.4.1/tests/test_level4/test_any_link.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_attribute.py` & `soupsieve-2.4.1/tests/test_level4/test_attribute.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,31 @@
         self.assert_selector(
             self.MARKUP,
             "[class*=WORDS i]",
             ["0", "3", "pre"],
             flags=util.HTML
         )
 
+    def test_attribute_case_insensitive_flag_spacing(self):
+        """Test attribute value case insensitivity spacing."""
+
+        self.assert_selector(
+            self.MARKUP,
+            "[class*=WORDSi]",
+            [],
+            flags=util.HTML
+        )
+
+        self.assert_selector(
+            self.MARKUP,
+            "[class*='WORDS'i]",
+            ["0", "3", "pre"],
+            flags=util.HTML
+        )
+
     def test_attribute_forced_case_insensitive_xml(self):
         """Test that attribute value case insensitivity can be forced in XML."""
 
         self.assert_selector(
             self.MARKUP,
             '[type="test" i]',
             ['0', '2'],
```

### Comparing `soupsieve-2.4/tests/test_level4/test_current.py` & `soupsieve-2.4.1/tests/test_level4/test_current.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_default.py` & `soupsieve-2.4.1/tests/test_level4/test_default.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_defined.py` & `soupsieve-2.4.1/tests/test_level4/test_defined.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_dir.py` & `soupsieve-2.4.1/tests/test_level4/test_dir.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_focus_visible.py` & `soupsieve-2.4.1/tests/test_level4/test_focus_visible.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_focus_within.py` & `soupsieve-2.4.1/tests/test_level4/test_focus_within.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_future.py` & `soupsieve-2.4.1/tests/test_level4/test_future.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_has.py` & `soupsieve-2.4.1/tests/test_level4/test_has.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_host.py` & `soupsieve-2.4.1/tests/test_level4/test_host.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_in_range.py` & `soupsieve-2.4.1/tests/test_level4/test_in_range.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_indeterminate.py` & `soupsieve-2.4.1/tests/test_level4/test_indeterminate.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_is.py` & `soupsieve-2.4.1/tests/test_level4/test_is.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_lang.py` & `soupsieve-2.4.1/tests/test_level4/test_lang.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_local_link.py` & `soupsieve-2.4.1/tests/test_level4/test_local_link.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_matches.py` & `soupsieve-2.4.1/tests/test_level4/test_matches.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_not.py` & `soupsieve-2.4.1/tests/test_level4/test_not.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_nth_child.py` & `soupsieve-2.4.1/tests/test_level4/test_nth_child.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_nth_last_child.py` & `soupsieve-2.4.1/tests/test_level4/test_nth_last_child.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_optional.py` & `soupsieve-2.4.1/tests/test_level4/test_optional.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_out_of_range.py` & `soupsieve-2.4.1/tests/test_level4/test_out_of_range.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_past.py` & `soupsieve-2.4.1/tests/test_level4/test_past.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_paused.py` & `soupsieve-2.4.1/tests/test_level4/test_paused.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_placeholder_shown.py` & `soupsieve-2.4.1/tests/test_level4/test_placeholder_shown.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_playing.py` & `soupsieve-2.4.1/tests/test_level4/test_playing.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_read_only.py` & `soupsieve-2.4.1/tests/test_level4/test_read_only.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_read_write.py` & `soupsieve-2.4.1/tests/test_level4/test_read_write.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_required.py` & `soupsieve-2.4.1/tests/test_level4/test_required.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_scope.py` & `soupsieve-2.4.1/tests/test_level4/test_scope.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_target_within.py` & `soupsieve-2.4.1/tests/test_level4/test_target_within.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_user_invalid.py` & `soupsieve-2.4.1/tests/test_level4/test_user_invalid.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/tests/test_level4/test_where.py` & `soupsieve-2.4.1/tests/test_level4/test_where.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/.gitignore` & `soupsieve-2.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/LICENSE.md` & `soupsieve-2.4.1/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 - 2022 Isaac Muse <isaacmuse@gmail.com>
+Copyright (c) 2018 - 2023 Isaac Muse <isaacmuse@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `soupsieve-2.4/README.md` & `soupsieve-2.4.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: soupsieve
+Version: 2.4.1
+Summary: A modern CSS selector implementation for Beautiful Soup.
+Project-URL: Homepage, https://github.com/facelessuser/soupsieve
+Author-email: Isaac Muse <Isaac.Muse@gmail.com>
+License-Expression: MIT
+License-File: LICENSE.md
+Keywords: CSS,HTML,XML,filter,query,selector,soup
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 [![Donate via PayPal][donate-image]][donate-link]
 [![Discord][discord-image]][discord-link]
 [![Build][github-ci-image]][github-ci-link]
 [![Coverage Status][codecov-image]][codecov-link]
 [![PyPI Version][pypi-image]][pypi-link]
 [![PyPI Downloads][pypi-down]][pypi-link]
 [![PyPI - Python Version][python-image]][pypi-link]
@@ -67,30 +93,15 @@
 
 ## Documentation
 
 Documentation is found here: https://facelessuser.github.io/soupsieve/.
 
 ## License
 
-MIT License
-
-Copyright (c) 2018 - 2022 Isaac Muse <isaacmuse@gmail.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
-persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
-Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
-WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
-OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+MIT
 
 [bs4]: https://beautiful-soup-4.readthedocs.io/en/latest/#
 
 [github-ci-image]: https://github.com/facelessuser/soupsieve/workflows/build/badge.svg?branch=master&event=push
 [github-ci-link]: https://github.com/facelessuser/soupsieve/actions?query=workflow%3Abuild+branch%3Amaster
 [discord-image]: https://img.shields.io/discord/678289859768745989?logo=discord&logoColor=aaaaaa&color=mediumpurple&labelColor=333333
 [discord-link]:https://discord.gg/XBnPUZF
```

### Comparing `soupsieve-2.4/hatch_build.py` & `soupsieve-2.4.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `soupsieve-2.4/pyproject.toml` & `soupsieve-2.4.1/pyproject.toml`

 * *Files identical despite different names*

