# Comparing `tmp/consoleAnsiInterface-1.0.1.tar.gz` & `tmp/consoleAnsiInterface-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consoleAnsiInterface-1.0.1.tar", last modified: Thu Dec 29 17:07:44 2022, max compression
+gzip compressed data, was "consoleAnsiInterface-1.2.0.tar", last modified: Mon Apr 17 15:39:38 2023, max compression
```

## Comparing `consoleAnsiInterface-1.0.1.tar` & `consoleAnsiInterface-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-12-29 17:07:44.409632 consoleAnsiInterface-1.0.1/
--rw-rw-rw-   0        0        0      145 2022-12-29 17:07:44.409632 consoleAnsiInterface-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-29 17:07:44.394011 consoleAnsiInterface-1.0.1/consoleAnsiInterface/
--rw-rw-rw-   0        0        0     2134 2022-12-29 12:31:43.000000 consoleAnsiInterface-1.0.1/consoleAnsiInterface/__init__.py
--rw-rw-rw-   0        0        0     2134 2022-12-29 12:31:43.000000 consoleAnsiInterface-1.0.1/consoleAnsiInterface/__main__.py
-drwxrwxrwx   0        0        0        0 2022-12-29 17:07:44.409632 consoleAnsiInterface-1.0.1/consoleAnsiInterface.egg-info/
--rw-rw-rw-   0        0        0      145 2022-12-29 17:07:44.000000 consoleAnsiInterface-1.0.1/consoleAnsiInterface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2022-12-29 17:07:44.000000 consoleAnsiInterface-1.0.1/consoleAnsiInterface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-29 17:07:44.000000 consoleAnsiInterface-1.0.1/consoleAnsiInterface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-12-29 17:07:44.000000 consoleAnsiInterface-1.0.1/consoleAnsiInterface.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2022-12-29 17:07:44.000000 consoleAnsiInterface-1.0.1/consoleAnsiInterface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-29 17:07:44.409632 consoleAnsiInterface-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      266 2022-12-29 17:05:12.000000 consoleAnsiInterface-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:39:38.989349 consoleAnsiInterface-1.2.0/
+-rw-rw-rw-   0        0        0      145 2023-04-17 15:39:38.987354 consoleAnsiInterface-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 15:39:38.976384 consoleAnsiInterface-1.2.0/consoleAnsiInterface/
+-rw-rw-rw-   0        0        0     2504 2023-04-17 15:32:47.000000 consoleAnsiInterface-1.2.0/consoleAnsiInterface/__init__.py
+-rw-rw-rw-   0        0        0     2175 2023-03-12 10:47:24.000000 consoleAnsiInterface-1.2.0/consoleAnsiInterface/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:39:38.985359 consoleAnsiInterface-1.2.0/consoleAnsiInterface.egg-info/
+-rw-rw-rw-   0        0        0      145 2023-04-17 15:39:38.000000 consoleAnsiInterface-1.2.0/consoleAnsiInterface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-04-17 15:39:38.000000 consoleAnsiInterface-1.2.0/consoleAnsiInterface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:39:38.000000 consoleAnsiInterface-1.2.0/consoleAnsiInterface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 15:39:38.000000 consoleAnsiInterface-1.2.0/consoleAnsiInterface.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-17 15:39:38.000000 consoleAnsiInterface-1.2.0/consoleAnsiInterface.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:39:38.989349 consoleAnsiInterface-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      266 2023-04-17 15:32:23.000000 consoleAnsiInterface-1.2.0/setup.py
```

### Comparing `consoleAnsiInterface-1.0.1/consoleAnsiInterface/__init__.py` & `consoleAnsiInterface-1.2.0/consoleAnsiInterface/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,19 @@
 def showCursor():
     cursor.show()
 
 def skipGetKey():
     msvcrt.ungetch(b'\0')
     msvcrt.ungetch(b'\0')
 
+def clearScreen():
+    print(_RESET_FORMAT + _CLEAR, end='', file=sys.__stdout__)
+
 k = windll.kernel32
 k.SetConsoleMode(k.GetStdHandle(-11), 7)
 del k
-print(_RESET_FORMAT + _CLEAR, end='', file=sys.__stdout__)
+clearScreen()
 sys.__stdout__.flush()
 
 if __name__ == '__main__':
     w = Window(5, 5)
     w.writeText('Spam', fg=(0, 255, 0), bg=(255, 0, 0), pos=(-2, -2))
```

### Comparing `consoleAnsiInterface-1.0.1/consoleAnsiInterface/__main__.py` & `consoleAnsiInterface-1.2.0/consoleAnsiInterface/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 _MOVE_DOWN = '\033[B'
 _MOVE_LEFT = '\033[D'
 _MOVE_TO = '\033[%(y)d;%(x)dH'
 _FG_24 = '\033[38;2;%d;%d;%dm'
 _BG_24 = '\033[48;2;%d;%d;%dm'
 _RESET_FORMAT = '\033[0m'
 
-UP = '🡡'
-DOWN = '🡣'
-LEFT = '🡠'
-RIGHT = '🡢'
+UP = '❈'
+DOWN = '❐'
+LEFT = '❋'
+RIGHT = '❍'
 
 class Window:
     def __init__(self, x, y):
         self.x = x
         self.y = y
     def writeText(self, text, *, fg: tuple[int]=None, bg: tuple[int]=None, pos=(0, 0)):
         print(_MOVE_TO % {'x':self.x + pos[0] + 1, 'y':self.y + pos[1] + 1}, end='', file=sys.__stdout__)
@@ -30,30 +30,26 @@
               text, _RESET_FORMAT, end=_MOVE_TO % {'x':1, 'y':1}, sep='', file=sys.__stdout__)
         if _SHELL:
             showAll()
 
 def showAll():
     sys.__stdout__.flush()
 
+_buf = []
 def getKey():
-    k = msvcrt.getch()
+    def getch():
+        try:
+            return _buf.pop(0)
+        except IndexError:
+            return msvcrt.getch()
+    k = getch()
     if k == b'\xe0':
-        match k := msvcrt.getch():
-            case b'H':
-                return UP
-            case b'P':
-                return DOWN
-            case b'K':
-                return LEFT
-            case b'M':
-                return RIGHT
-            case _:
-                return chr(0x2700 + k[0])
+        return chr(0x2700 + getch()[0])
     elif k == b'\0':
-        match k := msvcrt.getch():
+        match k := getch():
             case b'\0':
                 return '\0'
             case _:
                 return chr(0x3400 + k[0])
     elif k == b'\3':
         showCursor()
         raise KeyboardInterrupt
@@ -66,16 +62,33 @@
 def showCursor():
     cursor.show()
 
 def skipGetKey():
     msvcrt.ungetch(b'\0')
     msvcrt.ungetch(b'\0')
 
+def unGetKey(key):
+    try:
+        _buf.append(key.encode('852'))
+    except UnicodeEncodeError:
+        match ord(key) >> 8:
+            case 0x27:
+                _buf.append(b'\xe0')
+                _buf.append(bytes([ord(key) & 0xff]))
+            case 0x34:
+                _buf.append(b'\0')
+                _buf.append(bytes([ord(key) & 0xff]))
+            case _:
+                raise ValueError(f'Niedozwolony znak "{key}" ({hex(ord(key))})') from None
+
+def clearScreen():
+    print(_RESET_FORMAT + _CLEAR, end='', file=sys.__stdout__)
+
 k = windll.kernel32
 k.SetConsoleMode(k.GetStdHandle(-11), 7)
 del k
-print(_RESET_FORMAT + _CLEAR, end='', file=sys.__stdout__)
+clearScreen()
 sys.__stdout__.flush()
 
 if __name__ == '__main__':
     w = Window(5, 5)
     w.writeText('Spam', fg=(0, 255, 0), bg=(255, 0, 0), pos=(-2, -2))
```

