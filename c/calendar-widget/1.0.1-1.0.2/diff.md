# Comparing `tmp/calendar_widget-1.0.1.tar.gz` & `tmp/calendar_widget-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar_widget-1.0.1.tar", last modified: Sun Apr 16 14:30:49 2023, max compression
+gzip compressed data, was "calendar_widget-1.0.2.tar", last modified: Mon Apr 17 00:57:39 2023, max compression
```

## Comparing `calendar_widget-1.0.1.tar` & `calendar_widget-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:30:49.478744 calendar_widget-1.0.1/
--rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     5816 2023-04-16 14:30:49.478744 calendar_widget-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4995 2023-04-15 03:23:35.000000 calendar_widget-1.0.1/README.md
--rw-rw-rw-   0        0        0      763 2023-04-16 14:30:02.000000 calendar_widget-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 14:30:49.478744 calendar_widget-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 14:30:49.369363 calendar_widget-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 14:30:49.431869 calendar_widget-1.0.1/src/calendar_widget/
--rw-rw-rw-   0        0        0    32351 2023-04-16 14:28:58.000000 calendar_widget-1.0.1/src/calendar_widget/Calendar_Widget.py
--rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.1/src/calendar_widget/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:30:49.478744 calendar_widget-1.0.1/src/calendar_widget.egg-info/
--rw-rw-rw-   0        0        0     5816 2023-04-16 14:30:49.000000 calendar_widget-1.0.1/src/calendar_widget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-16 14:30:49.000000 calendar_widget-1.0.1/src/calendar_widget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:30:49.000000 calendar_widget-1.0.1/src/calendar_widget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-16 14:30:49.000000 calendar_widget-1.0.1/src/calendar_widget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 00:57:39.949842 calendar_widget-1.0.2/
+-rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0     7068 2023-04-17 00:57:39.949842 calendar_widget-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6215 2023-04-17 00:49:26.000000 calendar_widget-1.0.2/README.md
+-rw-rw-rw-   0        0        0      763 2023-04-17 00:56:24.000000 calendar_widget-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 00:57:39.949842 calendar_widget-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 00:57:39.793580 calendar_widget-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 00:57:39.856085 calendar_widget-1.0.2/src/calendar_widget/
+-rw-rw-rw-   0        0        0    32475 2023-04-17 00:56:16.000000 calendar_widget-1.0.2/src/calendar_widget/Calendar_Widget.py
+-rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.2/src/calendar_widget/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 00:57:39.934221 calendar_widget-1.0.2/src/calendar_widget.egg-info/
+-rw-rw-rw-   0        0        0     7068 2023-04-17 00:57:39.000000 calendar_widget-1.0.2/src/calendar_widget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-17 00:57:39.000000 calendar_widget-1.0.2/src/calendar_widget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 00:57:39.000000 calendar_widget-1.0.2/src/calendar_widget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-17 00:57:39.000000 calendar_widget-1.0.2/src/calendar_widget.egg-info/top_level.txt
```

### Comparing `calendar_widget-1.0.1/LICENSE.md` & `calendar_widget-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `calendar_widget-1.0.1/PKG-INFO` & `calendar_widget-1.0.2/src/calendar_widget.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calendar_widget
-Version: 1.0.1
+Name: calendar-widget
+Version: 1.0.2
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -35,15 +35,15 @@
 
 ------
 
 ------
 
 ------
 
-# Installation
+# INSTALLATION
 
 ##### Install the calendar widget using the following commands
 ```
 pip install calendar_widget
 ```
 
 # USAGE
@@ -85,20 +85,52 @@
 ```
 
 ##### To destroy the calendar widget, call the destroy method:
 ```
 Calendar.destroy()
 ```
 
+## Example 1 - Basic Setup
+
+-----
+<img align="right" src="https://github.com/Spartanlasergun/calendar_widget/blob/main/README_info/example_one.png?raw=true">
+
+```
+# import tkinter and the calendar widget
+import tkinter
+from calendar_widget import Calendar
+
+# define the main window into which the widget will be placed
+root = tkinter.Tk()
+root.geometry('600x600')  # the geometry function defines the size of the tkinter window
+                          # - in this case, we are using a window that is 600px by 600px
+
+# create the calendar widget
+Calendar = Calendar(root, # specify the tkinter window into which the widget will be placed
+	size = 250, # set the size of the calendar widget to 250px
+	pos_x = 0, # set the x position of the calendar widget within the tkinter window
+	pos_y = 0, # set the y position of the calendar widget within the tkinter window
+	background = 'lightblue', # set the background of the calendar to light blue
+	)
+
+# remember to call your mainloop function so that the tkinter window is persistent
+root.mainloop()
+```
+
+Note: if no 'pos_x' or 'pos_y' parameters are given, the Calendar widget will default to using the standard pack function.
+
+-----
+
+# Widget Parameters - functionality and styling
 
 The table below specifies opitons availiable for styling and other operations associated with the calendar widget
 
 | options | description |
 | ------- | ----------- |
-| size= | Sets the width of the widget in pixels. The default/minimum width is 300px. |
+| size= | Sets the width of the widget in pixels. The default width is 300px. |
 | pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
 | pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
 | style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. |
 | command= | A function to be called when the widget is clicked. |
 | background= | Sets the background of the Calendar to a valid tkinter colour. Example: background="blue" |
 | calendar_relief= | Sets the relief of the Calendar widget. |
 | arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. |
```

### Comparing `calendar_widget-1.0.1/pyproject.toml` & `calendar_widget-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calendar_widget"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Spartanlasergun", email="bns360@live.com" },
 ]
 description = "Calendar widget for use with python tkinter"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `calendar_widget-1.0.1/src/calendar_widget/Calendar_Widget.py` & `calendar_widget-1.0.2/src/calendar_widget/Calendar_Widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Main Class for Calendar Widget. All of its methods are encapsulated within this single class
 class Calendar:
 
     # The init function parameters describe the information that dictates the size, position and styling associated with
     # the calendar object. Comments associated with the usage of each parameter is given within the __init__ function
     # where they are first defined and used.
-    def __init__(self, window_name, pos_x=0, pos_y=0, size=300, style=None, command="no command",
+    def __init__(self, window_name, pos_x=None, pos_y=None, size=300, style=None, command="no command",
                  background="white", calendar_relief="flat",
                  arrow_box_border="black", arrow_box_fill="white", arrow_box_width=1,
                  date_box_border="black", date_box_fill="white", date_box_width=2, date_boxes_outline="black",
                  arrow_outline="black", arrow_fill="white", arrow_thickness=1, arrow_active="orange",
                  weekday_border="gray50", weekday_fill="black", weekday_width=2, weekday_font_fill="white",
                  calendar_date_title="black", date_text_fill="black", trail_box_fill="gray83", trail_text_fill="black",
                  date_highlight="orange", text_highlight_fill="black", weekday_font_family="Algerian",
@@ -70,17 +70,21 @@
         padding = int(size * 0.03333)
 
         # create the tkinter canvas onto which the calendar will be created
         self.Calendar = tkinter.Canvas(window_name, width=size, height=depth,
                                        background=background, relief=calendar_relief)
 
         # position the calendar with the default "pack" option or according the user specified x and y coordinates
-        if (pos_x == 0) and (pos_y == 0):
+        if (pos_x == None) and (pos_y == None):
             self.Calendar.pack()
         else:
+            if pos_x == None:
+                pos_x = 0
+            if pos_y == None:
+                pos_y = 0
             self.Calendar.place(x=pos_x, y=pos_y)
 
         # Calendar Arrow Box
         arrow_box_margin = int(size * 0.25)
         self.Calendar.create_rectangle(arrow_box_margin, padding, (size - arrow_box_margin), (depth * 0.25),
                                   outline=arrow_box_border, fill=arrow_box_fill, width=arrow_box_width, tags="arrow_box")
```

### Comparing `calendar_widget-1.0.1/src/calendar_widget.egg-info/PKG-INFO` & `calendar_widget-1.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calendar-widget
-Version: 1.0.1
+Name: calendar_widget
+Version: 1.0.2
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -35,15 +35,15 @@
 
 ------
 
 ------
 
 ------
 
-# Installation
+# INSTALLATION
 
 ##### Install the calendar widget using the following commands
 ```
 pip install calendar_widget
 ```
 
 # USAGE
@@ -85,20 +85,52 @@
 ```
 
 ##### To destroy the calendar widget, call the destroy method:
 ```
 Calendar.destroy()
 ```
 
+## Example 1 - Basic Setup
+
+-----
+<img align="right" src="https://github.com/Spartanlasergun/calendar_widget/blob/main/README_info/example_one.png?raw=true">
+
+```
+# import tkinter and the calendar widget
+import tkinter
+from calendar_widget import Calendar
+
+# define the main window into which the widget will be placed
+root = tkinter.Tk()
+root.geometry('600x600')  # the geometry function defines the size of the tkinter window
+                          # - in this case, we are using a window that is 600px by 600px
+
+# create the calendar widget
+Calendar = Calendar(root, # specify the tkinter window into which the widget will be placed
+	size = 250, # set the size of the calendar widget to 250px
+	pos_x = 0, # set the x position of the calendar widget within the tkinter window
+	pos_y = 0, # set the y position of the calendar widget within the tkinter window
+	background = 'lightblue', # set the background of the calendar to light blue
+	)
+
+# remember to call your mainloop function so that the tkinter window is persistent
+root.mainloop()
+```
+
+Note: if no 'pos_x' or 'pos_y' parameters are given, the Calendar widget will default to using the standard pack function.
+
+-----
+
+# Widget Parameters - functionality and styling
 
 The table below specifies opitons availiable for styling and other operations associated with the calendar widget
 
 | options | description |
 | ------- | ----------- |
-| size= | Sets the width of the widget in pixels. The default/minimum width is 300px. |
+| size= | Sets the width of the widget in pixels. The default width is 300px. |
 | pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
 | pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
 | style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. |
 | command= | A function to be called when the widget is clicked. |
 | background= | Sets the background of the Calendar to a valid tkinter colour. Example: background="blue" |
 | calendar_relief= | Sets the relief of the Calendar widget. |
 | arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. |
```

