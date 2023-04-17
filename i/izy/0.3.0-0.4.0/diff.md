# Comparing `tmp/izy-0.3.0.tar.gz` & `tmp/izy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izy-0.3.0.tar", last modified: Mon Mar 27 19:14:49 2023, max compression
+gzip compressed data, was "izy-0.4.0.tar", last modified: Mon Apr 17 10:50:53 2023, max compression
```

## Comparing `izy-0.3.0.tar` & `izy-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 19:14:49.144603 izy-0.3.0/
--rw-rw-rw-   0        0        0     1090 2021-12-30 20:14:03.000000 izy-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       43 2022-01-09 09:22:38.000000 izy-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0    16944 2023-03-27 19:14:49.143499 izy-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    16260 2023-03-27 19:08:49.000000 izy-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 19:14:49.117496 izy-0.3.0/izy/
--rw-rw-rw-   0        0        0      173 2023-03-27 10:36:56.000000 izy-0.3.0/izy/__init__.py
--rw-rw-rw-   0        0        0       21 2023-03-27 19:09:22.000000 izy-0.3.0/izy/__version__.py
--rw-rw-rw-   0        0        0     5439 2023-03-27 18:53:50.000000 izy-0.3.0/izy/bidict.py
--rw-rw-rw-   0        0        0     6280 2023-03-27 18:54:10.000000 izy-0.3.0/izy/decorators.py
--rw-rw-rw-   0        0        0     4722 2023-03-27 10:17:48.000000 izy-0.3.0/izy/discovery.py
--rw-rw-rw-   0        0        0     3765 2023-03-27 11:37:14.000000 izy-0.3.0/izy/misc.py
--rw-rw-rw-   0        0        0    19975 2023-03-27 11:28:22.000000 izy-0.3.0/izy/path.py
--rw-rw-rw-   0        0        0     5812 2023-03-27 19:07:33.000000 izy-0.3.0/izy/regex.py
--rw-rw-rw-   0        0        0     8697 2023-03-27 11:36:43.000000 izy-0.3.0/izy/scorer.py
--rw-rw-rw-   0        0        0     3575 2023-03-27 11:35:55.000000 izy-0.3.0/izy/sorting.py
--rw-rw-rw-   0        0        0     9246 2023-03-27 11:36:24.000000 izy-0.3.0/izy/table.py
-drwxrwxrwx   0        0        0        0 2023-03-27 19:14:49.142495 izy-0.3.0/izy.egg-info/
--rw-rw-rw-   0        0        0    16944 2023-03-27 19:14:48.000000 izy-0.3.0/izy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-03-27 19:14:48.000000 izy-0.3.0/izy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 19:14:48.000000 izy-0.3.0/izy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-03-27 19:14:48.000000 izy-0.3.0/izy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 19:14:49.144603 izy-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     3908 2023-03-27 19:09:22.000000 izy-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:50:53.481352 izy-0.4.0/
+-rw-rw-rw-   0        0        0     1090 2021-12-30 20:14:03.000000 izy-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       43 2022-01-09 09:22:38.000000 izy-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    16944 2023-04-17 10:50:53.481352 izy-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16260 2023-03-27 19:08:49.000000 izy-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 10:50:53.450099 izy-0.4.0/izy/
+-rw-rw-rw-   0        0        0      173 2023-03-27 10:36:56.000000 izy-0.4.0/izy/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-04-17 10:48:55.000000 izy-0.4.0/izy/__version__.py
+-rw-rw-rw-   0        0        0     5439 2023-04-16 21:13:45.000000 izy-0.4.0/izy/bidict.py
+-rw-rw-rw-   0        0        0    13199 2023-04-17 10:36:24.000000 izy-0.4.0/izy/decorators.py
+-rw-rw-rw-   0        0        0     4722 2023-03-27 10:17:48.000000 izy-0.4.0/izy/discovery.py
+-rw-rw-rw-   0        0        0     3765 2023-03-27 11:37:14.000000 izy-0.4.0/izy/misc.py
+-rw-rw-rw-   0        0        0    19975 2023-03-27 11:28:22.000000 izy-0.4.0/izy/path.py
+-rw-rw-rw-   0        0        0     8709 2023-04-10 22:32:43.000000 izy-0.4.0/izy/regex.py
+-rw-rw-rw-   0        0        0     8697 2023-03-27 11:36:43.000000 izy-0.4.0/izy/scorer.py
+-rw-rw-rw-   0        0        0     3575 2023-03-27 11:35:55.000000 izy-0.4.0/izy/sorting.py
+-rw-rw-rw-   0        0        0     9246 2023-03-27 11:36:24.000000 izy-0.4.0/izy/table.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:50:53.481352 izy-0.4.0/izy.egg-info/
+-rw-rw-rw-   0        0        0    16944 2023-04-17 10:50:53.000000 izy-0.4.0/izy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-04-17 10:50:53.000000 izy-0.4.0/izy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:50:53.000000 izy-0.4.0/izy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-17 10:50:53.000000 izy-0.4.0/izy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:50:53.481352 izy-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     3908 2023-04-17 10:48:55.000000 izy-0.4.0/setup.py
```

### Comparing `izy-0.3.0/LICENSE` & `izy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `izy-0.3.0/PKG-INFO` & `izy-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python functions and classes that make it even easier!
 Home-page: https://github.com/tabasy/izy
 Author: Mohsen Tabasi
 Author-email: m.tabasy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `izy-0.3.0/README.md` & `izy-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `izy-0.3.0/izy/bidict.py` & `izy-0.4.0/izy/bidict.py`

 * *Files identical despite different names*

### Comparing `izy-0.3.0/izy/discovery.py` & `izy-0.4.0/izy/discovery.py`

 * *Files identical despite different names*

### Comparing `izy-0.3.0/izy/misc.py` & `izy-0.4.0/izy/misc.py`

 * *Files identical despite different names*

### Comparing `izy-0.3.0/izy/path.py` & `izy-0.4.0/izy/path.py`

 * *Files identical despite different names*

### Comparing `izy-0.3.0/izy/regex.py` & `izy-0.4.0/izy/regex.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,90 @@
 """Regular expression helper functions.
 
 >>> p = make_regex(
 ...    following('then '),      # lookbehind
-...    charset('a-z '), '+',
-...    followed_by(r' end')     # lookahead
+...    grouped(r'[a-z ]+', name='code'),
+...    followed_by(r' end'),     # lookahead
 ...    )
 >>> p.pattern
-'(?<=then )[a-z ]+(?= end)'
+'(?<=then )(?P<code>[a-z ]+)(?= end)'
 >>> p.search('if condition then do something end; etc')
 <re.Match object; span=(18, 30), match='do something'>
 
 >>> p = make_regex(
 ...    any_of('ali', 'hossein', 'javad'),
-...    '\s+',
-...    grouped(any_of('goodarzi', 'sharafi'), name='family')
+...    SPACES,
+...    any_of('goodarzi', 'sharafi', name='family')
 ...    )
 >>> p.pattern
-'(?:hossein|javad|ali)\\\\s+(?P<family>(?:goodarzi|sharafi))'
+'(?:hossein|javad|ali)\\\\s+(?P<family>goodarzi|sharafi)'
 >>> match = p.search('his name is hossein sharafi.')
 >>> match
 <re.Match object; span=(12, 27), match='hossein sharafi'>
 >>> match.group('family')
 'sharafi'
+
+>>> p = make_regex(
+...    any_of(
+...        grouped('<p>', name='p'),
+...        grouped('<div>', name='div'),
+...        name='tag'
+...    ),
+...    repeated('.', greedy=False, name='inside'), 
+...    if_matched('p', then='</p>', otherwise='</div>')
+...    )
+>>> p.pattern        # this is really hard to read
+'(?P<tag>(?P<div><div>)|(?P<p><p>))(?P<inside>(?:.)+?)(?(p)</p>|</div>)'
+>>> text = '<div><p>hello world!</p></div><p>good morning...</p><div>bye!</div>'
+>>> for m in p.finditer(text):
+...     print(m.group('tag'), m.group('inside'))
+<div> <p>hello world!</p>
+<p> good morning...
+<div> bye!
+
+>>> p = make_regex('[0-9]')
+>>> p.sub(repl({'1': 'one', '2': 'two'}), '2 and a half.')
+'two and a half.'
+
+>>> p = make_regex('[0-9()\-+/*]{3,}')
+>>> p.sub(repl(eval), 'It costs 25*4+10 for you.')
+'It costs 110 for you.'
 """
 
 import re
 from operator import ior
 from typing import Mapping
 from functools import reduce
 
 
-__all__ = ['make_regex', 'grouped', 'if_matched',
+__all__ = ['join_patterns', 'make_regex', 'grouped', 
+           'atomic', 'if_matched',
            'followed_by', 'not_followed_by',
            'following', 'not_following', 
            'preceded_by', 'not_preceded_by', 
            'lookahead', 'neg_lookahead',
            'lookbehind', 'neg_lookbehind',
+           'repeated', 'possibly',
            'wordbounded', 'any_of', 'charset', 'any_char_but',
            'bag_of_patterns',
            'map2repl', 'func2repl', 'repl', 
+           'SPACES', 'DIGITS', 'DOT', 'BOS', 'EOS', 'BOL', 'EOL',
            ]
 
+
+SPACES = r'\s+'
+DIGITS = r'\d+'
+
+DOT = r'\.'
+BOS = r'\A'
+EOS = r'\Z'
+BOL = r'^'
+EOL = r'$'
+
+
 def join_patterns(*patterns, joiner=''):
     if len(patterns) == 1 and not isinstance(patterns[0], str):
         patterns = patterns[0]
     return joiner.join(patterns)
 
 
 def make_regex(*patterns, ascii=False, debug=False, ignorecase=False,
@@ -70,14 +110,24 @@
     if name:
         return fr'(?P<{name}>{pattern})'
     if no_capture:
         return fr'(?:{pattern})'
 
     return fr'({pattern})'
 
+# special groups
+
+def atomic(*pattern):
+    pattern = join_patterns(pattern)
+    return fr'(?>{pattern})'
+
+
+def if_matched(group_name, *, then, otherwise=''):
+    return fr'(?({group_name}){then}|{otherwise})'
+
 
 def followed_by(*pattern, immediately=True):
     pattern = join_patterns(pattern)
     prefix = '' if immediately else '.*'
     return fr'(?={prefix}{pattern})'
 
 
@@ -102,39 +152,80 @@
 
 lookahead = followed_by
 neg_lookahead = not_followed_by
 lookbehind = preceded_by
 neg_lookbehind = not_preceded_by
 
 
-def wordbounded(*pattern):
-    pattern = join_patterns(pattern)
-    return fr'\b{pattern}\b'
+# extras
 
+def repeated(*pattern, n=None, min=1, max=None, greedy=True, possessive=False, name=None):
+    """Repeated pattern
+
+    Args:
+        n (int, optional): Exact number of repetitions. If provided, `min`, `max` are ignored. Defaults to None.
+        min (int, optional): Minimum number of repetitions. Defaults to 1.
+        max (int, optional): Maximum number of repetitions. Defaults to None.
+        greedy (bool, optional): Match as much as possible? Defaults to True.
+        possessive (bool, optional): Do not backtrack after maching greedily? Defaults to False.
+        name (str, optional): The name of pattern group. if None, a non-capturing group is used. Defaults to None.
+
+    """
+    if n is not None:
+        return grouped(*pattern, name=name, no_capture=True) + fr'{{{n}}}'
+    
+    min_reps = str(min) if min else ''
+    max_reps = str(max) if max else ''
+    
+    special = ''
+    if not greedy:
+        special = '?'
+    elif possessive:
+        special = '+'
+    
+    repeats = fr'{{{min_reps},{max_reps}}}'
+    repeats = repeats.replace('{1,}', '+')
+    repeats = repeats.replace('{,}', '*')
+    repeats = repeats.replace('{,1}', '?')
+    
+    pattern = grouped(*pattern, no_capture=True) + fr'{repeats}{special}'
+    
+    if name:
+        return grouped(pattern, name=name)
+    return pattern
 
-def if_matched(group_name, *, then, otherwise=''):
-    pattern = join_patterns(pattern)
-    return fr'(?({group_name}){then}|{otherwise})'
 
+def possibly(*pattern, name=None):
+    return grouped(pattern, name=name, no_capture=True) + '?'
 
-def any_of(*patterns, sort=True):
+
+def wordbounded(*pattern, name=None):
+    pattern = join_patterns(r'\b', *pattern, r'\b')
+    if name:
+        return grouped(pattern, name=name)
+    return pattern
+
+
+def any_of(*patterns, sort=True, name=None):
     """Makes the pattern to match any of the input patterns (using `|`). Optionally,
     sorts the patterns starting from the longest to prioritize for the longest. But
     this only works for fixed-length patterns, as the lenght of dynamic patterns 
     cannot be determined.
 
     Args:
         patterns (Iterable): The input patterns.
         sort (bool, optional): Whether or not to sort the patterns starting from the longest. Defaults to True.
+        name (str, optional): The name of pattern group. if None, a non-capturing group is used. Defaults to None.
     """
     if len(patterns) == 1 and not isinstance(patterns[0], str):
         patterns = patterns[0]
     if sort:
         patterns = sorted(patterns, key=len, reverse=True)
-    return grouped(r'|'.join(patterns), no_capture=True)
+
+    return grouped(r'|'.join(patterns), name=name, no_capture=True)
 
 
 def charset(characters: str):
     return fr'[{characters}]'
 
 
 def any_char_but(characters: str):
@@ -149,45 +240,46 @@
         patterns (Iterable): The input patterns.
     """
     if len(patterns) == 1 and not isinstance(patterns[0], str):
         patterns = patterns[0]
     return ''.join(followed_by(p, immediately=False) for p in patterns)
 
 
+# repl maker
 
 def func2repl(fn, group=0):
-    """Converts a str to str function, to a valid `repl` argument for `re.sub()`.
+    """Converts a str-to-str function, to a valid `repl` argument for `re.sub()`.
 
     Args:
         fn (function): A str to str function.
         group (int, optional): The match group to pass to the function. Defaults to 0.
     """
     def repl_func(match):
-        return fn(match.group(group))
+        return str(fn(match.group(group)))
     return repl_func
 
 
 def map2repl(mapping: Mapping, group=0, default_str=''):
-    """Converts a str to str mapping, to a valid `repl` argument for `re.sub()`.
+    """Converts a str-to-str mapping, to a valid `repl` argument for `re.sub()`.
 
     Args:
         mapping (_type_): _description_
         group (int, optional): The match group to pass to the function. Defaults to 0.
         default_str (str, optional): _description_. Defaults to ''.
     """
     def repl_func(match):
-        return mapping.get(match.group(group), default_str)
+        return str(mapping.get(match.group(group), default_str))
     return repl_func
 
 
 def repl(rep, group=0):
     if isinstance(rep, Mapping):
         return map2repl(rep, group=group)
     elif callable(rep):
-        func2repl(rep, group=group)
+        return func2repl(rep, group=group)
     else:
         raise ValueError(
             'Provide a `Callable` or `Mapping` to make a repl function')
 
 
 if __name__ == '__main__':
     import doctest
```

### Comparing `izy-0.3.0/izy/scorer.py` & `izy-0.4.0/izy/scorer.py`

 * *Files identical despite different names*

### Comparing `izy-0.3.0/izy/sorting.py` & `izy-0.4.0/izy/sorting.py`

 * *Files identical despite different names*

### Comparing `izy-0.3.0/izy/table.py` & `izy-0.4.0/izy/table.py`

 * *Files identical despite different names*

### Comparing `izy-0.3.0/izy.egg-info/PKG-INFO` & `izy-0.4.0/izy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python functions and classes that make it even easier!
 Home-page: https://github.com/tabasy/izy
 Author: Mohsen Tabasi
 Author-email: m.tabasy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `izy-0.3.0/setup.py` & `izy-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Package meta-data
 NAME = 'izy'
 DESCRIPTION = 'Python functions and classes that make it even easier!'
 URL = 'https://github.com/tabasy/izy'
 EMAIL = 'm.tabasy@gmail.com'
 AUTHOR = 'Mohsen Tabasi'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.0'
+VERSION = '0.4.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

