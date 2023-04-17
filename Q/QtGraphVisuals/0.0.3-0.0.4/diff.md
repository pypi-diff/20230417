# Comparing `tmp/qtgraphvisuals-0.0.3.tar.gz` & `tmp/qtgraphvisuals-0.0.4.tar.gz`

## Comparing `qtgraphvisuals-0.0.3.tar` & `qtgraphvisuals-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/src/QtGraphVisuals/.gitignore
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/src/QtGraphVisuals/README.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/src/QtGraphVisuals/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/src/QtGraphVisuals/__main__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/src/QtGraphVisuals/default_visual_schemes.json
--rw-r--r--   0        0        0    16731 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/src/QtGraphVisuals/widgets.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/tests/.test.py.swp
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/tests/test.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/LICENSE
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/.__main__.py.swp
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/.gitignore
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/__main__.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/default_visual_schemes.json
+-rw-r--r--   0        0        0    21369 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/src/QtGraphVisuals/widgets.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/tests/test.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/LICENSE
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 qtgraphvisuals-0.0.4/PKG-INFO
```

### Comparing `qtgraphvisuals-0.0.3/src/QtGraphVisuals/__main__.py` & `qtgraphvisuals-0.0.4/src/QtGraphVisuals/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from PySide6.QtWidgets import QApplication
 from QtGraphVisuals import QGraphViewer
 from qt_material import apply_stylesheet
 import networkx as nx
 
 # Temporary graph generation function
 def graph1():
-    return nx.DiGraph([(1,2), (1,3), (2,4), (3,4), (4,5), (2,5)])
+    return nx.MultiDiGraph([(1,2), (1,3), (2,4), (3,4), (4,5), (2,5)])
 
 def graph2():
-    return nx.DiGraph([(1,2), (1,3), (1,4)])
+    return nx.MultiDiGraph([(1,2), (1,3), (1,4)])
 
 if __name__ == "__main__":
 
     app = QApplication(sys.argv)
     app.setApplicationName("QtGraphVisuals Demo")
 
     extra={ "secondaryDarkColor":"#232629", "font_size": '15px',}
     apply_stylesheet(app, theme='dark_blue.xml', extra=extra)
 
     viewer = QGraphViewer({'graph1': graph1(), 'graph2':graph2()})
+    viewer.resize(800,600)
     viewer.show()
 
     sys.exit(app.exec())
```

### Comparing `qtgraphvisuals-0.0.3/src/QtGraphVisuals/default_visual_schemes.json` & `qtgraphvisuals-0.0.4/src/QtGraphVisuals/default_visual_schemes.json`

 * *Files identical despite different names*

### Comparing `qtgraphvisuals-0.0.3/src/QtGraphVisuals/widgets.py` & `qtgraphvisuals-0.0.4/src/QtGraphVisuals/widgets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
-
 import sys, json, pathlib
 import networkx as nx
 import numpy as np
 from PySide6.QtCore import (Qt, Signal, Slot, QPoint, QPointF, QLine, QLineF,
         QRect, QRectF)
 from PySide6.QtWidgets import (QApplication, QWidget, QLabel, QHBoxLayout,
         QVBoxLayout, QGraphicsView, QGraphicsScene, QGraphicsRectItem,
-        QGraphicsEllipseItem, QGraphicsItem, QGraphicsTextItem, QGroupBox,
+        QGraphicsEllipseItem, QGraphicsItem, QGraphicsTextItem, QGraphicsLineItem, QGroupBox,
         QScrollArea, QFrame, QTabWidget, QSplitter)
 from PySide6.QtGui import QPainter, QTransform, QBrush, QPen, QColor
 
 # Load default visual schemes 
 default_visual_schemes = {}
 path = pathlib.Path(__file__).parent
 with open(path / 'default_visual_schemes.json', 'r') as f:
@@ -163,28 +162,30 @@
 
         # Set scene bounding rect
         self.setSceneRect()
 
         # State
         self._dragging = False
         self._selected = None
+        self._hovering = None
 
         # Center the Scene
         self.centerScene()
 
     def setSceneRect(self):
         br = self.scene().itemsBoundingRect()
         size = QPointF(br.height(), br.width())*10
         tl, br = br.center()-size, br.center()+size
         self.scene().setSceneRect(QRectF(tl, br))
 
     def mousePressEvent(self, e):
         if e.button() == Qt.LeftButton:
             item = self.itemAt(e.position().toPoint())
-            if item and not isinstance(item, VisualGraph):
+
+            if isinstance(item, VisualNode):# and not isinstance(item, VisualGraph):
                 self._selected = item
             else:
                 self._selected = None
 
             self._dragging = True
             self._last_drag_pos = e.position()
         super().mousePressEvent(e)
@@ -194,15 +195,37 @@
             self._dragging = False
             self.setCursor(Qt.ArrowCursor)
             if self._selected:
                 self.clicked.emit(self._selected.get_properties())
                 #self.scene().setSceneRect(self.scene().itemsBoundingRect())
         super().mouseReleaseEvent(e)
 
+    def _checkHovering(self, e):
+        item = self.itemAt(e.position().toPoint())
+        if not item and not self._hovering:
+            pass
+        elif item and not self._hovering:
+            if hasattr(item, 'setHovering'):
+                item.setHovering(True)
+            self._hovering = item
+        elif not item and self._hovering:
+            if hasattr(self._hovering, 'setHovering'):
+                self._hovering.setHovering(False)
+            self._hovering = None 
+        else: # item and self._hovering
+            if not item is self._hovering:
+                if hasattr(self._hovering, 'setHovering'):
+                    self._hovering.setHovering(False)
+                if hasattr(item, 'setHovering'):
+                    item.setHovering(True)
+                self._hovering = item
+
     def mouseMoveEvent(self, e):
+        self._checkHovering(e)
+
         if self._dragging:
             if self._selected:
                 pos = self.mapToScene(e.position().toPoint()) - self._selected.boundingRect().center()
                 self._selected.setPos(pos)
                 #self._vgraph.update()
             else:
                 p0 = self.mapToScene(e.position().toPoint())
@@ -233,42 +256,56 @@
     def centerOfView(self):
         return (self.size().width()-1)/2, (self.size().height()-1)/2
 
     def setGraph(self, graph, visual_scheme=None):
         self.scene().clear()
         
         # Convert graph (if not already a DiGraph) and set visual scheme (if not specified)
-        if isinstance(graph, nx.DiGraph):
+        if isinstance(graph, nx.MultiDiGraph):
             self._graph = graph
             if visual_scheme is None:
                 visual_scheme = default_visual_schemes['default']
         elif 'keras' in graph.__module__:
-            self._graph = self.kerasToDiGraph(graph)
+            self._graph = self.kerasToMultiDiGraph(graph)
             if visual_scheme is None:
                 visual_scheme = default_visual_schemes['keras']
 
         self._vgraph = VisualGraph(self._graph, visual_scheme=visual_scheme)
         self.scene().addItem(self._vgraph)
         self.setSceneRect()
 
         # reset-state
         self._dragging = False
         self._selected = None
 
-    def kerasToDiGraph(self, keras_graph):
+    def kerasToMultiDiGraph(self, model):
         from tensorflow import keras
+        graph = nx.MultiDiGraph()
 
-        graph = nx.DiGraph(name=keras_graph.name)
-        for layer in keras_graph.layers:
-            if layer not in graph:
-                graph.add_node(layer)
-
-            for keras_node in layer.outbound_nodes:
-                graph.add_edge(layer, keras_node.layer)
+        # Add all 'Layers' (aka nodes) to the graph
+        graph.add_nodes_from(model.layers)
 
+        # Get a set of all 'Nodes' (aka edges) in the keras graph
+        keras_nodes = []
+        for layer in model.layers:
+            for node in layer.outbound_nodes:
+                keras_nodes.append(node)
+        keras_nodes = set(keras_nodes)
+
+        # Add the edges to the graph
+        for kn in keras_nodes:
+            input_layers = kn.inbound_layers
+            if not isinstance(input_layers, list): 
+                input_layers = [input_layers]
+            output_layer = kn.outbound_layer
+
+            for index, input_layer in enumerate(input_layers):
+                shape = input_layer.output_shape
+                graph.add_edge(input_layer, output_layer,
+                            in_index=0, out_index=index, shape=shape)
         return graph
 
 class VisualGraph(QGraphicsItem):
     def __init__(self, graph=None, visual_scheme=None, parent=None):
         super().__init__(parent=parent)
 
         # Drawing Config
@@ -279,14 +316,16 @@
 
         self.brush = QBrush(Qt.darkGreen)
         self.pen = QPen(Qt.black, 2)
 
         # State 
         self._graph = graph
         self._node_to_vnode_map = {}
+        self._edge_to_vedge_map = {}
+
         self._generation_map = {}
 
         if graph:
             self.setGraph(graph)
         self._bounding_rect = self.childrenBoundingRect()
 
     def calculate_positions(self):
@@ -326,21 +365,26 @@
 
     def create_visual_nodes(self, positions):
         for node,pos in positions.items():
             l,t = pos[0]-self.node_size/2, pos[1]-self.node_size/2
             self._node_to_vnode_map[node] = VisualNode(node, QPointF(l,t),
                     self.visual_scheme, parent=self)
 
+    def create_visual_edges(self):
+        self._edge_to_vedge_map.clear()
+        for u,v,key,data in self._graph.edges(keys=True, data=True):
+            self._edge_to_vedge_map[(u,v,key)] = VisualEdge((u,v,key,data), parent=self)
+
     def paint(self, painter, option, widget=None):
         if not self._graph:
             return
 
-        for x,y in self._graph.edges:
-            self.paintEdge(x, y, painter) 
-
+        for x,y,_ in self._graph.edges:
+            pass
+            #self.paintEdge(x, y, painter) 
 
     def paintEdge(self, from_node, to_node, painter):
         n0, n1 = self._node_to_vnode_map[from_node], self._node_to_vnode_map[to_node]
         n0_center = n0.pos() + n0.boundingRect().center()
         n1_center = n1.pos() + n1.boundingRect().center()
         t, b = n0_center.y(), n1_center.y()
         l, r = n0_center.x(), n1_center.x()
@@ -348,34 +392,16 @@
         generational_gap = self._generation_map[to_node] - self._generation_map[from_node]
         if  generational_gap > 1 and abs(l - r) < self.x_spacing/4:
             w = self.x_spacing * generational_gap/4 
             rect = QRectF(l-w/2, t, w, b-t)
             start, span = 90*16, np.sign(l-r+0.001)*180*16
             painter.drawArc(rect, start, span)
 
-            #t, b = n0_center.y(), n1_center.y()
-            #l, r = n0_center.x(), n1_center.x()
-            #w, h = (r-l)*2, (b-t)*2
-            #if abs(l - r) < self.x_spacing/4:
-            #    w = self.x_spacing * generational_gap/4 
-            #    rect = QRectF(l-w/2, t, w, b-t)
-            #    start, span = 90*16, np.sign(l-r)*180*16
-            #else:
-            #    rect = QRectF(l-w/2, t, w, h)
-            #    if w >= 0 and h >= 0:
-            #        start, span = 0, 90*16
-            #    elif w < 0 and h >= 0:
-            #        start, span = 180*16, -90*16
-            #    elif w >= 0 and h < 0:
-            #        start, span = 0, -90*16
-            #    elif w < 0 and h < 0:
-            #        start, span = 180*16, 90*16
-            #painter.drawArc(rect, start, span)
-
         else:
+
             line = QLineF(n1_center, n0_center)
             painter.drawLine(line)
 
             c = line.center()
             u = line.unitVector().p1() - line.unitVector().p2()
 
             # Arrow head
@@ -390,26 +416,121 @@
             painter.drawLine(arrow_right)
 
     def boundingRect(self):
         br = self.childrenBoundingRect()
         size = QPointF(br.width(), br.height())
         return QRectF(br.center()-size*2, br.center()+size*2)#self._bounding_rect
 
-    def childrenMoved(self):
+    def childrenMoved(self, child):
         self._bounding_rect = self.childrenBoundingRect()
-        self.update()
+        self.update_adjacent_edges(child.node)
+        #self.update()
+
+    def update_adjacent_edges(self, node):
+        for u,v,idx in self._graph.in_edges(node, keys=True):
+            self._edge_to_vedge_map[(u,v,idx)].updatePath()
+
+        for u,v,idx in self._graph.out_edges(node, keys=True):
+            self._edge_to_vedge_map[(u,v,idx)].updatePath()
 
     def setGraph(self, graph):
-        if not isinstance(graph, nx.DiGraph):
-            raise ValueError()
-        self._graph = graph
+        self._graph = nx.MultiDiGraph(graph)
         positions = self.calculate_positions()
         self.create_visual_nodes(positions)
+        self.create_visual_edges()
         self._bounding_rect = self.childrenBoundingRect()
 
+class VisualEdge(QGraphicsItem):
+    def __init__(self, edge, parent=None):
+        super().__init__(parent=parent)
+
+        # Unpack the edge
+        self.edge = edge
+        self.in_node, self.out_node, self.key, self.data = edge
+        self.in_vnode = self.parentItem()._node_to_vnode_map[self.in_node]
+        self.out_vnode = self.parentItem()._node_to_vnode_map[self.out_node]
+
+        # Create the graphics items
+        self.path = QGraphicsLineItem(parent=self)
+        self.arrow_left = QGraphicsLineItem(parent=self)
+        self.arrow_right = QGraphicsLineItem(parent=self)
+        self.text = QGraphicsTextItem(str(self.data), parent=self)#str(self.data))
+
+        self.path.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
+        self.arrow_left.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
+        self.arrow_right.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
+        self.text.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
+        self.text.setVisible(False)
+
+        # Colorize
+        self.path.setPen(QPen(Qt.white))
+        self.arrow_left.setPen(QPen(Qt.white))
+        self.arrow_right.setPen(QPen(Qt.white))
+        self.text.setDefaultTextColor(Qt.lightGray)
+
+        # Calculate graphic items positions
+        self.setZValue(-1)
+        self.calculatePath()
+        self.calculateArrowHead()
+        self.calculateText()
+
+    def calculatePath(self):
+        delta = 0
+        if isinstance(self.key, int):
+            if self.key != 0:
+                delta = 8 if self.key % 2 else -8
+
+        line = QLineF(self.out_vnode.center(), self.in_vnode.center())
+        if delta:
+            offset = (line.normalVector().unitVector().p2() - line.p1()) * delta
+            line.translate(offset)
+        self.path.setLine(line)
+
+    def calculateArrowHead(self):
+        c = self.path.line().center()
+        u = self.path.line().unitVector().p1() - self.path.line().unitVector().p2()
+        angle = self.path.line().angle()
+
+        # Arrow head
+        arrow_right = QLineF(c+3*u, c-3*u)
+        arrow_right.setAngle(angle+30)
+
+        arrow_left = QLineF(c+3*u, c-3*u)
+        arrow_left.setAngle(angle-30)
+
+        self.arrow_left.setLine(arrow_left)
+        self.arrow_right.setLine(arrow_right)
+
+    def calculateText(self):
+        self.text.setPos(self.path.line().center())
+
+    def updatePath(self):
+        self.calculatePath()
+        self.calculateArrowHead()
+        self.calculateText()
+
+    def setHovering(self, state):
+        if state:
+            self.path.setPen(QPen(Qt.red))
+            self.arrow_left.setPen(QPen(Qt.red))
+            self.arrow_right.setPen(QPen(Qt.red))
+            self.text.setVisible(True)
+        else:
+            self.path.setPen(QPen(Qt.white))
+            self.arrow_left.setPen(QPen(Qt.white))
+            self.arrow_right.setPen(QPen(Qt.white))
+            self.text.setVisible(False)
+        self.update()
+
+    def paint(self, painter, option, widget=None):
+        pass
+
+    def boundingRect(self):
+        return QRectF(self.arrow_left.boundingRect()).united(self.arrow_right.boundingRect())
+
 class VisualNode(QGraphicsItem):
     def __init__(self, node, pos, visual_scheme, parent=None):
         super().__init__(parent)
         # Keep reference to node
         self.visual_scheme = visual_scheme
         self.node = node
 
@@ -417,23 +538,25 @@
         self.node_label, self.pen, self.brush, self.size = None, None, None, None
         self.setNodeConfig()
 
         # set node shell
         self.shell = QGraphicsEllipseItem(0, 0, self.size[0], self.size[1], parent=self)
         self.shell.setBrush(self.brush)
         self.shell.setPen(self.pen)
+        self.shell.setEnabled(False)
         self.shell.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
 
         # set text
         self.text = QGraphicsTextItem(self.label_text, parent=self)
         self.text.setPos(self.shell.boundingRect().center() - self.text.boundingRect().center())
         self.text.setFlag(QGraphicsItem.ItemStacksBehindParent, enabled=True)
+        self.text.setEnabled(False)
         self.text.setDefaultTextColor(Qt.white)
 
-        self.setPos(pos - self.boundingRect().center())
+        super().setPos(pos - self.boundingRect().center())
 
     def setNodeConfig(self):
         ntype = type(self.node).__name__
         default_config = self.visual_scheme['nodes'].get('default', {})
         config = self.visual_scheme['nodes'].get(ntype, default_config)
 
         # Pen
@@ -471,17 +594,20 @@
 
     def paint(self, painter, option, widget=None):
         pass
 
     def boundingRect(self):
         return self.childrenBoundingRect() 
 
+    def center(self):
+        return self.pos() + self.childrenBoundingRect().center()
+
     def setPos(self, pos):
         super().setPos(pos)
-        self.parentItem().childrenMoved()
+        self.parentItem().childrenMoved(self)
 
     def mousePressEvent(self, e):
         super().mousePressEvent(e)
 
 class GraphLayout:
     def __init__(self):
         pass
```

### Comparing `qtgraphvisuals-0.0.3/LICENSE` & `qtgraphvisuals-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgraphvisuals-0.0.3/PKG-INFO` & `qtgraphvisuals-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: QtGraphVisuals
-Version: 0.0.3
+Version: 0.0.4
 Summary: A qt-widget to visualize directed graphs
 Project-URL: Homepage, https://github.com/jake987654321/QtGraphVisuals
 Project-URL: Bug Tracker, https://github.com/jake987654321/QtGraphVisuals/issues
 Author-email: Jacob Botimer <botimerj@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: networkx
+Requires-Dist: numpy
 Requires-Dist: pyside6
 Requires-Dist: qt-material
 Description-Content-Type: text/markdown
 
 # Example Package
```

