# Comparing `tmp/tkblock-1.0.0.tar.gz` & `tmp/tkblock-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkblock-1.0.0.tar", last modified: Thu Mar 16 16:14:59 2023, max compression
+gzip compressed data, was "tkblock-1.1.0.tar", last modified: Mon Apr 17 10:49:37 2023, max compression
```

## Comparing `tkblock-1.0.0.tar` & `tkblock-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 16:14:59.511906 tkblock-1.0.0/
--rw-rw-rw-   0        0        0     1077 2023-03-07 11:27:05.000000 tkblock-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    14315 2023-03-16 16:14:59.509905 tkblock-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    13610 2023-03-16 16:09:16.000000 tkblock-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-16 16:14:59.511906 tkblock-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1017 2023-03-16 16:14:57.000000 tkblock-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-16 16:14:59.489956 tkblock-1.0.0/tkblock/
--rw-rw-rw-   0        0        0      225 2023-03-14 16:09:02.000000 tkblock-1.0.0/tkblock/__init__.py
--rw-rw-rw-   0        0        0      488 2023-03-07 11:43:33.000000 tkblock-1.0.0/tkblock/block_framebase.py
--rw-rw-rw-   0        0        0    19550 2023-03-16 13:07:05.000000 tkblock-1.0.0/tkblock/block_framework.py
--rw-rw-rw-   0        0        0     5894 2023-03-16 00:17:20.000000 tkblock-1.0.0/tkblock/block_service.py
--rw-rw-rw-   0        0        0      426 2023-03-07 11:43:37.000000 tkblock-1.0.0/tkblock/block_util.py
--rw-rw-rw-   0        0        0     1418 2023-03-07 11:43:40.000000 tkblock-1.0.0/tkblock/canvas.py
--rw-rw-rw-   0        0        0      494 2023-03-07 11:43:38.000000 tkblock-1.0.0/tkblock/layout.py
--rw-rw-rw-   0        0        0      368 2023-03-16 12:45:43.000000 tkblock-1.0.0/tkblock/scrollbar.py
-drwxrwxrwx   0        0        0        0 2023-03-16 16:14:59.505913 tkblock-1.0.0/tkblock.egg-info/
--rw-rw-rw-   0        0        0    14315 2023-03-16 16:14:59.000000 tkblock-1.0.0/tkblock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-03-16 16:14:59.000000 tkblock-1.0.0/tkblock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 16:14:59.000000 tkblock-1.0.0/tkblock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-16 16:14:59.000000 tkblock-1.0.0/tkblock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 10:49:37.648985 tkblock-1.1.0/
+-rw-rw-rw-   0        0        0     1077 2023-03-07 11:27:05.000000 tkblock-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0    14133 2023-04-17 10:49:37.647988 tkblock-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13433 2023-04-17 09:10:12.000000 tkblock-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:49:37.649983 tkblock-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2023-04-17 10:49:30.000000 tkblock-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:49:37.618079 tkblock-1.1.0/tkblock/
+-rw-rw-rw-   0        0        0      225 2023-03-14 16:09:02.000000 tkblock-1.1.0/tkblock/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-03-17 02:44:56.000000 tkblock-1.1.0/tkblock/block_framebase.py
+-rw-rw-rw-   0        0        0    21260 2023-04-17 10:11:19.000000 tkblock-1.1.0/tkblock/block_framework.py
+-rw-rw-rw-   0        0        0     6263 2023-04-17 10:43:14.000000 tkblock-1.1.0/tkblock/block_service.py
+-rw-rw-rw-   0        0        0      426 2023-03-16 16:16:54.000000 tkblock-1.1.0/tkblock/block_util.py
+-rw-rw-rw-   0        0        0     1418 2023-03-16 16:16:54.000000 tkblock-1.1.0/tkblock/canvas.py
+-rw-rw-rw-   0        0        0      494 2023-03-16 16:16:54.000000 tkblock-1.1.0/tkblock/layout.py
+-rw-rw-rw-   0        0        0      368 2023-03-16 16:16:54.000000 tkblock-1.1.0/tkblock/scrollbar.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:49:37.644995 tkblock-1.1.0/tkblock.egg-info/
+-rw-rw-rw-   0        0        0    14133 2023-04-17 10:49:37.000000 tkblock-1.1.0/tkblock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-04-17 10:49:37.000000 tkblock-1.1.0/tkblock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:49:37.000000 tkblock-1.1.0/tkblock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 10:49:37.000000 tkblock-1.1.0/tkblock.egg-info/top_level.txt
```

### Comparing `tkblock-1.0.0/LICENSE` & `tkblock-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkblock-1.0.0/PKG-INFO` & `tkblock-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 1.0.0
+Version: 1.1.0
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
@@ -88,15 +88,14 @@
 + width: The width of the frame. If not specified, it is the width of the destination window. In this case, 600  
 + height: The height of the frame. If not specified, it is the height of the destination window. In this case, it is 400  
 + root: The window where the frame will be placed. If not specified, the placement destination is the root window. In this case, the root window.  
 
 By the way, to make it easier to see the table layout during development, a canvas is created internally to draw auxiliary lines.  
 ```python
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 ```
 You can draw an auxiliary line by executing the above code.  
 
 ``BlockService.place_frame_widget()``  
 is explained in the next section.  
 
 <img width="451" alt="readme_frame" src="https://user-images.githubusercontent.com/78261582/223762159-000cbd81-562e-4014-a8cf-8fa8a6d9d443.png">  
@@ -149,26 +148,24 @@
 from tkblock.block_service import BlockService
 
 root = BlockService.init("test", 10, 20, 600, 400)
 frame = BlockService.create_frame("test")
 label = ttk.Label(frame, text="how to use", anchor=tk.CENTER)
 label.layout = BlockService.layout(3, 6, 2, 4)
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 root.mainloop()
 ```
 
 BlockService's in the tkblock library.  
 + init  
 + create_frame  
 + layout  
-+ place_frame_widget  
 You can easily use tkinter Widget just by using.  
 
-<img width="898" alt="readme_layout3" src="https://user-images.githubusercontent.com/78261582/225677201-75f12fa3-1021-4a15-b039-dfb3e4b1fd84.png">
+<img width="897" alt="readme_widget" src="https://user-images.githubusercontent.com/78261582/225685418-ea328480-f051-4617-a459-d7af68ca8d5d.png">
 
 In this figure, several Widget are placed in the above basic usage.  
 Please try to create an application by placing various widgets.  
 
 ## About Layout padding settings
 
 From here, I will explain a few details about the settings.  
@@ -236,15 +233,14 @@
 ```python
 root = BlockService.init("test_frame", 10, 10, 600, 400)
 frame1 = BlockService.create_frame("test_frame1", col=5, row=5)
 frame1.layout = BlockService.layout(1, 9, 1, 9)
 frame2 = BlockService.create_frame("test_frame2", col=3, row=3, root=frame1)
 frame2.layout = BlockService.layout(1, 3, 2, 4)
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 root.mainloop()
 ```
 
 In this code, test_frame1 is placed at coordinates (1,1)(9,9) of root, and  
 test_frame2 is placed at coordinates (1,2)(3,4) of test_frame1.  
 The table structure of each frame is also changed.  
 In this way, a dedicated Frame can be placed on top of a dedicated Frame, which is useful when you want to group Widgets together.  
@@ -296,15 +292,14 @@
 scrollbar_x = tk.Scrollbar(frame, orient=tk.HORIZONTAL)
 scrollbar_y.config(command=listbox.yview)
 scrollbar_x.config(command=listbox.xview)
 listbox.config(yscrollcommand=scrollbar_y.set)
 listbox.config(xscrollcommand=scrollbar_x.set)
 listbox.scrollbar = BlockService.scrollbar(y=scrollbar_y, x=scrollbar_x, size=30)
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 root.mainloop()
 ```
 
 The basic usage of the scrollbar is the same. If you want the scrollbar to be placed automatically, you can place it by linking the scrollbar to the widget.  
 If you wish to manually place it anywhere you wish, simply specify the layout as you would for a normal widget.  
 
 ## How to use the Menu bar
```

### Comparing `tkblock-1.0.0/README.md` & `tkblock-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 + width: The width of the frame. If not specified, it is the width of the destination window. In this case, 600  
 + height: The height of the frame. If not specified, it is the height of the destination window. In this case, it is 400  
 + root: The window where the frame will be placed. If not specified, the placement destination is the root window. In this case, the root window.  
 
 By the way, to make it easier to see the table layout during development, a canvas is created internally to draw auxiliary lines.  
 ```python
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 ```
 You can draw an auxiliary line by executing the above code.  
 
 ``BlockService.place_frame_widget()``  
 is explained in the next section.  
 
 <img width="451" alt="readme_frame" src="https://user-images.githubusercontent.com/78261582/223762159-000cbd81-562e-4014-a8cf-8fa8a6d9d443.png">  
@@ -135,26 +134,24 @@
 from tkblock.block_service import BlockService
 
 root = BlockService.init("test", 10, 20, 600, 400)
 frame = BlockService.create_frame("test")
 label = ttk.Label(frame, text="how to use", anchor=tk.CENTER)
 label.layout = BlockService.layout(3, 6, 2, 4)
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 root.mainloop()
 ```
 
 BlockService's in the tkblock library.  
 + init  
 + create_frame  
 + layout  
-+ place_frame_widget  
 You can easily use tkinter Widget just by using.  
 
-<img width="898" alt="readme_layout3" src="https://user-images.githubusercontent.com/78261582/225677201-75f12fa3-1021-4a15-b039-dfb3e4b1fd84.png">
+<img width="897" alt="readme_widget" src="https://user-images.githubusercontent.com/78261582/225685418-ea328480-f051-4617-a459-d7af68ca8d5d.png">
 
 In this figure, several Widget are placed in the above basic usage.  
 Please try to create an application by placing various widgets.  
 
 ## About Layout padding settings
 
 From here, I will explain a few details about the settings.  
@@ -222,15 +219,14 @@
 ```python
 root = BlockService.init("test_frame", 10, 10, 600, 400)
 frame1 = BlockService.create_frame("test_frame1", col=5, row=5)
 frame1.layout = BlockService.layout(1, 9, 1, 9)
 frame2 = BlockService.create_frame("test_frame2", col=3, row=3, root=frame1)
 frame2.layout = BlockService.layout(1, 3, 2, 4)
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 root.mainloop()
 ```
 
 In this code, test_frame1 is placed at coordinates (1,1)(9,9) of root, and  
 test_frame2 is placed at coordinates (1,2)(3,4) of test_frame1.  
 The table structure of each frame is also changed.  
 In this way, a dedicated Frame can be placed on top of a dedicated Frame, which is useful when you want to group Widgets together.  
@@ -282,15 +278,14 @@
 scrollbar_x = tk.Scrollbar(frame, orient=tk.HORIZONTAL)
 scrollbar_y.config(command=listbox.yview)
 scrollbar_x.config(command=listbox.xview)
 listbox.config(yscrollcommand=scrollbar_y.set)
 listbox.config(xscrollcommand=scrollbar_x.set)
 listbox.scrollbar = BlockService.scrollbar(y=scrollbar_y, x=scrollbar_x, size=30)
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 root.mainloop()
 ```
 
 The basic usage of the scrollbar is the same. If you want the scrollbar to be placed automatically, you can place it by linking the scrollbar to the widget.  
 If you wish to manually place it anywhere you wish, simply specify the layout as you would for a normal widget.  
 
 ## How to use the Menu bar
```

### Comparing `tkblock-1.0.0/setup.py` & `tkblock-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 # README.mdをlong_discriptionにするために読み込む
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name=package_name,
-    version="1.0.0",
+    version="1.1.0",
     description="tkinter block framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kuri-pome/tkblock",
     author="kuri_pome",
     license="MIT",
     keywords="tkinter place widget easy",
```

### Comparing `tkblock-1.0.0/tkblock/block_framework.py` & `tkblock-1.1.0/tkblock/block_framework.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,30 +57,34 @@
 class BlockFramework(tk.Tk):
     """WidgetをBlock形式で指定することで配置操作を行うためのFramework
 
     Args:
         tk (tk.Tk): tk.Tk
     """
 
-    def __init__(self, max_col: int, max_row: int, width: int, height: int) -> None:
+    def __init__(
+        self, max_col: int, max_row: int, width: int, height: int, is_debug=False
+    ) -> None:
         """コンストラクタ
 
         Args:
             max_col (int): 分割を行う行数
             max_row (int): 分割を行う列数
             width (int): frameの横幅
             height (int): frameの縦幅
+            is_debug (bool, optional): デバッグモードならTrue
         """
 
         super().__init__()
         self.max_col: int = max_col
         self.max_row: int = max_row
         self.width: int = width
         self.height: int = height
         self._name: str = "main"
+        self.is_debug: bool = is_debug
         super().geometry(f"{width}x{height}")
 
     def _override_valiable(
         self, default_valiable: Any, attribute_name: str, class_object: Any
     ) -> Any:
         """値の上書きリターン
 
@@ -316,23 +320,29 @@
         # objcetが最初に置く対象のクラスなら終了
         if widget.__class__.__name__ not in PLACE_TARGET_OBJECTS:
             raise Exception(f"cannot place object error: {widget.__class__.__name__}")
         # layout属性を持っていないなら終了
         # Frameの下に直接配置しているものはここでreturn
         if not ("layout" in dir(widget)):
             return
+
         if hasattr(widget, "scrollbar"):
             x_size: int = 0
             y_size: int = 0
             if widget.scrollbar.x is not None:
                 # x軸のスクロールバーがないということは、y軸つまり高さのサイズは調整しない
                 y_size = widget.scrollbar.size
+                widget.scrollbar.x.config(command=widget.xview)
+                widget.config(xscrollcommand=widget.scrollbar.x.set)
             if widget.scrollbar.y is not None:
                 # y軸のスクロールバーがないということは、x軸つまり幅のサイズは調整しない
                 x_size = widget.scrollbar.size
+                widget.scrollbar.y.config(command=widget.yview)
+                widget.config(yscrollcommand=widget.scrollbar.y.set)
+
             (
                 widget_values,
                 scrollbar_x_values,
                 scrollbar_y_values,
             ) = self._calc_place_rel_with_scroll(
                 width,
                 height,
@@ -354,24 +364,23 @@
                     height,
                     col_size,
                     row_size,
                     **dataclasses.asdict(widget.layout),
                 )
             )
 
-    def place_frame_widget(self, frame: Any = None) -> None:
+    def _place_frame_widget(self, frame) -> None:
         """Frame上のwidgetを全て配置する。
 
         Layout指定をしている全てのwidgetを配置する。
         この関数は、Frame配下に子Frameを考慮して、再起処理で実現している。
 
         Args:
-            frame (Any, optional): 配置する先のFrame. Defaults to None.
+            frame (Any): 配置する先のFrame. Defaults to None.
         """
-        frame: Any = self if frame is None else frame
         width: int
         height: int
         col_size: float
         row_size: float
         (
             _,
             _,
@@ -403,14 +412,28 @@
                 # 上記以外は、Widgetのみになるので配置処理を実施。
                 self._place_widget(widget, width, height, col_size, row_size)
         # 最後にFrameを最前面に移動しておく。
         for _, widget in frame.children.items():
             if widget.__class__.__name__ in ("Frame", "BlockFrameBase"):
                 widget.tkraise()
 
+    def place_frame_widget(self, frame: Any = None) -> None:
+        """Frame上のwidgetを全て配置する。
+
+        Layout指定をしている全てのwidgetを配置する。
+        この関数は、Frame配下に子Frameを考慮して、再起処理で実現している。
+
+        Args:
+            frame (Any, optional): 配置する先のFrame. Defaults to None.
+        """
+        frame: Any = self if frame is None else frame
+        self._place_frame_widget(frame=frame)
+        if self.is_debug:
+            self._create_auxiliary_line(frame)
+
     def _write_auxiliary_line(self, frame: Any, widget: ResizingCanvas) -> None:
         """debug用に補助線を引く
 
         Args:
             frame (_type_):  Canvasを保持しているFrameまたは、その上位のFrame
             widget (ResizingCanvas): 補助線を引くcanvas
         """
@@ -428,21 +451,37 @@
         for index in range(0, col_num):
             x: int = int(index * col_size)
             widget.create_line(x, start_y, x, end_y)
         for index in range(0, row_num):
             y: int = int(index * row_size)
             widget.create_line(start_x, y, end_x, y)
 
-    def create_auxiliary_line(self, frame: Any = None) -> None:
+    def _create_auxiliary_line(self, frame: Any) -> None:
+        """補助線を作成する
+
+        この関数は、Frame配下に子Frameを考慮して、再起処理で実現している。
+
+        Args:
+            frame (Any, optional): Canvasを保持しているFrameまたは、その上位のFrame. Defaults to None.
+        """
+        for name, widget in frame.children.items():
+            if widget.__class__.__name__ == "ResizingCanvas":
+                self._write_auxiliary_line(frame, widget)
+            if widget.__class__.__name__ in ("Frame", "BlockFrameBase"):
+                self._create_auxiliary_line(widget)
+
+    def create_auxiliary_line(self, frame: Any = None, is_debug=None) -> None:
         """補助線を作成する
 
         この関数は、Frame配下に子Frameを考慮して、再起処理で実現している。
 
         Args:
             frame (Any, optional): Canvasを保持しているFrameまたは、その上位のFrame. Defaults to None.
         """
         frame: Any = self if frame is None else frame
         for name, widget in frame.children.items():
             if widget.__class__.__name__ == "ResizingCanvas":
                 self._write_auxiliary_line(frame, widget)
             if widget.__class__.__name__ in ("Frame", "BlockFrameBase"):
-                self.create_auxiliary_line(widget)
+                is_debug: bool = self.is_debug if is_debug is None else is_debug
+                if is_debug:
+                    self._create_auxiliary_line(widget)
```

### Comparing `tkblock-1.0.0/tkblock/block_service.py` & `tkblock-1.1.0/tkblock/block_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,38 +17,57 @@
 class BlockService:
     """BlockFrameworkを操作するためのクラス"""
 
     root = None
 
     @classmethod
     def init(
-        cls, title: str, max_col: int, max_row: int, width: int, height: int
+        cls,
+        title: str,
+        max_col: int,
+        max_row: int,
+        width: int,
+        height: int,
+        is_debug=False,
     ) -> BlockFramework:
         """コンストラクタ
 
         Args:
             title (str): rootのタイトル名
             max_col (int): defaultとなる分割する列数
             max_row (int): defaultとなる分割する行数
             width (int): フレームの横幅
             height (int): フレームの縦幅
+            is_debug (bool, optional): デバッグモードならTrue
 
         Returns:
             BlockFramework: 大本のrootとなるFrameを継承したクラスのインスタンス
         """
-        cls.root: BlockFramework = BlockFramework(max_col, max_row, width, height)
+        cls.root: BlockFramework = BlockFramework(
+            max_col, max_row, width, height, is_debug=is_debug
+        )
         cls.root.grid_rowconfigure(0, weight=1)
         cls.root.grid_columnconfigure(0, weight=1)
         cls.root.title(title)
         return cls.root
 
     @classmethod
-    def place_frame_widget(cls) -> None:
+    def place_frame_widget(cls, frame=None) -> None:
         """root配下のwidgetを配置する"""
-        cls.root.place_frame_widget()
+        frame = cls.root if frame is None else frame
+        cls.root.place_frame_widget(frame=frame)
+
+    @classmethod
+    def create_auxiliary_line(cls, is_debug, frame=None) -> None:
+        """debug用に補助線を作成する関数
+
+        補助線を引かない場合はこの関数をcallしないこと
+        """
+        frame = cls.root if frame is None else frame
+        cls.root.create_auxiliary_line(is_debug=is_debug, frame=frame)
 
     @classmethod
     def create_frame(
         cls,
         frame_name: str,
         col: int = None,
         row: int = None,
@@ -148,15 +167,7 @@
         Returns:
             Scrollbar: Scrollbar
         """
         if size is None:
             return Scrollbar(x, y)
         else:
             return Scrollbar(x, y, size=size)
-
-    @classmethod
-    def create_auxiliary_line(cls) -> None:
-        """debug用に補助線を作成する関数
-
-        補助線を引かない場合はこの関数をcallしないこと
-        """
-        cls.root.create_auxiliary_line()
```

### Comparing `tkblock-1.0.0/tkblock/canvas.py` & `tkblock-1.1.0/tkblock/canvas.py`

 * *Files identical despite different names*

### Comparing `tkblock-1.0.0/tkblock.egg-info/PKG-INFO` & `tkblock-1.1.0/tkblock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 1.0.0
+Version: 1.1.0
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
@@ -88,15 +88,14 @@
 + width: The width of the frame. If not specified, it is the width of the destination window. In this case, 600  
 + height: The height of the frame. If not specified, it is the height of the destination window. In this case, it is 400  
 + root: The window where the frame will be placed. If not specified, the placement destination is the root window. In this case, the root window.  
 
 By the way, to make it easier to see the table layout during development, a canvas is created internally to draw auxiliary lines.  
 ```python
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 ```
 You can draw an auxiliary line by executing the above code.  
 
 ``BlockService.place_frame_widget()``  
 is explained in the next section.  
 
 <img width="451" alt="readme_frame" src="https://user-images.githubusercontent.com/78261582/223762159-000cbd81-562e-4014-a8cf-8fa8a6d9d443.png">  
@@ -149,26 +148,24 @@
 from tkblock.block_service import BlockService
 
 root = BlockService.init("test", 10, 20, 600, 400)
 frame = BlockService.create_frame("test")
 label = ttk.Label(frame, text="how to use", anchor=tk.CENTER)
 label.layout = BlockService.layout(3, 6, 2, 4)
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 root.mainloop()
 ```
 
 BlockService's in the tkblock library.  
 + init  
 + create_frame  
 + layout  
-+ place_frame_widget  
 You can easily use tkinter Widget just by using.  
 
-<img width="898" alt="readme_layout3" src="https://user-images.githubusercontent.com/78261582/225677201-75f12fa3-1021-4a15-b039-dfb3e4b1fd84.png">
+<img width="897" alt="readme_widget" src="https://user-images.githubusercontent.com/78261582/225685418-ea328480-f051-4617-a459-d7af68ca8d5d.png">
 
 In this figure, several Widget are placed in the above basic usage.  
 Please try to create an application by placing various widgets.  
 
 ## About Layout padding settings
 
 From here, I will explain a few details about the settings.  
@@ -236,15 +233,14 @@
 ```python
 root = BlockService.init("test_frame", 10, 10, 600, 400)
 frame1 = BlockService.create_frame("test_frame1", col=5, row=5)
 frame1.layout = BlockService.layout(1, 9, 1, 9)
 frame2 = BlockService.create_frame("test_frame2", col=3, row=3, root=frame1)
 frame2.layout = BlockService.layout(1, 3, 2, 4)
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 root.mainloop()
 ```
 
 In this code, test_frame1 is placed at coordinates (1,1)(9,9) of root, and  
 test_frame2 is placed at coordinates (1,2)(3,4) of test_frame1.  
 The table structure of each frame is also changed.  
 In this way, a dedicated Frame can be placed on top of a dedicated Frame, which is useful when you want to group Widgets together.  
@@ -296,15 +292,14 @@
 scrollbar_x = tk.Scrollbar(frame, orient=tk.HORIZONTAL)
 scrollbar_y.config(command=listbox.yview)
 scrollbar_x.config(command=listbox.xview)
 listbox.config(yscrollcommand=scrollbar_y.set)
 listbox.config(xscrollcommand=scrollbar_x.set)
 listbox.scrollbar = BlockService.scrollbar(y=scrollbar_y, x=scrollbar_x, size=30)
 BlockService.place_frame_widget()
-BlockService.create_auxiliary_line()
 root.mainloop()
 ```
 
 The basic usage of the scrollbar is the same. If you want the scrollbar to be placed automatically, you can place it by linking the scrollbar to the widget.  
 If you wish to manually place it anywhere you wish, simply specify the layout as you would for a normal widget.  
 
 ## How to use the Menu bar
```

