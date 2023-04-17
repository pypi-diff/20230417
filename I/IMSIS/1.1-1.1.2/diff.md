# Comparing `tmp/imsis-1.1.tar.gz` & `tmp/IMSIS-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imsis-1.1.tar", last modified: Fri Nov 18 22:05:08 2022, max compression
+gzip compressed data, was "IMSIS-1.1.2.tar", last modified: Mon Apr 17 03:59:53 2023, max compression
```

## Comparing `imsis-1.1.tar` & `IMSIS-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-11-18 22:05:08.000000 imsis-1.1/
-drwxrwxrwx   0        0        0        0 2022-11-18 22:05:08.000000 imsis-1.1/imsis/
--rw-rw-rw-   0        0        0    81543 2022-06-02 21:33:29.000000 imsis-1.1/imsis/analyze.py
--rw-rw-rw-   0        0        0    70860 2022-11-18 20:08:01.000000 imsis-1.1/imsis/dialogs.py
--rw-rw-rw-   0        0        0    94179 2022-11-05 20:00:07.000000 imsis-1.1/imsis/image.py
--rw-rw-rw-   0        0        0    10818 2022-03-14 19:31:26.000000 imsis-1.1/imsis/imagestack.py
--rw-rw-rw-   0        0        0      763 2022-04-07 18:39:47.000000 imsis-1.1/imsis/logging.py
--rw-rw-rw-   0        0        0     5025 2022-01-25 22:46:06.000000 imsis-1.1/imsis/misc.py
--rw-rw-rw-   0        0        0     9365 2022-04-09 09:31:10.000000 imsis-1.1/imsis/view.py
--rw-rw-rw-   0        0        0      243 2021-11-26 19:58:43.000000 imsis-1.1/imsis/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-18 22:05:08.000000 imsis-1.1/imsis.egg-info/
--rw-rw-rw-   0        0        0        1 2022-11-18 22:05:08.000000 imsis-1.1/imsis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      786 2022-11-18 22:05:08.000000 imsis-1.1/imsis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        9 2022-11-18 22:05:08.000000 imsis-1.1/imsis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      319 2022-11-18 22:05:08.000000 imsis-1.1/imsis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2022-11-18 22:05:08.000000 imsis-1.1/imsis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      786 2022-11-18 22:05:08.000000 imsis-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      469 2022-11-18 21:57:08.000000 imsis-1.1/pyproject.toml
--rw-rw-rw-   0        0        0     3209 2021-12-18 17:06:47.000000 imsis-1.1/README.md
--rw-rw-rw-   0        0        0       86 2022-11-18 22:05:08.000000 imsis-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1040 2022-11-18 22:00:04.000000 imsis-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:59:53.248866 IMSIS-1.1.2/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:59:53.231867 IMSIS-1.1.2/IMSIS.egg-info/
+-rw-rw-rw-   0        0        0     4042 2023-04-17 03:59:53.000000 IMSIS-1.1.2/IMSIS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-04-17 03:59:53.000000 IMSIS-1.1.2/IMSIS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 03:59:53.000000 IMSIS-1.1.2/IMSIS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 03:59:53.000000 IMSIS-1.1.2/IMSIS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 03:59:53.000000 IMSIS-1.1.2/IMSIS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1071 2021-12-18 17:06:47.000000 IMSIS-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1075 2022-04-04 20:33:25.000000 IMSIS-1.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4042 2023-04-17 03:59:53.248866 IMSIS-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3209 2021-12-18 17:06:47.000000 IMSIS-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 03:59:53.247874 IMSIS-1.1.2/imsis/
+-rw-rw-rw-   0        0        0      243 2021-11-26 19:58:43.000000 IMSIS-1.1.2/imsis/__init__.py
+-rw-rw-rw-   0        0        0   100705 2023-02-21 20:48:24.000000 IMSIS-1.1.2/imsis/analyze.py
+-rw-rw-rw-   0        0        0    78317 2023-02-27 12:01:13.000000 IMSIS-1.1.2/imsis/dialogs.py
+-rw-rw-rw-   0        0        0   107448 2023-02-16 10:27:54.000000 IMSIS-1.1.2/imsis/image.py
+-rw-rw-rw-   0        0        0    13126 2023-02-16 09:01:52.000000 IMSIS-1.1.2/imsis/imagestack.py
+-rw-rw-rw-   0        0        0      763 2022-04-07 18:39:47.000000 IMSIS-1.1.2/imsis/logging.py
+-rw-rw-rw-   0        0        0     6261 2023-01-30 23:11:03.000000 IMSIS-1.1.2/imsis/misc.py
+-rw-rw-rw-   0        0        0     9677 2023-01-30 22:01:02.000000 IMSIS-1.1.2/imsis/view.py
+-rw-rw-rw-   0        0        0      466 2023-04-17 03:59:07.000000 IMSIS-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-04-17 03:59:53.249865 IMSIS-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1227 2023-04-17 03:56:25.000000 IMSIS-1.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imsis-1.1/imsis/analyze.py` & `IMSIS-1.1.2/imsis/analyze.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,53 +5,86 @@
 Licensed under the MIT license:
 http://www.opensource.org/licenses/MIT-license
 
 This module contains methods to analyze images
 """
 
 import math
+import time
 
 import cv2 as cv
 import matplotlib.gridspec as gridspec
 import matplotlib.pyplot as plt
+import matplotlib.patches as mpatches
+
 import numpy as np
 
 import imsis as ims
 from scipy import ndimage
 from PIL import Image
 from PIL import ImageDraw
 from PIL import ImageFont
 import scipy
 import sys
 
 import scipy.stats as stats
 from scipy import fftpack
+import random as rng
+from collections import deque
+
+rng.seed(12345)
 
 colors = [
+    [255, 255, 128],
     [255, 255, 64],
-    [255, 64, 255],
-    [192, 255, 64],
-    [192, 64, 255],
+    [255, 192, 192],
+    [255, 192, 128],
     [255, 192, 64],
+    [255, 128, 192],
+    [255, 128, 128],
+    [255, 128, 64],
     [255, 64, 192],
+    [255, 64, 128],
+    [255, 64, 64],
+    [192, 255, 192],
+    [192, 255, 128],
+    [192, 255, 64],
+    [192, 192, 255],
+    [192, 192, 128],
     [192, 192, 64],
+    [192, 128, 192],
+    [192, 128, 128],
+    [192, 128, 64],
     [192, 64, 192],
+    [192, 64, 128],
+    [192, 64, 64],
+    [128, 255, 192],
+    [128, 255, 128],
     [128, 255, 64],
-    [128, 64, 255],
-    [255, 128, 64],
-    [255, 64, 128],
+    [128, 192, 192],
+    [128, 192, 128],
     [128, 192, 64],
-    [128, 64, 192],
-    [192, 128, 64],
-    [192, 64, 128],
-    [255, 64, 64],
+    [128, 128, 192],
+    [128, 128, 255],
     [128, 128, 64],
+    [128, 64, 192],
     [128, 64, 128],
-    [192, 64, 64],
     [128, 64, 64],
+    [64, 255, 192],
+    [64, 255, 128],
+    [64, 255, 64],
+    [64, 192, 192],
+    [64, 192, 128],
+    [64, 192, 64],
+    [64, 128, 192],
+    [64, 128, 255],
+    [64, 128, 64],
+    [64, 64, 192],
+    [64, 64, 128],
+    [64, 64, 255]
 ]
 
 
 class Analyze(object):
 
     @staticmethod
     def __findlocalExtrema(y):
@@ -158,26 +191,26 @@
             gridspec.GridSpec(4, 1)
             plt.subplot2grid((4, 1), (0, 0), colspan=1, rowspan=2)
             st1 = "Edge position=({},{})".format(xpos, ypos)
             plt.title(st1)
             plt.imshow(rgb)
             plt.subplot2grid((4, 1), (2, 0), colspan=1, rowspan=1)
             plt.plot(xn, yn)
-            plt.axvline(x=yf,color='g', linestyle='--')
+            plt.axvline(x=yf, color='g', linestyle='--')
 
             # Show the major grid lines with dark grey lines
             plt.grid(b=True, which='major', color='#666666', linestyle='-')
             # Show the minor grid lines with very faint and almost transparent grey lines
             plt.minorticks_on()
             plt.grid(b=True, which='minor', color='#999999', linestyle='-', alpha=0.2)
             #  plt.grid(color='green', linestyle='--', linewidth=0.5)
 
             plt.subplot2grid((4, 1), (3, 0), colspan=1, rowspan=1)
             plt.plot(xn, y2)
-            plt.axvline(x=yf,color='g', linestyle='--')
+            plt.axvline(x=yf, color='g', linestyle='--')
 
             # Show the major grid lines with dark grey lines
             plt.grid(b=True, which='major', color='#666666', linestyle='-')
             # Show the minor grid lines with very faint and almost transparent grey lines
             plt.minorticks_on()
             plt.grid(b=True, which='minor', color='#999999', linestyle='-', alpha=0.2)
             #  plt.grid(color='green', linestyle='--', linewidth=0.5)
@@ -961,14 +994,16 @@
         Enter the threshold value for masking. Features will be labeled and counted.
 
         overlay displays an overlay of the features found on top of the original image.
         out shows the labeled features without overlay
         graph shows the size distribution
         cntsSorted contains the list of contours
 
+        DEPRECIATED - replaced by class FeatureSizeDistribution
+
         :Parameters: original_image, threshold_image
         :Returns: overlay, out, cntsSorted, (area, colorvalue)
         """
 
         # img = ims.Image.Convert.toGray(orig)
         # Find all contours on the map
         # _th, contours, hierarchy = cv.findContours(thresh, cv.RETR_TREE, cv.CHAIN_APPROX_NONE)
@@ -1014,31 +1049,28 @@
 
         overlay = cv.addWeighted(img5b, 0.7, out, 0.3, 0)
         # graph = fig
         # fig.show()
         return overlay, out, cntsSorted, sizedistout
 
     @staticmethod
-    def correct_imageshift_list(framelist):
+    def correct_imageshift_list(framelist, update_reference_image=True, high_precision=False):
         """
+        DEPRECIATED - use Imagestack.align_images
+
         Correct image shifts for a list of images in memory
         Images should be of the same size
 
+        update_reference_image True: means the last aligned image acts as a reference. False the first image acts as a reference.
+        high precision uses a nonmaximum suppression algorithm: this is more precise but a lot slower
+
         :Parameters: image list
         :Returns: image list, correctiondata list(X,Y,Score)
         """
-        framelist2 = []
-        correctiondatalist = []
-        frames = len(framelist)
-        frame0 = framelist[0]
-        for i in range(1, frames):
-            frame1 = framelist[i]
-            frame0, sx, sy, score = Analyze.ImageAlignment.NCC(frame0, frame1)
-            framelist2.append(frame0)
-            correctiondatalist.append([sx, sy, score])
+        framelist2, correctiondatalist = ims.ImageStack.align_images(framelist,update_reference_image=update_reference_image,high_precision=high_precision)
         return framelist2, correctiondatalist
 
     @staticmethod
     def PSNR(target, ref):
         """Return peaksignal to noise ratio
 
         :Parameters: image1, image2
@@ -1167,26 +1199,24 @@
             plt.figure(3)
             plt.clf()
             plt.gcf().canvas.set_window_title('Power Spectrum')
             plt.semilogy(psd1D)
             plt.xlabel("Spatial Frequency")
             plt.ylabel("Power Spectrum")
 
-            if autoclose>0:
+            if autoclose > 0:
                 try:
                     plt.show(block=False)
                     plt.pause(autoclose)  # 3 seconds, I use 1 usually
                 except:
                     print("interrupted while waiting.")
                 plt.close("all")
             else:
                 plt.show()
 
-
-
         return psd1D
 
     @staticmethod
     def hough_lines(image, threshold=2, minlinelength=50, maxlinegap=5):
         """ Hough lines detection
 
         :Parameters: image
@@ -1244,14 +1274,16 @@
             colors, count = np.unique(img.reshape(-1, img.shape[-1]), axis=0, return_counts=True)
             out = (colors[count.argmax()]).tolist()
         else:
             colors, count = np.unique(img.reshape(-1, 1), axis=0, return_counts=True)
             out = (colors[count.argmax()]).tolist()
         return out
 
+
+
     class SharpnessDetection:
         # Ref: http: // radjkarl.github.io / imgProcessor / _modules / imgProcessor / measure / sharpness / parameters.html
 
         def varianceOfLaplacian(self, img):
             """Variance of Laplacian (LAPV) Pech 2000
             """
             lap = cv.Laplacian(img, ddepth=-1)  # cv2.cv.CV_64F)
@@ -1732,16 +1764,15 @@
         def s_center_pixels(self, value):
             self._s_center_pixels = value
 
         @s_size_pixels.setter
         def s_size_pixels(self, value):
             self._s_size_pixels = value
 
-
-        #methods = ['cv.TM_CCOEFF', 'cv.TM_CCOEFF_NORMED', 'cv.TM_CCORR',
+        # methods = ['cv.TM_CCOEFF', 'cv.TM_CCOEFF_NORMED', 'cv.TM_CCORR',
         #                   'cv.TM_CCORR_NORMED', 'cv.TM_SQDIFF', 'cv.TM_SQDIFF_NORMED','zncc','ssd','sad']
         @template_matcher.setter
         def template_matcher(self, value):
             self._template_matcher = value
 
         @apply_gradient.setter
         def apply_gradient(self, value):
@@ -1829,18 +1860,20 @@
             :Returns: -
             """
             img0 = ims.Image.Convert.to8bit(img0)
             img2 = ims.Analyze.add_text(img0, 0, 0, 'Input: drag a rectangle around the fiducial area.', 20)
             shapes = ims.Dialogs.select_areas(img2, 'Template matching input')
             if not shapes:
                 print("Warning: Shape is not defined, taking 90% of full image")
-                shapes = [[(int(img0.shape[1]*0.1),int(img0.shape[0]*0.1)),(int(img0.shape[1]*0.9),int(img0.shape[0]*0.9))]]
-            if len(shapes)>1:
+                shapes = [[(int(img0.shape[1] * 0.1), int(img0.shape[0] * 0.1)),
+                           (int(img0.shape[1] * 0.9), int(img0.shape[0] * 0.9))]]
+            if len(shapes) > 1:
                 print("Warning: Multiple shapes defined, taking 90% of full image")
-                shapes = [[(int(img0.shape[1]*0.1),int(img0.shape[0]*0.1)),(int(img0.shape[1]*0.9),int(img0.shape[0]*0.9))]]
+                shapes = [[(int(img0.shape[1] * 0.1), int(img0.shape[0] * 0.1)),
+                           (int(img0.shape[1] * 0.9), int(img0.shape[0] * 0.9))]]
             widthperc, heightperc, centerxperc, centeryperc = ims.Analyze.rectangle_pixels_to_percentage(img0,
                                                                                                          shapes[0])
             t_center_perc = [centerxperc, centeryperc]
             t_size_perc = [widthperc, heightperc]
             # template = self.create_template(img0, t_center_perc, t_size_perc)
             t_center_px, t_size_px = ims.Analyze.rectangle_percentage_to_pixels(img0, t_center_perc, t_size_perc)
             template = self.__cut(img0, t_center_px, t_size_px)
@@ -1900,15 +1933,15 @@
                 if (method == 6):
                     top_left, max_val = self._template_matching_zncc(img, template)
                 if (method == 7):
                     top_left, max_val = self._template_matching_ssd(img, template)
                 if (method == 8):
                     top_left, max_val = self._template_matching_sad(img, template)
 
-            #print(top_left, max_val)
+            # print(top_left, max_val)
             # sys.exit()
             bottom_right = (w, h)
             wd2 = int(w / 2)
             hd2 = int(h / 2)
             pt = (top_left[0] + wd2, top_left[1] + hd2)
             # print("Position found:",pt)
             score = max_val
@@ -2056,11 +2089,428 @@
             self.s_size_perc = [self.t_size_perc[0] * perc, self.t_size_perc[1] * perc]
             if self.s_size_perc[0] > 1:
                 self.s_size_perc[0] = 1
             if self.s_size_perc[1] > 1:
                 self.s_size_perc[1] = 1
             if verbose == True:
                 print('searchregion, searchsize: ', self.s_center_perc, self.s_size_perc)
-            #calculate same but in pixels
+            # calculate same but in pixels
             self.s_center_pixels, self.s_size_pixels = ims.Analyze.rectangle_percentage_to_pixels(img,
                                                                                                   self.s_center_perc,
                                                                                                   self.s_size_perc)
+
+    class FeatureProperties(object):
+
+        propertynames = ['Area',
+                         'EquivalentDiameter',
+                         'Orientation',
+                         'MajorAxisLength',
+                         'MinorAxisLength',
+                         'Perimeter',
+                         'XCoord',
+                         'YCoord',
+                         'Solidity',
+                         'BoundingBoxWidth',
+                         'BoundingBoxHeight',
+                         'BoundingBoxArea',
+                         'ConvexHullArea',
+                         'MinIntensity',
+                         'MeanIntensity',
+                         'MaxIntensity',
+                         'Extent',
+                         'AspectRatio',
+                         'ColorValue',
+                         'Filename']
+
+        @staticmethod
+        def _process_contours(orig, thresh, contours, minarea, maxarea, filename):
+            cntsSorted = sorted(contours, key=lambda x: cv.contourArea(x))
+
+            imggray = ims.Image.Convert.toGray(orig)
+
+            img5 = ims.Image.Convert.toRGB(orig)
+            img5b = img5.copy()
+            img5c = np.zeros([img5.shape[0], img5.shape[1], 3], dtype=np.uint8)
+
+            if maxarea == -1:
+                maxarea = orig.shape[0] * orig.shape[1]
+
+            featureproperties = []
+            coords = []
+            cntsSorted_new = []
+            for i in range(len(cntsSorted)):
+                failed = False
+                try:
+                    ((centx, centy), (width, height), angle) = cv.fitEllipse(cntsSorted[i])
+                    orientation = angle
+                    majoraxislength = width
+                    minoraxislength = height
+
+                    area = cv.contourArea(cntsSorted[i])
+                    hull = cv.convexHull(cntsSorted[i])
+                    hull_area = cv.contourArea(hull)
+                    xcoord = 0
+                    ycoord = 0
+
+                    if (area < minarea) or (area > maxarea):
+                        failed = True
+
+                    x, y, w, h = cv.boundingRect(cntsSorted[i])
+                    bboxwidth = w
+                    bboxheight = h
+                    bboxarea = bboxwidth * bboxheight
+                    if bboxarea > (orig.shape[0] * orig.shape[1]) * 0.98:
+                        failed = True  # entire image is selected
+                    if hull_area == 0:
+                        solidity = 0
+                        failed = True
+                    else:
+                        solidity = float(area) / hull_area
+                        M = cv.moments(cntsSorted[i])
+                        cx = int(M['m10'] / M['m00'])
+                        cy = int(M['m01'] / M['m00'])
+                        xcoord = cx
+                        ycoord = cy
+                except:
+                    failed = True
+
+                if failed == False:
+                    # excluding failed calculations, usually 1 pixel measurements.
+                    perimeter = cv.arcLength(cntsSorted[i], True)
+                    equi_diameter = np.sqrt(4 * area / np.pi)
+
+                    if bboxarea > 0:
+                        extent = area / bboxarea
+                    else:
+                        extent = 0
+                    if h > 0:
+                        aspect_ratio = w / h
+                    else:
+                        aspect_ratio = 1
+
+                    bboximage = imggray[y:y + h, x:x + w]
+                    min_val, max_val, min_loc, max_loc = cv.minMaxLoc(bboximage)
+
+                    meanintensity = cv.mean(bboximage)[0]
+                    minintensity = min_val
+                    maxintensity = max_val
+
+                    if (xcoord, ycoord) not in coords and ((xcoord - 1, ycoord)) not in coords and (
+                            (xcoord, ycoord - 1)) not in coords and ((xcoord + 1, ycoord)) not in coords and (
+                            (xcoord, ycoord + 1)) not in coords:
+                        coords.append((xcoord, ycoord))
+                        featureproperties.append(
+                            [area, equi_diameter, orientation, majoraxislength, minoraxislength, perimeter, xcoord,
+                             ycoord,
+                             solidity, bboxwidth, bboxheight, bboxarea, hull_area, minintensity, meanintensity,
+                             maxintensity, extent, aspect_ratio, 0, filename])
+                        cntsSorted_new.append(cntsSorted[i])
+
+            print("countsSorted_new: ", len(cntsSorted_new))
+            if (len(cntsSorted_new) > 0):
+                minarea = cv.contourArea(cntsSorted_new[0])
+                maxarea = cv.contourArea(cntsSorted_new[-1])
+                mularea = (len(colors) - 1) / (maxarea - minarea)
+
+                colvalidx = Analyze.FeatureProperties.propertynames.index("ColorValue")
+
+                for i in range(len(cntsSorted_new)):
+                    area = cv.contourArea(cntsSorted_new[i]) - minarea + 1
+                    colvi = int(area * mularea)
+                    coln = colors[colvi]
+                    featureproperties[i][colvalidx] = colvi
+                    img6 = cv.drawContours(img5c, cntsSorted_new, i, coln, -1)
+
+                print("Number of contours detected = %d" % len(featureproperties))
+
+                out = cv.bitwise_and(img6, img6, mask=thresh)
+                overlay = cv.addWeighted(img5b, 0.7, out, 0.3, 0)
+            else:
+                print("Warning: No contours found.")
+                overlay = img5.copy()
+                out = img5.copy()
+            return overlay, out, featureproperties
+
+        @staticmethod
+        def _contours_with_distance_map(orig, thresh, distance_threshold=0.2):
+            # noise removal
+            kernel = np.ones((3, 3), np.uint8)
+            opening = cv.morphologyEx(thresh, cv.MORPH_OPEN, kernel, iterations=1)
+
+            # sure background area
+            sure_bg = cv.dilate(opening, kernel, iterations=1)
+
+            # Finding sure foreground area
+            dist_transform = cv.distanceTransform(opening, cv.DIST_L2, 3)
+            # ims.View.plot(dist_transform)
+
+            # the 0.2 threshold figure modifies the figure
+            ret, sure_fg = cv.threshold(dist_transform, distance_threshold * dist_transform.max(), 255, 0)
+
+            # Finding unknown feature
+            sure_fg = np.uint8(sure_fg)
+            unknown = cv.subtract(sure_bg, sure_fg)
+
+            # Marker labelling
+            ret, markers = cv.connectedComponents(sure_fg)
+            # Add one to all labels so that sure background is not 0, but 1
+            markers = markers + 1
+            # Now, mark the feature of unknown with zero
+            markers[unknown == 255] = 0
+
+            orig2 = ims.Image.Convert.toRGB(orig)
+            markers = cv.watershed(orig2, markers)
+            orig2[markers == -1] = [255, 0, 0]
+
+            contour, hierarchy = cv.findContours(image=markers.copy(), mode=cv.RETR_CCOMP,
+                                                 method=cv.CHAIN_APPROX_SIMPLE)
+            return contour, markers
+
+        @staticmethod
+        def get_featureproperties(orig, thresh, minarea=0,
+                                  maxarea=-1, applydistancemap=True, distance_threshold=0.2, filename=""):
+            """Determine the list of features with properties per patch
+
+            threshold value for the applied image mask.
+            mininum and maximum bounding box size (=width x height of a feature.
+            enable/disable a distance map for seperation of overlapping features
+            distance threshold between 0.1 and 0.9 if a distance map is used.
+
+            overlay displays an overlay of the features found on top of the original image.
+            out shows the labeled features without overlay
+            graph shows the size distribution
+
+            propertynames = ['Area',
+                        'EquivalentDiameter',
+                        'Orientation',
+                        'MajorAxisLength',
+                        'MinorAxisLength',
+                        'Perimeter',
+                        'XCoord',
+                        'YCoord',
+                        'Solidity',
+                        'BoundingBoxWidth',
+                        'BoundingBoxHeight',
+                        'BoundingBoxArea',
+                        'ConvexHullArea',
+                        'MinIntensity',
+                        'MeanIntensity',
+                        'MaxIntensity',
+                        'Extent',
+                        'AspectRatio',
+                        'ColorValue',
+                        'Filename']
+
+
+            :Parameters: original_image, threshold_image, minarea, maxarea, apply_distance_map, distance_threshold
+            :Returns: overlay, out, markers featureproperties
+            """
+
+            # img = ims.Image.Convert.toGray(orig)
+            # Find all contours on the map
+            # _th, contours, hierarchy = cv.findContours(thresh, cv.RETR_TREE, cv.CHAIN_APPROX_NONE)
+
+            # cv version check
+
+            if applydistancemap == True:
+                contours, markers = Analyze.FeatureProperties._contours_with_distance_map(orig, thresh,
+                                                                                          distance_threshold)
+            else:
+                markers = ims.Image.new(8, 8)
+                (cvmajor, cvminor, _) = cv.__version__.split(".")
+                if (int(cvmajor) < 4):
+                    _th, contours, hierarchy = cv.findContours(thresh, cv.RETR_TREE, cv.CHAIN_APPROX_NONE)
+                else:
+                    contours, hierarchy = cv.findContours(thresh, cv.RETR_TREE, cv.CHAIN_APPROX_NONE)
+
+            overlay, out, featureproperties = Analyze.FeatureProperties._process_contours(orig, thresh, contours,
+                                                                                          minarea, maxarea, filename)
+            return overlay, out, markers, featureproperties
+
+        def plot_feature_size_distribution(im_labeled, featureproperties, path_out, autoclose=0):
+            """Plot the feature size distribution
+                :Parameters: labeled_image, featureproperties, path_out,autoclose
+                :Returns: NA
+            """
+
+            areaidx = Analyze.FeatureProperties.propertynames.index("Area")
+            coloridx = Analyze.FeatureProperties.propertynames.index("ColorValue")
+
+            arealist = []
+            colorList = []
+            for item in featureproperties:
+                arealist.append(item[areaidx])
+
+                coln = colors[item[coloridx]]
+                # print(coln)
+                col = [coln[2] / 255., coln[1] / 255., coln[0] / 255., 1]
+                colorList.append(col)
+
+            Y = (np.array(arealist))
+            X = np.arange(1, len(arealist) + 1)
+
+            plt.figure(figsize=(8, 4))
+            plt.gcf().canvas.set_window_title('Size Distribution')
+
+            gridspec.GridSpec(1, 2)
+            plt.subplot2grid((1, 2), (0, 0), colspan=1, rowspan=1)
+            plt.imshow(im_labeled)
+
+            plt.subplot2grid((1, 2), (0, 1), colspan=1, rowspan=1)
+
+            plt.bar(X, Y, color=colorList)
+            plt.xlabel("Feature Number")
+            plt.ylabel("Area [pixels]")
+            plt.tight_layout()
+
+            plt.savefig(path_out + "size_distribution.png")
+            if autoclose > 0:
+                try:
+                    plt.show(block=False)
+                    plt.pause(autoclose)  # 3 seconds, I use 1 usually
+                except:
+                    print("interrupted while waiting.")
+                plt.close("all")
+            else:
+                plt.show()
+            plt.close()
+
+        def get_image_with_boundingboxes(image, featureproperties, path_out):
+            """Plot the feature size distribution
+                :Parameters: image, featureproperties, path_out
+                :Returns: image_with_boundingboxes
+            """
+            widx = Analyze.FeatureProperties.propertynames.index("BoundingBoxWidth")
+            hidx = Analyze.FeatureProperties.propertynames.index("BoundingBoxHeight")
+            xidx = Analyze.FeatureProperties.propertynames.index("XCoord")
+            yidx = Analyze.FeatureProperties.propertynames.index("YCoord")
+
+            img = image.copy()
+
+            for item in featureproperties:
+                # Draw rectangle around segmented items.
+                w = item[widx]
+                h = item[hidx]
+                x = item[xidx] - int(w / 2)
+                y = item[yidx] - int(h / 2)
+
+                img = cv.rectangle(img, (x, y), (x + w, y + h), (0, 0, 255), 3)
+            return img
+
+        def get_image_with_centermarkers(image, featureproperties, path_out):
+            """Plot the feature size distribution
+                :Parameters: image, featureproperties, path_out
+                :Returns: image_with_labels
+            """
+            xidx = Analyze.FeatureProperties.propertynames.index("XCoord")
+            yidx = Analyze.FeatureProperties.propertynames.index("YCoord")
+
+            img = image.copy()
+
+            for item in featureproperties:
+                x = item[xidx]
+                y = item[yidx]
+
+                img = cv.circle(img, (x, y), 1, (0, 0, 255), 3)
+            return img
+
+        def get_image_with_ellipses(image, featureproperties):
+            """Plot the feature size distribution
+                :Parameters: image, featureproperties, path_out
+                :Returns: image_with_ellipses
+            """
+            majidx = Analyze.FeatureProperties.propertynames.index("MajorAxisLength")
+            minidx = Analyze.FeatureProperties.propertynames.index("MinorAxisLength")
+            oidx = Analyze.FeatureProperties.propertynames.index("Orientation")
+            xidx = Analyze.FeatureProperties.propertynames.index("XCoord")
+            yidx = Analyze.FeatureProperties.propertynames.index("YCoord")
+
+            img = image.copy()
+
+            for item in featureproperties:
+                # Draw rectangle around segmented items.
+                w = int(item[majidx] / 2)
+                h = int(item[minidx] / 2)
+                angle = item[oidx]
+                x = item[xidx]
+                y = item[yidx]
+                img = cv.ellipse(img, (x, y), (w, h), angle=angle, startAngle=0, endAngle=360, color=(0, 0, 255),
+                                 thickness=2)
+            return img
+
+        def save_boundingboxes(image, featureproperties, path_out, max_features_per_page=50):
+            """Plot a patched image of features found
+                :Parameters: image, featureproperties, path_out
+                :Returns: NA
+            """
+            widx = Analyze.FeatureProperties.propertynames.index("BoundingBoxWidth")
+            hidx = Analyze.FeatureProperties.propertynames.index("BoundingBoxHeight")
+            xidx = Analyze.FeatureProperties.propertynames.index("XCoord")
+            yidx = Analyze.FeatureProperties.propertynames.index("YCoord")
+
+            img = image.copy()
+
+            j = 0
+            for item in featureproperties:
+                # Draw rectangle around segmented items.
+                w = item[widx]
+                h = item[hidx]
+                x = item[xidx] - int(w / 2)
+                y = item[yidx] - int(h / 2)
+                bboximage = img[y:y + h, x:x + w]
+                ims.Image.save(bboximage, path_out + "patches\label_{}.png".format(j), verbose=False)
+                j = j + 1
+
+    class OpticalFlow(object):
+        def draw_flow(img, flow, step=16):
+            h, w = img.shape[:2]
+            y, x = np.mgrid[step / 2:h:step, step / 2:w:step].reshape(2, -1).astype(int)
+            fx, fy = flow[y, x].T
+            lines = np.vstack([x, y, x + fx, y + fy]).T.reshape(-1, 2, 2)
+            lines = np.int32(lines + 0.5)
+            vis = cv.cvtColor(img, cv.COLOR_GRAY2BGR)
+            cv.polylines(vis, lines, 0, (0, 255, 0))
+            for (x1, y1), (x2, y2) in lines:
+                cv.circle(vis, (x1, y1), 1, (0, 255, 0), -1)
+            return vis
+
+        def draw_hsv(flow):
+            h, w = flow.shape[:2]
+            fx, fy = flow[:, :, 0], flow[:, :, 1]
+            ang = np.arctan2(fy, fx) + np.pi
+            v = np.sqrt(fx * fx + fy * fy)
+            hsv = np.zeros((h, w, 3), np.uint8)
+            hsv[..., 0] = ang * (180 / np.pi / 2)
+            hsv[..., 1] = 255
+            hsv[..., 2] = np.minimum(v * 4, 255)
+
+            bgr = cv.cvtColor(hsv, cv.COLOR_HSV2BGR)
+            return bgr
+
+        def warp_flow(img, flow):
+            h, w = flow.shape[:2]
+            flow = -flow
+            flow[:, :, 0] += np.arange(w)
+            flow[:, :, 1] += np.arange(h)[:, np.newaxis]
+            res = cv.remap(img, flow, None, cv.INTER_LINEAR)
+            return res
+
+        def dense_optical_flow(img0, img1):
+            img0 = ims.Image.Convert.toRGB(img0)
+            img1 = ims.Image.Convert.toRGB(img1)
+            imgL = cv.pyrDown(img0)
+            imgR = cv.pyrDown(img1)
+            prev = imgL
+            prevgray = cv.cvtColor(prev, cv.COLOR_BGR2GRAY)
+            cur_glitch = prev.copy()
+            img = imgR
+            gray = cv.cvtColor(img, cv.COLOR_BGR2GRAY)
+            flow = cv.calcOpticalFlowFarneback(prevgray, gray, None, 0.5, 3, 15, 3, 5, 1.2, 0)
+            cur_glitch = Analyze.OpticalFlow.warp_flow(cur_glitch, flow)
+            flow = Analyze.OpticalFlow.draw_flow(gray, flow)
+            hsv = Analyze.OpticalFlow.draw_hsv(flow)
+            hsv = ims.Image.Convert.BGRtoRGB(hsv)
+            cur_glitch = ims.Image.Convert.BGRtoRGB(cur_glitch)
+
+            bgr = cv.cvtColor(hsv, cv.COLOR_HSV2BGR)
+
+            return hsv, flow, cur_glitch
```

### Comparing `imsis-1.1/imsis/dialogs.py` & `IMSIS-1.1.2/imsis/dialogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             row = table.currentRow()
             print(row)
             dct = eval(properties[row][1])
             actkey = list(dct.keys())[value]
 
             for key, val in dct.items():
                 dct[key] = False
-                if key ==actkey:
+                if key == actkey:
                     dct[key] = True
 
             properties[row][1] = str(dct)
 
         def onButtonClicked():
             allRows = table.rowCount()
             print("")
@@ -193,31 +193,31 @@
                     combo.currentIndexChanged.connect(onComboIndexChanged)
                     # combo.currentIndexChanged.connect(onCurrentIndexChanged)
 
                 else:
                     table.setItem(i, 1, QtWidgets.QTableWidgetItem(item[1]))
             i = i + 1
 
-        #print(highlighted_index)
+        # print(highlighted_index)
 
         # Add Header
         table.setHorizontalHeaderLabels(horHeaders)
 
         # Adjust size of Table, first column adjusted to text, 2nd column adjusted to max 400
         table.resizeColumnsToContents()
         table.resizeRowsToContents()
         w0 = table.columnWidth(0)
         w1 = table.columnWidth(1)
-        w0=int(w0*1.1)
-        w1=int(w1*1.2)
-        #print(w0,w1)
-        if w0>400:
-            w0=400
-        if w1>400:
-            w1=400
+        w0 = int(w0 * 1.1)
+        w1 = int(w1 * 1.2)
+        # print(w0,w1)
+        if w0 > 400:
+            w0 = 400
+        if w1 > 400:
+            w1 = 400
         table.setColumnWidth(0, w0)
         table.setColumnWidth(1, w1)
 
         # Add Table to Grid
         grid.addWidget(table, 0, 0)
 
         lines = len(data)
@@ -227,23 +227,22 @@
 
         Qinfo = QtWidgets.QLabel(info)
 
         okButton = QtWidgets.QPushButton("OK")
         if len(info) != 0:
             grid.addWidget(Qinfo)
         grid.addWidget(okButton)
-        #self.setGeometry(200, 200, 600, newheight)
+        # self.setGeometry(200, 200, 600, newheight)
 
-        #table.setSizeAdjustPolicy(
+        # table.setSizeAdjustPolicy(
         #    QtWidgets.QAbstractScrollArea.AdjustToContents)
 
         table.setSizeAdjustPolicy(
             QtWidgets.QAbstractScrollArea.AdjustToContentsOnFirstShow)
 
-
         self.show()
         self.raise_()
 
         okButton.clicked.connect(onButtonClicked)
 
         return properties
 
@@ -466,37 +465,37 @@
         # self.listView = QtWidgets.QListView()
         self.button_group = QtWidgets.QComboBox()
 
         self.setAttribute(QtCore.Qt.WA_DeleteOnClose)  # stop qtimer assertion when closing
         vbox = QtWidgets.QVBoxLayout(self)
 
         i = 0
-        highlighted_index=0
+        highlighted_index = 0
         # check state of all buttons, prevent that all buttons are disabled, if multiple buttons are selected last one is enabled.
         anybuttonselected = False
         for string, datatype in datalist:
             if datatype == True:
                 anybuttonselected = True
                 highlighted_index = i
             i = i + 1
         if anybuttonselected == False:
             datalist[0][1] = True
 
-        i=0
+        i = 0
         for string, datatype in datalist:
             self.button_group.addItem(string)
             # self.button_group.setId(self.button_name, i)
             # self.button_name.setChecked(datatype)
-            #vbox.addWidget(self.button_group)
+            # vbox.addWidget(self.button_group)
 
             i = i + 1
         vbox.addWidget(self.button_group)
 
-        #highlighted_index=2
-        #print('index', highlighted_index)
+        # highlighted_index=2
+        # print('index', highlighted_index)
         self.button_group.setCurrentIndex(highlighted_index)
 
         Qinfo = QtWidgets.QLabel(info)
 
         self.okButton = QtWidgets.QPushButton('OK')
         self.abortButton = QtWidgets.QPushButton('Abort')
 
@@ -600,15 +599,15 @@
     def dialog_ok_cancel(text, windowtext="Confirm", alwaysontop=True):
         """Dialog ask Ok or Cancel
 
         :Parameters: title, text
         :Returns: result
         """
 
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
 
         window = Window()
         if alwaysontop == True:
             window.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
@@ -629,15 +628,15 @@
         .. code-block:: python
 
             items = collections.OrderedDict([('Left', True), ('Right', False), ('Up', True)]) #ordered
             ret = em.Dialogs.dialog_checklist(items)
             print(ret)
 
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
 
         datalist = []
         for key, val in properties.items():
             datalist.append([key, val])
@@ -676,24 +675,22 @@
     def dialog_dictionary_activeindex(dct):
         """Dialog combobox activekey
 
         retrieve the active key from a combobox in dictionary form
         :Parameters: dictionary
         :Returns: key
         """
-        index=0
+        index = 0
         valfinal = 0
         for key, value in dct.items():
             if value == True:
                 valfinal = index
-            index=index+1
+            index = index + 1
         return valfinal
 
-
-
     @staticmethod
     def dialog_comboboxlist(properties, windowtext="Checklist", info="", alwaysontop=True):
         """Dialog checklist
 
         List of ordered dictionary checkboxes is used such as
         items = collections.OrderedDict([('Left', True), ('Right', False), ('Up', True)]) #ordered
 
@@ -703,15 +700,15 @@
         .. code-block:: python
 
             items = collections.OrderedDict([('Left', True), ('Right', False), ('Up', True)]) #ordered
             ret = em.Dialogs.dialog_checklist(items)
             print(ret)
 
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
 
         datalist = []
         for key, val in properties.items():
             datalist.append([key, val])
@@ -748,15 +745,15 @@
         .. code-block:: python
 
             items = collections.OrderedDict([('Left', True), ('Right', False), ('Up', True)]) #ordered
             ret = em.Dialogs.dialog_checklist(items)
             print(ret)
 
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
 
         datalist = []
         for key, val in properties.items():
             datalist.append([key, val])
@@ -792,15 +789,15 @@
 
             #buttons = {'Left': 1, 'Right': 2, 'Up': 3, 'Down': 4, 'Abort': 5} #unordered, >Python3.7->ordered.
             buttons = OrderedDict([('Left', 1), ('Right', 2), ('Up', 3), ('Down', 4), ('Abort', 5)]) #ordered
             ret = em.Dialogs.dialog_multiplebuttons(buttons)
 
         """
 
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
 
         window = MultiButtonWidget(listbuttons, windowtext, info)
         if alwaysontop == True:
             window.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
@@ -824,15 +821,15 @@
             print(ret,type(ret))
             ret = em.Dialogs.dialog_input("input",'fill in a float',15)
             print(ret,type(ret))
 
         """
         entry_type = type(input)
 
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
         window = Window()
         if alwaysontop == True:
             window.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
 
@@ -867,15 +864,15 @@
 
     @staticmethod
     def message(text, alwaysontop=True):
         """Text message
 
         :Parameters: text
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
         window = Window()
         if alwaysontop == True:
             window.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
 
@@ -883,15 +880,15 @@
 
     @staticmethod
     def textbox(text, windowtext="Textbox", alwaysontop=True):
         """Text message
         This is a multi-line textbox
         :Parameters: text
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
         window = Window()
         window.dialog_textbox(windowtext, text)
         window.setWindowTitle(windowtext)
         if alwaysontop == True:
@@ -903,15 +900,15 @@
 
     @staticmethod
     def textbox_html(text, windowtext="Textbox", alwaysontop=True):
         """Text message
         This is a multi-line textbox, input is a HTML string
         :Parameters: text
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
         window = Window()
         window.dialog_textbox_html(windowtext, text)
         window.setWindowTitle(windowtext)
         if alwaysontop == True:
@@ -923,15 +920,15 @@
 
     @staticmethod
     def error(text, alwaysontop=True):
         """Error message
 
         :Parameters: text
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
         window = Window()
         if alwaysontop == True:
             window.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
 
@@ -948,26 +945,26 @@
 
             properties = {'rows': 3, 'cols':3}
             propertiesafter = em.Dialogs.dialog_propertygrid(properties)
             print(properties)
             print(propertiesafter)
 
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
         window = Window()
         if alwaysontop == True:
             window.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
 
         data = []
         datatypes = []
 
-        #avoid triggering errors due to empty strings
+        # avoid triggering errors due to empty strings
         for k, v in properties.items():
             if v == "":
                 properties.update({k: " "})
 
         for key, val in properties.items():
             data.append([key, str(val)])
             datatypes.append(type(val))
@@ -1001,71 +998,72 @@
                         # changed from int to float
                 else:
                     if (datatypes[row] is float):
                         properties[twi0] = float(twi1)
                     else:
                         if (datatypes[row] is dict):
                             properties[twi0] = eval(twi1)
-                            print('eval:' , eval(twi1))
+                            print('eval:', eval(twi1))
                         else:
                             properties[twi0] = twi1  # not float or int therefore making it string
 
         if (verbose == True):
             print('types: ', st1)
             print('out: ', properties)
         return properties
 
     @staticmethod
-    def openfile_dialog(path='/', windowtext='Open File Dialog',filter="Images (*.png *.jpg *.bmp, *.tif, *.tiff)", alwaysontop=True):
+    def openfile_dialog(path='/', windowtext='Open File Dialog', filter="Images (*.png *.jpg *.bmp, *.tif, *.tiff)",
+                        alwaysontop=True):
         """
         Open file dialog
 
         :Parameters: path, text, filter, alwaysontop
         :Returns: path
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
         window = Window()
         if alwaysontop == True:
             window.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
 
-        filename, _filter = QtWidgets.QFileDialog.getOpenFileName(window, windowtext, path,filter)
+        filename, _filter = QtWidgets.QFileDialog.getOpenFileName(window, windowtext, path, filter)
         return filename
 
     @staticmethod
-    def savefile_dialog(path='/', windowtext='Save File Dialog',filter="Images (*.png *.jpg *.bmp, *.tif, *.tiff)", alwaysontop=True):
+    def savefile_dialog(path='/', windowtext='Save File Dialog', filter="Images (*.png *.jpg *.bmp, *.tif, *.tiff)",
+                        alwaysontop=True):
         """
         Save file dialog
 
         :Parameters: path, text, filter, alwaysontop
         :Returns: path
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
         window = Window()
         if alwaysontop == True:
             window.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
 
         filename, _filter = QtWidgets.QFileDialog.getSaveFileName(window, windowtext, path, filter)
         return filename
 
-
     @staticmethod
     def openfolder_dialog(path='/', windowtext='Open File Dialog', alwaysontop=True):
         """
         Open folder dialog
 
         :Parameters: path, text
         :Returns: path
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
         window = Window()
         if alwaysontop == True:
             window.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
 
@@ -1230,30 +1228,24 @@
                 break
 
         # close all open windows
         cv.destroyAllWindows()
         print("points: {0}".format(pntslist))
         return pntslist
 
+    '''
     @staticmethod
-    def select_lines(img, windowtext="Select Lines"):
+    def select_lines_OLD(img, windowtext="Select Lines"):
         """Draw multiple lines in an image and return (x0,y0,x1,y1) for each rectangle
 
         :Parameters: windowtext=name of form
         :Returns: list of shapes [shapenumber][(x0,y0),(x1,y1)]
         :rtype: object
         """
-        '''
-        fx = 1024 / img.shape[1]
-        if fx < 1:
-            frame = cv.resize(img, None, fx=fx, fy=fx)
-            img0 = frame.copy()  # avoid drawing inside the copy
-        else:
-            img0 = img.copy()
-        '''
+
 
         img0 = img.copy()
         fx = 1
 
         cv.namedWindow(windowtext, cv.WINDOW_AUTOSIZE)
 
         refPt = []
@@ -1307,107 +1299,150 @@
             if cv.getWindowProperty(windowtext, cv.WND_PROP_AUTOSIZE) < 1:
                 break
 
         # close all open windows
         cv.destroyAllWindows()
         print("lines: {0}".format(pntslist))
         return pntslist
+    '''
+
+    @staticmethod
+    def select_lines(img, windowtext="Select Lines"):
+        """Draw multiple lines in an image and return (x0,y0,x1,y1) for each rectangle
+
+        :Parameters: windowtext=name of form
+        :Returns: list of shapes [shapenumber][(x0,y0),(x1,y1)]
+        :rtype: object
+        """
+
+        img0 = img.copy()
+
+        cv.namedWindow(windowtext, cv.WINDOW_AUTOSIZE)
+
+        refPt = []
+        img0 = ims.Image.Convert.toRGB(img0)
+
+        pntslist = []
+
+        def click_and_crop(event, x, y, flags, param):
+            # grab references to the global variables
+            global refPt
+
+            # if the left mouse button was clicked, record the starting
+            # (x, y) coordinates and indicate that cropping is being
+            # performed
+            if event == cv.EVENT_LBUTTONDOWN:
+                refPt = [(x, y)]
+
+            # check to see if the left mouse button was released
+            elif event == cv.EVENT_LBUTTONUP:
+                # record the ending (x, y) coordinates and indicate that
+                # the cropping operation is finished
+                refPt.append((x, y))
+
+                # draw the final line from point 0 to 1
+                cv.line(img0, refPt[0], refPt[1], (0, 255, 0), 2)
+
+                refPt2 = [(int(refPt[0][0] * 1), int(refPt[0][1] * 1)),
+                          (int(refPt[1][0] * 1), int(refPt[1][1] * 1))]
+                pntslist.append(refPt2)
+                cv.imshow(windowtext, img0)
+
+            # check to see if the mouse is moving and the left mouse button is down
+            elif event == cv.EVENT_MOUSEMOVE and flags == cv.EVENT_FLAG_LBUTTON:
+                # draw a temporary line from point 0 to the current mouse position
+                tempImg = img0.copy()
+                cv.line(tempImg, refPt[0], (x, y), (0, 255, 0), 2)
+                cv.imshow(windowtext, tempImg)
+
+            # clone = img0.copy()
+
+        cv.setMouseCallback(windowtext, click_and_crop)
+        cv.imshow(windowtext, img0)
+
+        # keep looping until the 'q' key is pressed
+        while True:
+            # display the image and wait for a keypress
+            key = cv.waitKey(1) & 0xFF
+
+            # monitor escape
+            if key == 27:
+                break
+            if cv.getWindowProperty(windowtext, cv.WND_PROP_AUTOSIZE) < 1:
+                break
+
+        # close all open windows
+        cv.destroyAllWindows()
+        print("lines: {0}".format(pntslist))
+        return pntslist
 
     @staticmethod
     def select_areas(img, windowtext="Select Areas"):
         """
         Draw multiple rectangles in an image and return the position of the rectangles
 
         :Parameters: windowtext=name of form
         :Returns: list of shapes [shapenumber][(x0,y0),(x1,y1)]
         """
 
-        '''
-        fx = 1024 / img.shape[1]
-        if fx < 1:
-            frame = cv.resize(img, None, fx=fx, fy=fx)
-            img0 = frame.copy()  # avoid drawing inside the copy
-        else:
-            img0 = img.copy()
-        '''
-
         img0 = img.copy()
-        zoomfactor = 1
-        fx = zoomfactor
 
-        # print(fx)
         cv.namedWindow(windowtext, cv.WINDOW_AUTOSIZE)
 
         refPt = []
-        cropping = False
         img0 = ims.Image.Convert.toRGB(img0)
 
         pntslist = []
 
         def click_and_crop(event, x, y, flags, param):
             # grab references to the global variables
-            global refPt, cropping
+            global refPt
 
             # if the left mouse button was clicked, record the starting
             # (x, y) coordinates and indicate that cropping is being
             # performed
             if event == cv.EVENT_LBUTTONDOWN:
                 refPt = [(x, y)]
-                cropping = True
 
             # check to see if the left mouse button was released
             elif event == cv.EVENT_LBUTTONUP:
                 # record the ending (x, y) coordinates and indicate that
                 # the cropping operation is finished
                 refPt.append((x, y))
-                cropping = False
 
-                # draw a rectangle around the region of interest
+                # draw the final line from point 0 to 1
                 cv.rectangle(img0, refPt[0], refPt[1], (0, 255, 0), 2)
-                # print(refPt)
-                refPt2 = [(int(refPt[0][0] * 1 / fx), int(refPt[0][1] * 1 / fx)),
-                          (int(refPt[1][0] * 1 / fx), int(refPt[1][1] * 1 / fx))]
-                # print(refPt2)
+
+                refPt2 = [(int(refPt[0][0] * 1), int(refPt[0][1] * 1)),
+                          (int(refPt[1][0] * 1), int(refPt[1][1] * 1))]
                 pntslist.append(refPt2)
                 cv.imshow(windowtext, img0)
 
-        clone = img0.copy()
+            # check to see if the mouse is moving and the left mouse button is down
+            elif event == cv.EVENT_MOUSEMOVE and flags == cv.EVENT_FLAG_LBUTTON:
+                # draw a temporary line from point 0 to the current mouse position
+                tempImg = img0.copy()
+                cv.rectangle(tempImg, refPt[0], (x, y), (0, 255, 0), 2)
+
+                cv.imshow(windowtext, tempImg)
 
-        # cv.namedWindow(windowtext)
         cv.setMouseCallback(windowtext, click_and_crop)
-        zoomfactor = 1
+        cv.imshow(windowtext, img0)
 
         # keep looping until the 'q' key is pressed
         while True:
             # display the image and wait for a keypress
-            cv.imshow(windowtext, img0)
             key = cv.waitKey(1) & 0xFF
 
-            # if the 'r' key is pressed, reset the cropping region
-            if key == ord("r"):
-                img0 = clone.copy()
             # monitor escape
-            elif key == 27:
+            if key == 27:
                 break
             if cv.getWindowProperty(windowtext, cv.WND_PROP_AUTOSIZE) < 1:
                 break
 
-            if key == 43:
-                zoomfactor = zoomfactor * 1.25
-                img0 = cv.resize(img, None, fx=zoomfactor, fy=zoomfactor)
-                fx = zoomfactor
-            if key == 45:
-                zoomfactor = zoomfactor * 0.75
-                img0 = cv.resize(img, None, fx=zoomfactor, fy=zoomfactor)
-                fx = zoomfactor
-            if key == 114:
-                zoomfactor = 1
-                img0 = cv.resize(img, None, fx=zoomfactor, fy=zoomfactor)
-                fx = zoomfactor
-
         # close all open windows
         cv.destroyAllWindows()
         print("areas: {0}".format(pntslist))
         return pntslist
 
     @staticmethod
     def adjust_mask(img, windowtext="Select Mask"):
@@ -1460,30 +1495,37 @@
 
         cv.destroyAllWindows()
         print("Mask: thresholdedimage, Min={},Max={},Blur={}".format(min, max, blur))
         thresh1 = subfunction(img, min, max, blur)
         return thresh1, min, max, blur
 
     @staticmethod
-    def adjust_mask_with_background(img, windowtext="Select Mask"):
+    def adjust_mask_with_overlay(img, windowtext="Select Mask", text="Zoom +/-/r Hide h"):
         """create an image mask by setting the intensity range and blur. Returns: image, min,max,blur
         zoom in/out with +/-, reset zoom with r
         hide/unhide mask with h
         :Parameters: image, windowtext=name of form
-        :Returns: ImageOut, Min,Max,Blur
+        :Returns: Image_Thresholded, Min,Max,Blur
         """
 
         def subfunction(img, min, max, blur, zoomfactor, hidemask):
             img = cv.resize(img, None, fx=zoomfactor, fy=zoomfactor)
             imout = cv.GaussianBlur(img, (blur, blur), 0)
             thresh0 = cv.inRange(imout, min, max)
-            thresh1 = ims.Image.Process.Falsecolor.falsecolor_merge2channels(thresh0, imout)
+            thresh1 = ims.Image.Process.Falsecolor.falsecolor_merge2channels(thresh0, img)
             if hidemask == True:
                 thresh1 = img
+            if text:
+                thresh1 = ims.Analyze.add_text(thresh1, 0, 0, text, fontsize=20)
+
+            return thresh1
 
+        def subfunction_final(img, min, max, blur):
+            imout = cv.GaussianBlur(img, (blur, blur), 0)
+            thresh1 = cv.inRange(imout, min, max)
             return thresh1
 
         def nothing(x):
             pass
 
         fx = 1024 / img.shape[1]
         if fx < 1:
@@ -1496,21 +1538,30 @@
         cv.createTrackbar("Min", windowtext, 32, 255, nothing)
         cv.createTrackbar("Max", windowtext, 128, 255, nothing)
         cv.createTrackbar("Blur", windowtext, 1, 50, nothing)
 
         zoomfactor = 1
         hidemask = False
 
+        minlast = 0
+        maxlast = 0
+        blurlast = 0
+
         while (1):
             min = cv.getTrackbarPos("Min", windowtext)
             max = cv.getTrackbarPos("Max", windowtext)
             blur = cv.getTrackbarPos("Blur", windowtext)
             if (blur % 2 == 0):
                 blur = blur + 1
-            thresh1 = subfunction(frame, min, max, blur, zoomfactor, hidemask)
+
+            if (min != minlast) or (max != maxlast) or (blur != blurlast):
+                minlast = min
+                maxlast = max
+                blurlast = blur
+                thresh1 = subfunction(frame, min, max, blur, zoomfactor, hidemask)
 
             cv.imshow(windowtext, thresh1)
             k = cv.waitKey(1) & 0xFF
             if k == 27:
                 break
             if cv.getWindowProperty(windowtext, cv.WND_PROP_AUTOSIZE) < 1:
                 break
@@ -1524,18 +1575,126 @@
                 if hidemask == True:
                     hidemask = False
                 else:
                     hidemask = True
 
         cv.destroyAllWindows()
         print("MaskWithBackground: thresholdedimage, Min={},Max={},Blur={}".format(min, max, blur))
-        thresh1 = subfunction(img, min, max, blur, zoomfactor=1, hidemask=False)
+        # thresh1 = subfunction(img, min, max, blur, zoomfactor=1, hidemask=False)
+        thresh1 = subfunction_final(img, min, max, blur)
         return thresh1, min, max, blur
 
     @staticmethod
+    def adjust_contours_after_masking(img, min, max, blur, windowtext="Select Mask", text="Zoom +/-/r Hide h"):
+        """Adjust the settings for contours after masking
+        zoom in/out with +/-, reset zoom with r
+        hide/unhide mask with h
+        :Parameters: image, windowtext=name of form
+        :Returns: Image_Thresholded, Min,Max,Blur
+        """
+
+        def subfunction(img, min, max, blur, minArea, maxArea, dt, zoomfactor, hidemask):
+            if minArea >= maxArea:
+                minArea = maxArea - 1  # avoid division by 0
+            # img = cv.resize(img, None, fx=zoomfactor, fy=zoomfactor)
+            imout = cv.GaussianBlur(img, (blur, blur), 0)
+            thresh0 = cv.inRange(imout, min, max)
+            # thresh1 = ims.Image.Process.Falsecolor.falsecolor_merge2channels(thresh0, img)
+            fn = 'overlay.png'
+            print(min, max, blur, minArea, maxArea, dt)
+            try:
+                overlay, labels, markers, featurelist = ims.Analyze.FeatureProperties.get_featureproperties(img,
+                                                                                                            thresh0,
+                                                                                                            minarea=minArea,
+                                                                                                            maxarea=maxArea,
+                                                                                                            applydistancemap=True,
+                                                                                                            distance_threshold=dt / 100)
+                overlay2 = ims.Analyze.FeatureProperties.get_image_with_ellipses(overlay, featurelist)
+            except:
+                print("Error")
+                overlay2 = img.copy()
+
+            return overlay2
+
+        def subfunction_final(img, min, max, blur, minArea, maxArea, dt):
+            print("final ", min, max, blur, minArea, maxArea, dt)
+            imout = cv.GaussianBlur(img, (blur, blur), 0)
+            thresh0 = cv.inRange(imout, min, max)
+            overlay, labels, markers, featurelist = ims.Analyze.FeatureProperties.get_featureproperties(img,
+                                                                                                        thresh0,
+                                                                                                        minarea=minArea,
+                                                                                                        maxarea=maxArea,
+                                                                                                        applydistancemap=True,
+                                                                                                        distance_threshold=dt / 100)
+            return overlay
+
+        def nothing(x):
+            pass
+
+        def resizeimg(img):
+            fx = 1024 / img.shape[1]
+            if fx < 1:
+                frame = cv.resize(img, None, fx=fx, fy=fx)
+            else:
+                frame = img.copy()
+            return frame
+
+        frame = img.copy()
+        orig = img.copy()
+        maxarealimit = int(img.shape[0] * img.shape[1] * 0.1)
+
+        cv.namedWindow(windowtext, cv.WINDOW_AUTOSIZE)
+
+        cv.createTrackbar("MinArea", windowtext, 200, maxarealimit, nothing)
+        cv.createTrackbar("MaxArea", windowtext, 1500, maxarealimit, nothing)
+        cv.createTrackbar("DistanceThreshold", windowtext, 1, 100, nothing)
+
+        zoomfactor = 1
+        hidemask = False
+
+        minArealast = 0
+        maxArealast = 0
+        dtlast = 0
+
+        while (1):
+            minArea = cv.getTrackbarPos("MinArea", windowtext)
+            maxArea = cv.getTrackbarPos("MaxArea", windowtext)
+            dt = cv.getTrackbarPos("DistanceThreshold", windowtext)
+
+            if (dt != dtlast) or (minArea != minArealast) or (maxArea != maxArealast):
+                thresh1 = subfunction(frame, min, max, blur, minArea, maxArea, dt, zoomfactor, hidemask)
+                minArealast = minArea
+                maxArealast = maxArea
+                dtlast = dt
+
+            cv.imshow(windowtext, resizeimg(thresh1))
+            k = cv.waitKey(1) & 0xFF
+            if k == 27:
+                break
+            if cv.getWindowProperty(windowtext, cv.WND_PROP_AUTOSIZE) < 1:
+                break
+            if k == 43:
+                zoomfactor = zoomfactor * 1.25
+            if k == 45:
+                zoomfactor = zoomfactor * 0.75
+            if k == 114:
+                zoomfactor = 1
+            if k == 104:
+                if hidemask == True:
+                    hidemask = False
+                else:
+                    hidemask = True
+
+        cv.destroyAllWindows()
+        print("MaskWithBackground: thresholdedimage, Min={},Max={},Blur={}".format(min, max, blur))
+        print("final ", min, max, blur, minArea, maxArea, dt, minArealast, maxArealast, dtlast)
+        overlay = subfunction_final(orig, min, max, blur, minArea, maxArea, dt)
+        return overlay, minArea, maxArea, dt / 100
+
+    @staticmethod
     def select_edges(img, windowtext="Select Edges"):
         """Find all edges in image. Returns: threshold image, threshold value,blur
 
         :Parameters: windowtext=name of form
         :Returns: ImageOut, Threshold, Blur
 
         .. code-block:: python
@@ -2082,15 +2241,15 @@
     @staticmethod
     def dialog_imagelistview(windowtext="Drag and drop image dialog", alwaysontop=True):
         """
         Image listview dialog. The listview allows for dragging dropping and thumbnail previewing of files.
 
         :Returns: list of urls
         """
-        #workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
+        # workaround to avoid multiple instances of QtWidget causing memory leaks, required for QT5.14.2, better method available?
         app = QtCore.QCoreApplication.instance()
         if app is None:
             app = QtWidgets.QApplication(sys.argv)
         window = ImageListViewForm()
 
         if alwaysontop == True:
             window.setWindowFlags(QtCore.Qt.WindowStaysOnTopHint)
```

### Comparing `imsis-1.1/imsis/image.py` & `IMSIS-1.1.2/imsis/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import matplotlib.gridspec as gridspec
 import numpy as np
 import scipy.misc
 from matplotlib import pyplot as plt
 import numpy.random as random
 from matplotlib.colors import hsv_to_rgb
 from datetime import datetime
+from scipy import ndimage
+
 
 
 class Image(object):
 
     @staticmethod
     def load(filename, verbose=True):
         """Load image
@@ -148,24 +150,25 @@
         (aMean, aStd) = (a.mean(), a.std())
         (bMean, bStd) = (b.mean(), b.std())
 
         # return the color statistics
         return (lMean, lStd, aMean, aStd, bMean, bStd)
 
     @staticmethod
-    def save(img, fn):
+    def save(img, fn, verbose=True):
         """Save image (PNG,TIF)
 
         :Parameters: image, filename
         """
         try:
             if (os.path.dirname(fn)):
-               os.makedirs(os.path.dirname(fn), exist_ok=True) #mkdir if not empty
+                os.makedirs(os.path.dirname(fn), exist_ok=True)  # mkdir if not empty
             cv.imwrite(fn, img)
-            print("file saved. ", fn)
+            if verbose == True:
+                print("file saved. ", fn)
         except:
             print("Error: cannot save file {}".format(fn))
 
     @staticmethod
     def save_withuniquetimestamp(img):
         """Save PNG image with unique timestamp.
 
@@ -252,15 +255,15 @@
         """add 2 images weighted (default alpha=0.5)
         :Parameters: image1, image2, alpha
         :Returns: image
         """
         a = img0
         b = img1
         beta = 1 - alpha
-        gamma=0
+        gamma = 0
         out = cv.addWeighted(a, alpha, b, beta, gamma)
         return out
 
     @staticmethod
     def new(height, width):
         """Create a new blank image
 
@@ -284,17 +287,15 @@
 
     @staticmethod
     def info(img):
         """get image properties
 
         :Parameters: img
         """
-        print(img.shape)
-        print(img.size)
-        print(img.dtype)
+        print("{}, {}, {}".format(img.shape, img.size, img.dtype))
 
     @staticmethod
     def unique_colours(image):
         """get number of unique colors in an image
 
         :Parameters: img
         """
@@ -310,63 +311,14 @@
             out_in_32U_2D = np.int32(image)  # bit wise shift 8 for each channel.
             out_in_32U_1D = out_in_32U_2D.reshape(-1)  # convert to 1D
             np.unique(out_in_32U_1D)
             out = len(np.unique(out_in_32U_1D))
         print(out)
         return out
 
-    @staticmethod
-    def video_to_imagesondisk(file_in='video.avi', path_out='images'):
-        """video to image
-
-        :Parameters: video_filename
-        :Returns: images
-        """
-        video_file = file_in
-        output_folder = path_out
-        vidcap = cv.VideoCapture(video_file)
-        success, image = vidcap.read()
-        count = 0
-        success = True
-        while success:
-            fn = output_folder + "/" + "frame%d.png" % count
-            cv.imwrite(fn, image)  # save frame as JPEG file
-            success, image = vidcap.read()
-            print('Read a new frame: ', success, fn)
-            count += 1
-        print("ready.")
-
-    @staticmethod
-    def imagesfromdisk_to_video(path_in, file_out='video.avi', framerate=15):
-        """images from file to video
-
-        :Parameters: path with list of frames
-        :Returns: video
-        """
-        image_folder = path_in
-        video_name = file_out
-
-        output_folder = "output"
-
-        fn = image_folder + "/" + output_folder + "/"
-        print(fn)
-        os.makedirs(os.path.dirname(fn), exist_ok=True)
-
-        images = [img for img in os.listdir(image_folder) if (img.endswith(".tif") or img.endswith(".png"))]
-        frame = cv.imread(os.path.join(image_folder, images[0]))
-        height, width, layers = frame.shape
-
-        video = cv.VideoWriter(fn + video_name, 0, framerate, (width, height))
-
-        for image in images:
-            video.write(cv.imread(os.path.join(image_folder, image)))
-
-        cv.destroyAllWindows()
-        video.release()
-
     '''
     @staticmethod
     def zoom(image0, factor=2):
         """
         zoom image, resize with factor n, crop in center to same size as original image
         :Parameters: image0, zoom factor
         :Returns: image
@@ -493,14 +445,16 @@
             grad = np.power(np.power(im3h, 2.0) + np.power(im3v, 2.0), 0.5)
             theta = np.arctan2(im3v, im3h)
             thetaQ = (np.round(theta * (5.0 / np.pi)) + 5) % 5  # Quantize direction
 
             gradSup = nonmaxsuppression(im, grad)
             return gradSup, thetaQ
 
+
+
         @staticmethod
         def nonlocalmeans(img, h=10, templatewindowsize=7, searchwindowsize=21):
             """Apply a non-local-means filter with filtering strength (h), template windowsize (blocksize), searchwindowsize
             :Parameters: image, h=10, templatewindowsize=7, searchwindowsize=21
             :Returns: image
             """
 
@@ -621,24 +575,26 @@
             img_back = np.fft.ifft2(back_ishift, axes=(0, 1))
             img_back = np.abs(img_back).clip(0, 255).astype(np.uint8)
 
             return img_back
 
         @staticmethod
         def FD_bandpass_filter(img, D0=5, w=10, bptype=0):
+            if D0 < 1:
+                D0 = 1
 
             gray = Image.Convert.toGray(img)
-            kernel = Image.FilterKernels.ideal_bandpass_kernel(gray, D0, w)
+            gray_fft = np.fft.fft2(gray)
+            gray_fftshift = np.fft.fftshift(gray_fft)
             if bptype == 1:
                 kernel = Image.FilterKernels.gaussian_bandpass_kernel(gray, D0, w)
             elif bptype == 2:
                 kernel = Image.FilterKernels.butterworth_bandpass_kernel(gray, D0, w)
-            gray = np.float64(gray)
-            gray_fft = np.fft.fft2(gray)
-            gray_fftshift = np.fft.fftshift(gray_fft)
+            else:
+                kernel = Image.FilterKernels.ideal_bandpass_kernel(gray, D0, w)
             dst_filtered = np.multiply(kernel, gray_fftshift)
             dst_ifftshift = np.fft.ifftshift(dst_filtered)
             dst_ifft = np.fft.ifft2(dst_ifftshift)
             dst = np.abs(np.real(dst_ifft))
             dst = np.clip(dst, 0, 255)
             out = np.uint8(dst)
             return out, kernel
@@ -917,14 +873,16 @@
             noise_img = img.astype(np.float)
             stddev = prob * 100.0
             noise = np.random.randn(*img.shape) * stddev
             noise_img += noise
             noise_img = np.clip(noise_img, 0, 255).astype(np.uint8)
             return noise_img
 
+        '''
+        #slow method
         @staticmethod
         def salt_and_pepper_noise(image, prob=0.01):
             """Add salt and pepper noise
 
             :Parameters: image, sigma=0.01
             :Returns: image
             """
@@ -936,14 +894,32 @@
                     if rdn < prob:
                         output[i][j] = 0
                     elif rdn > thres:
                         output[i][j] = 255
                     else:
                         output[i][j] = image[i][j]
             return output
+        '''
+
+        def salt_and_pepper_noise(img, prob=0.01):
+            """Add salt and pepper noise to an image
+
+            :Parameters:
+                - image: numpy array of shape (height, width, channels)
+                - prob: probability of adding noise (default is 0.01)
+
+            :Returns: image with added noise
+            """
+            out = img.copy()
+
+            black, white = np.array([0, 0, 0], dtype='uint8'), np.array([255, 255, 255], dtype='uint8')
+            probs = np.random.random(out.shape[:2])
+            out[probs < (prob / 2)] = black
+            out[probs > 1 - (prob / 2)] = white
+            return out
 
         @staticmethod
         def poisson_noise(img, prob=0.25):
             """ Induce poisson noise
 
             :Parameters: image, lambda=0.25
             :Returns: image
@@ -1097,14 +1073,141 @@
 
                 r0, g0, b0 = cv.split(img0)
                 r1, g1, b1 = cv.split(img1)
                 r2, g2, b2 = cv.split(img2)
                 img3 = cv.merge([b2, g1, r0])
                 return img3
 
+            @staticmethod
+            def grayscale_to_color(img, color):
+                """ colorize a grayscale image by a given color
+                :Parameters: image, color
+                :Returns: image
+                """
+
+                # Add a small value to grayscale image
+                gray_img = img.copy()
+                # gray_img += 1
+
+                # Normalize grayscale image to the range [0, 255]
+                # gray_img = cv.normalize(gray_img, None, 0, 255, cv.NORM_MINMAX, cv.CV_8U)
+
+                # Create color image
+                color_img = np.zeros((gray_img.shape[0], gray_img.shape[1], 3), dtype=np.uint8)
+                color_img[:, :, 0] = color[0]
+                color_img[:, :, 1] = color[1]
+                color_img[:, :, 2] = color[2]
+                color_img = color_img.astype(np.uint8) * gray_img[:, :, np.newaxis].astype(np.uint8)
+
+                return color_img
+
+        @staticmethod
+        def gradient_removal(img, filtersize=513, sigmaX=32):
+            """Remove Image gradient
+            :Parameters: image, filtersize, sigmaX
+            :Returns: image
+            """
+
+            gray = Image.Convert.toGray(img)
+            gaussianImg = cv.GaussianBlur(gray, (filtersize, filtersize), sigmaX=sigmaX)
+            img = (gray - gaussianImg)
+            img = Image.Adjust.invert(img)
+
+            return img
+
+        @staticmethod
+        def replace_black_pixels_by_median(img):
+            """Replace black pixels by the median of neighbours
+
+            :Parameters: image
+            :Returns: image
+            """
+
+            # Make mask of black pixels, True where black
+            # Define a threshold to consider a pixel as black
+            black_threshold = 20
+
+            # Create a binary mask of black pixels, where True means black
+            blackMask = np.all(img < black_threshold, axis=-1)
+
+            # blackMask = np.all(img == 0, axis=-1)
+            median = cv.medianBlur(img, 3)
+            res = np.where(blackMask[..., None], median, img)
+            return res
+
+        def replace_black_pixels_using_nonlocalmeans(img):
+            """Replace black pixels by nonlocalmeans filtering
+
+            :Parameters: image
+            :Returns: image
+            """
+            # Define a threshold to consider a pixel as black
+            black_threshold = 20
+
+            # Create a binary mask of black pixels, where True means black
+            black_mask = np.all(img < black_threshold, axis=-1)
+
+            # Create a copy of the image to modify only black pixels
+            img_copy = img.copy()
+
+            # Apply Gaussian blur to black pixels
+            blurred = cv.GaussianBlur(img_copy, (5, 5), 0)
+            blurred[~black_mask] = img[~black_mask]
+
+            # Apply non-local means denoising to black pixels
+            denoised = cv.fastNlMeansDenoisingColored(blurred, None, 10, 10, 7, 21)
+            denoised[~black_mask] = img[~black_mask]
+
+            # Apply morphological operations to black pixels
+            kernel = np.ones((3, 3), np.uint8)
+            cleaned = cv.morphologyEx(denoised, cv.MORPH_CLOSE, kernel)
+            cleaned[~black_mask] = img[~black_mask]
+            return cleaned
+
+        '''
+        @staticmethod
+        def noise_reduction_thresholded(img):
+            """Replace black pixels by the median of neighbours
+
+            :Parameters: image
+            :Returns: image
+            """
+
+            threshold = 1
+            _, thresh = cv.threshold(cv.cvtColor(img, cv.COLOR_BGR2GRAY), threshold, 255, cv.THRESH_BINARY)
+
+            # Find the contours of the noisy regions
+            contours, _ = cv.findContours(thresh, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
+
+            # Draw a black mask on the noisy regions
+            mask = np.zeros_like(img)
+            cv.drawContours(mask, contours, -1, (0, 0, 0), -1)
+
+            # Remove the noisy regions by applying the mask on the image
+            result = cv.bitwise_and(img, mask)
+
+            return result
+        '''
+
+        @staticmethod
+        def remove_islands_colour(img, kernel=13):
+            """Remove islands in a colour image using a kernel
+
+            :Parameters: image, kernel=13
+            :Returns: image
+            """
+            # Convert the image to grayscale
+            gray = Image.Convert.toGray(img)
+
+            blur = cv.GaussianBlur(gray, (kernel, kernel), 0)
+            thresh = cv.threshold(blur, 100, 255, cv.THRESH_BINARY)[1]
+            # Remove the noisy regions by applying the mask on the image
+            result = cv.bitwise_and(img, img, mask=thresh)
+            return result
+
     class Adjust:
         @staticmethod
         def invert(img):
             """Invert image
 
             :Parameters: image
             :Returns: image
@@ -1507,15 +1610,15 @@
                 if zeros == size:
                     done = True
             return skel
 
         # Zhang-Suen Thinning Algorithm - https://github.com/linbojin/Skeletonization-by-Zhang-Suen-Thinning-Algorithm
         # note: slow filter
         @staticmethod
-        def thinning(img):
+        def zhang_suen_thinning(img):
             """Applies the Zhang-Suen thinning algorithm.
 
             :Parameters: image
             :Returns: image
             """
 
             def neighbours(x, y, img):
@@ -1562,14 +1665,64 @@
                                 P2 * P4 * P8 == 0 and  # Condition 3
                                 P2 * P6 * P8 == 0):  # Condition 4
                             changing2.append((x, y))
                 for x, y in changing2:
                     img_Thinned[x][y] = 0
             return img_Thinned
 
+        '''
+        @staticmethod
+        def zhang_suen_thinning2(img):
+
+            def neighbours_vec(image):
+                return image[2:, 1:-1], image[2:, 2:], image[1:-1, 2:], image[:-2, 2:], image[:-2, 1:-1], image[:-2,
+                                                                                                          :-2], image[
+                                                                                                                1:-1,
+                                                                                                                :-2], image[
+                                                                                                                      2:,
+                                                                                                                      :-2]
+
+            def transitions_vec(P2, P3, P4, P5, P6, P7, P8, P9):
+                return ((P3 - P2) > 0).astype(int) + ((P4 - P3) > 0).astype(int) + \
+                       ((P5 - P4) > 0).astype(int) + ((P6 - P5) > 0).astype(int) + \
+                       ((P7 - P6) > 0).astype(int) + ((P8 - P7) > 0).astype(int) + \
+                       ((P9 - P8) > 0).astype(int) + ((P2 - P9) > 0).astype(int)
+
+            def zhangSuen_vec(image, iterations):
+                for iter in range(1, iterations):
+                    # step 1
+                    P2, P3, P4, P5, P6, P7, P8, P9 = neighbours_vec(image)
+                    condition0 = image[1:-1, 1:-1]
+                    condition4 = P4 * P6 * P8
+                    condition3 = P2 * P4 * P6
+                    condition2 = transitions_vec(P2, P3, P4, P5, P6, P7, P8, P9) == 1
+                    condition1 = (2 <= P2 + P3 + P4 + P5 + P6 + P7 + P8 + P9) * (
+                                P2 + P3 + P4 + P5 + P6 + P7 + P8 + P9 <= 6)
+                    cond = (condition0 == 1) * (condition4 == 0) * (condition3 == 0) * (condition2 == 1) * (
+                                condition1 == 1)
+                    changing1 = np.where(cond == 1)
+                    image[changing1[0] + 1, changing1[1] + 1] = 0
+                    # step 2
+                    P2, P3, P4, P5, P6, P7, P8, P9 = neighbours_vec(image)
+                    condition0 = image[1:-1, 1:-1]
+                    condition4 = P2 * P6 * P8
+                    condition3 = P2 * P4 * P8
+                    condition2 = transitions_vec(P2, P3, P4, P5, P6, P7, P8, P9) == 1
+                    condition1 = (2 <= P2 + P3 + P4 + P5 + P6 + P7 + P8 + P9) * (
+                                P2 + P3 + P4 + P5 + P6 + P7 + P8 + P9 <= 6)
+                    cond = (condition0 == 1) * (condition4 == 0) * (condition3 == 0) * (condition2 == 1) * (
+                                condition1 == 1)
+                    changing2 = np.where(cond == 1)
+                    image[changing2[0] + 1, changing2[1] + 1] = 0
+                return image
+
+            image = zhangSuen_vec(img, 1)
+            return image
+        '''
+
         @staticmethod
         def morphology_erode(img, kernel=5):
             """Morphology filter - erode
 
             :Parameters: image, kernel
             :Returns: image
             """
@@ -1658,14 +1811,15 @@
         @staticmethod
         def remove_islands(img0, min_size=150):
             """Remove islands in an image
 
             :Parameters: image, min_size=150
             :Returns: image
             """
+
             # find all your connected components (white blobs in your image)
             nb_components, output, stats, centroids = cv.connectedComponentsWithStats(img0, connectivity=8)
             # connectedComponentswithStats yields every seperated component with information on each of them, such as size
             # the following part is just taking out the background which is also considered a component, but most of the time we don't want that.
             sizes = stats[1:, -1]
             nb_components = nb_components - 1
 
@@ -1833,28 +1987,48 @@
             d = np.power(c, 2.0) + np.power(r, 2.0)
             kernel_matrix = np.zeros((rows, cols), np.float32)
             kernel = 1.0 / (1 + np.power(np.sqrt(d) / radius, 2 * n))
             kernel_matrix[:, :] = kernel
             return kernel_matrix
 
         @staticmethod
-        def ideal_bandpass_kernel(img, D0=32, w=9):
-            rows, cols = img.shape
+        def ideal_bandpass_kernel2(img, D0=32, w=9):
+            rows, cols = img.shape[:2]
             crow, ccol = int(rows / 2), int(cols / 2)
             mask = np.ones((rows, cols), np.uint8)
             for i in range(0, rows):
                 for j in range(0, cols):
                     d = np.sqrt(pow(i - crow, 2) + pow(j - ccol, 2))
                     if D0 - w / 2 < d < D0 + w / 2:
                         mask[i, j] = 1
                     else:
                         mask[i, j] = 0
             kernel = mask
             return kernel
 
+        def ideal_bandpass_kernel(img, D0=32, w=9):
+            rows, cols = img.shape[:2]
+            crow, ccol = rows // 2, cols // 2
+
+            # Create a meshgrid of row and column indices
+            rows_idx, cols_idx = np.ogrid[:rows, :cols]
+
+            # Calculate the distance from the center of the image
+            distance = np.sqrt((rows_idx - crow) ** 2 + (cols_idx - ccol) ** 2)
+
+            # Create a mask with ones within the specified distance from the center
+            mask = np.zeros((rows, cols), np.uint8)
+            mask[(distance >= D0 - w / 2) & (distance <= D0 + w / 2)] = 1
+
+            resized_kernel = cv.resize(mask, (img.shape[1], img.shape[0]))
+
+            # Multiply the mask with the bandpass kernel to create the final kernel
+            kernel = mask * resized_kernel
+            return kernel
+
         @staticmethod
         def ideal_bandstop_kernel(img, D0=32, W=9):
             kernel = 1.0 - Image.FilterKernels.ideal_bandpass_kernel(img, D0, W)
             return kernel
 
         @staticmethod
         def gaussian_bandstop_kernel(img, D0=32, W=9):
@@ -2348,15 +2522,15 @@
             # Mask input image with binary mask
             result = cv.bitwise_and(img, mask)
             # Color background white
             # result[mask == 0] = 255  # Optional
             return result
 
         @staticmethod
-        def imageregistration(img1, img2,verbose=False):
+        def imageregistration(img1, img2, verbose=False):
             """
             Register 2 images using opencv ORB (Oriented FAST and rotated BRIEF)
             Initiate ORB detector
 
             :Parameters: img1, img2
             :Returns: image
             """
@@ -2376,15 +2550,15 @@
                 if m.distance < 0.7 * n.distance:
                     rawMatches.append(m)
 
             sortMatches = sorted(rawMatches, key=lambda x: x.distance)
             matches = sortMatches[0:128]
 
             img3 = cv.drawMatches(img1, kp1, img2, kp2, matches[:100], None, flags=2)
-            if verbose==True:
+            if verbose == True:
                 cv.imshow("Feature descriptor matching", img3)
                 cv.waitKey(0)
 
             image_1_points = np.zeros((len(matches), 1, 2), dtype=np.float32)
             image_2_points = np.zeros((len(matches), 1, 2), dtype=np.float32)
 
             for i in range(0, len(matches)):
@@ -2460,7 +2634,138 @@
                 new_img[:hb, wa:wa + wb, ] = imgb
 
             # dist2 = cv.convertScaleAbs(new_img)
             dist2 = cv.normalize(new_img, None, 255, 0, cv.NORM_MINMAX, cv.CV_8UC1)
             # dist2 = new_img
 
             return dist2
+
+        @staticmethod
+        def video_to_imagesondisk(file_in='video.avi', path_out='images'):
+            """video to image
+
+            :Parameters: video_filename
+            :Returns: images
+            """
+            video_file = file_in
+            output_folder = path_out
+            vidcap = cv.VideoCapture(video_file)
+            success, image = vidcap.read()
+            count = 0
+            success = True
+            while success:
+                fn = output_folder + "/" + "frame%d.png" % count
+                cv.imwrite(fn, image)  # save frame as JPEG file
+                success, image = vidcap.read()
+                print('Read a new frame: ', success, fn)
+                count += 1
+            print("ready.")
+
+        @staticmethod
+        def imagesfromdisk_to_video(path_in, file_out='video.avi', framerate=15):
+            """images from file to video
+
+            :Parameters: path with list of frames
+            :Returns: video
+            """
+            image_folder = path_in
+            video_name = file_out
+
+            output_folder = "output"
+
+            fn = image_folder + "/" + output_folder + "/"
+            print(fn)
+            os.makedirs(os.path.dirname(fn), exist_ok=True)
+
+            images = [img for img in os.listdir(image_folder) if (img.endswith(".tif") or img.endswith(".png"))]
+            frame = cv.imread(os.path.join(image_folder, images[0]))
+            height, width, layers = frame.shape
+
+            video = cv.VideoWriter(fn + video_name, 0, framerate, (width, height))
+
+            for image in images:
+                video.write(cv.imread(os.path.join(image_folder, image)))
+
+            cv.destroyAllWindows()
+            video.release()
+
+        @staticmethod
+        def _get_dominant_color(img):
+            """ Return dominant color in an image
+            :Parameters: image
+            :Returns: color
+            """
+            if len(img.shape) == 3:
+                colors, count = np.unique(img.reshape(-1, img.shape[-1]), axis=0, return_counts=True)
+                out = (colors[count.argmax()]).tolist()
+            else:
+                colors, count = np.unique(img.reshape(-1, 1), axis=0, return_counts=True)
+                out = (colors[count.argmax()]).tolist()
+            return out
+
+        @staticmethod
+        def intensity_compensation_per_line(img):
+            """intensity compensation per line
+
+            :Parameters: image
+            :Returns: image
+            """
+
+            '''
+            def histogram(img, range=None, step=0.1, order=None, smoothed=False, smoothing_order=1, mask=None):
+                round_min = lambda x, step: round(x - x % step, 3)
+                round_max = lambda x, step: round(x - x % step + step, 3)
+
+                if not mask is None:
+                    unmasked = np.where(mask != 0.0)
+                    unmasked = list(zip(*unmasked))
+                    data = img
+                    data = np.array([data[y, x] for y, x in unmasked])
+                else:
+                    # data = img.data.flatten()
+                    data = img.flatten()
+
+                if range is None:
+                    range = [round_min(data.min(), step), round_max(data.max(), step)]
+                elif len(range) == 2:
+                    range = [round_min(range[0], step), round_max(range[1], step)]
+                else:
+                    raise ValueError
+                bins = int((range[1] - range[0]) / step)
+                hist, hist_bins = np.histogram(data, bins=bins, range=range)
+                if smoothed:
+                    kernel = cv2.getGaussianKernel(smoothing_order, 0)[:, 0]
+                    hist = np.convolve(hist, kernel, mode='same')
+                if order is None:
+                    order = int(round(1 / step))
+                peaks = signal.argrelmax(hist, order=order)[0]
+
+                return hist, hist_bins[:-1], peaks
+
+            def heightcorrection0(src, makeItZero=False, peak_num=21, step=0.1):
+                dst = src.copy()
+                hist, bins, peak_idx = histogram(dst, step=step)
+                peak = bins[peak_idx[peak_num - 1]]
+                dst = dst - peak
+                if makeItZero:
+                    black = np.zeros_like(dst, dtype='uint8')
+                    dst = np.where(dst >= 0.0, dst, black)
+                return dst
+            '''
+
+            col = Image.Tools._get_dominant_color(img)
+            img2 = Image.Convert.toGray(img)
+            img2 = cv.normalize(img2, None, 0, 255, cv.NORM_MINMAX, cv.CV_8U)
+
+            # calculate the mean intensity of each line
+            mean_intensities = np.mean(img2, axis=1)
+            # subtract the mean intensity from each line
+            res = img2 - mean_intensities[:, np.newaxis]
+            res = cv.normalize(res, None, 0, 255, cv.NORM_MINMAX, cv.CV_8U)
+
+            # Apply binary threshold to detect bright pixels
+            _, thresh = cv.threshold(img2, 0, 128, cv.THRESH_BINARY)
+            # Invert binary image
+            # Multiply binary image with grayscale image to remove bright pixels
+            res = cv.bitwise_and(res, thresh)
+            res = Image.Process.Falsecolor.grayscale_to_color(res, col)
+            return res
```

### Comparing `imsis-1.1/imsis/imagestack.py` & `IMSIS-1.1.2/imsis/imagestack.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,297 +14,375 @@
 import cv2 as cv
 import matplotlib.gridspec as gridspec
 import numpy as np
 import scipy.misc
 from matplotlib import pyplot as plt
 import numpy.random as random
 import imsis as ims
+import numpy.random as random
+
 
 class ImageStack:
-        @staticmethod
-        def to_video(image_list, file_out=r'video.avi', framerate=15):
-            """image list (in memory) to video
-
-            :Parameters: image_list
-            :Returns: video
-            """
-
-            os.makedirs(os.path.dirname(file_out), exist_ok=True)
-
-            frame = image_list[0]
-            height, width = frame.shape[0], frame.shape[1]
-
-            video = cv.VideoWriter(file_out, 0, framerate, (width, height))
-
-            for image in image_list:
-                image = ims.Image.Convert.toRGB(image)
-                video.write(image)
-            cv.destroyAllWindows()
-            video.release()
-
-        @staticmethod
-        def play(image_list, framerate=15, verbose=True):
-            """view image list (in memory)
-            """
-            window_name = 'Imagestack'
-            wk = int(1000 / framerate)
-            if wk < 1:
-                wk = 1
-            if verbose==True:
-                print("imagestack play: delay per frame in ms {}".format(wk))
-
-            cv.imshow(window_name, image_list[0])
-            cv.moveWindow(window_name, 0, 0)
-
-            for image in image_list:
-                image = ims.Image.Convert.toRGB(image)
-                cv.imshow(window_name, image)
-
-                k = cv.waitKey(wk)
-                if k == 27:  # Esc key to stop
-                    break
-
-            # cv.destroyAllWindows()
-
-        @staticmethod
-        def integrate_images(framelist):
-            """compute the integration of n frames
-            the last frames weigh heavier
-            :Parameters: list of frames
-            :Returns: image
-            """
-            frames = len(framelist)
-            out = framelist[0]
-            for i in range(1, frames):
-                out = cv.addWeighted(out, (1 - 1 / frames), framelist[i], (1 / frames), -1)
-            return out
-
-        @staticmethod
-        def average_images(framelist):
-            """compute the average of n frames
-            all frames have the same weight
-            :Parameters: list of frames
-            :Returns: image
-            """
-            if (len(framelist))>0:
-                if (framelist[0].dtype==np.uint8):
-                    out = np.average(framelist, axis=0).astype(dtype=np.uint8)
-                else:
-                    out = np.average(framelist, axis=0).astype(dtype=np.uint16)
+    @staticmethod
+    def to_video(image_list, file_out=r'video.avi', framerate=15):
+        """image list (in memory) to video
+
+        :Parameters: image_list
+        :Returns: video
+        """
+
+        os.makedirs(os.path.dirname(file_out), exist_ok=True)
+
+        frame = image_list[0]
+        height, width = frame.shape[0], frame.shape[1]
+
+        video = cv.VideoWriter(file_out, 0, framerate, (width, height))
+
+        for image in image_list:
+            image = ims.Image.Convert.toRGB(image)
+            video.write(image)
+        cv.destroyAllWindows()
+        video.release()
+
+    @staticmethod
+    def play(image_list, framerate=15, verbose=True, window_name="Imagestack"):
+        """view image list (in memory)
+        """
+        wk = int(1000 / framerate)
+        if wk < 1:
+            wk = 1
+        if verbose == True:
+            print("imagestack play: delay per frame in ms {}".format(wk))
+
+        cv.imshow(window_name, image_list[0])
+        cv.moveWindow(window_name, 0, 0)
+
+        for image in image_list:
+            image = ims.Image.Convert.toRGB(image)
+            cv.imshow(window_name, image)
+
+            k = cv.waitKey(wk)
+            if k == 27:  # Esc key to stop
+                break
+
+        cv.destroyWindow(window_name)
+
+    @staticmethod
+    def integrate_images(framelist):
+        """compute the integration of n frames
+        the last frames weigh heavier
+        :Parameters: list of frames
+        :Returns: image
+        """
+        frames = len(framelist)
+        out = framelist[0]
+        for i in range(1, frames):
+            out = cv.addWeighted(out, (1 - 1 / frames), framelist[i], (1 / frames), -1)
+        return out
+
+    @staticmethod
+    def average_images(framelist):
+        """compute the average of n frames
+        all frames have the same weight
+        :Parameters: list of frames
+        :Returns: image
+        """
+        if (len(framelist)) > 0:
+            if (framelist[0].dtype == np.uint8):
+                out = np.average(framelist, axis=0).astype(dtype=np.uint8)
             else:
-                print("Error: Insufficient frames in list.")
-            return out
+                out = np.average(framelist, axis=0).astype(dtype=np.uint16)
+        else:
+            print("Error: Insufficient frames in list.")
+        return out
+
+    @staticmethod
+    def median_images(framelist):
+        """compute the median of n frames
+        the frames with the most frequent features weight more
+        :Parameters: list of frames
+        :Returns: image
+        """
+        out = np.median(framelist, axis=0).astype(dtype=np.uint8)
+        return out
+
+    @staticmethod
+    def reverse(framelist):
+        """reverse frames
+        :Parameters: list of frames
+        :Returns: list of frames
+        """
+        return framelist[::-1]
+
+    @staticmethod
+    def load(path_in):
+        """load image stack
+
+        :Parameters: path
+        :Returns: image_list
+        """
+        filelist = []
+        for filename in sorted(os.listdir(path_in)):
+            if filename.endswith(('.tiff', '.png', '.tif', '.bmp', '.jpg', '.TIFF', '.PNG', '.TIF', '.BMP', '.JPG')):
+                fn = os.path.join(path_in, filename)
+                filelist.append(fn)
+        image_list = []
+        print(filelist)
+        for fn in filelist:
+            img = ims.Image.load(fn)
+
+            image_list.append(img)
+        return image_list
+
+    @staticmethod
+    def save(image_list, path_out):
+        """save image stack
+        :Parameters: image_list, path
+        """
+        i = 0
+        for im3 in image_list:
+            cv.imwrite(path_out + "im{:02d}.png".format(i), im3)
+            i = i + 1
+
+    @staticmethod
+    def transition_dissolve(image0, image1, duration=5 * 15):
+        """
+        transition dissolve within n frames
+
+        :Parameters: image0, image1
+        :Returns: duration in frames
+        """
+        step = 1 / duration
+        alphas = [1 - (step * x) for x in range(0, duration)]
+        s = []
+        gamma = 1
+        for x in range(duration):
+            a = image0
+            b = image1
+            alpha = alphas[x]
+            beta = 1 - alpha
+            dissolved = cv.addWeighted(a, alpha, b, beta, gamma)
+            s.append(dissolved)
+        return s
+
+    @staticmethod
+    def transition_fadeinout(image0, duration=5 * 15, fadein=True):
+        """
+        transition fade or out within n frames
+        :Parameters: image0, image1
+        :Returns: duration in frames, fade in or fade out
+        """
+        mask = np.zeros(image0.shape, dtype='uint8')
+        step = 1 / duration
+        alphas = [x * step for x in range(1, duration + 1)]
+        s = []
+        gamma = 1
 
-        @staticmethod
-        def median_images(framelist):
-            """compute the median of n frames
-            the frames with the most frequent features weight more
-            :Parameters: list of frames
-            :Returns: image
-            """
-            out = np.median(framelist, axis=0).astype(dtype=np.uint8)
-            return out
-
-        @staticmethod
-        def reverse(framelist):
-            """reverse frames
-            :Parameters: list of frames
-            :Returns: list of frames
-            """
-            return framelist[::-1]
-
-
-        @staticmethod
-        def load(path_in):
-            """load image stack
-
-            :Parameters: path
-            :Returns: image_list
-            """
-            filelist = []
-            for filename in sorted(os.listdir(path_in)):
-                if filename.endswith(('.tiff','.png','.tif','.bmp','.jpg')):
-                    fn = os.path.join(path_in, filename)
-                    filelist.append(fn)
-            image_list=[]
-            print(filelist)
-            for fn in filelist:
-                img= ims.Image.load(fn)
-
-                image_list.append(img)
-            return image_list
-
-
-        @staticmethod
-        def save(image_list, path_out):
-            """save image stack
-            :Parameters: image_list, path
-            """
-            i=0
-            for im3 in image_list:
-                cv.imwrite(path_out + "im{:02d}.png".format(i), im3)
-                i=i+1
-
-        @staticmethod
-        def transition_dissolve(image0, image1, duration=5 * 15):
-            """
-            transition dissolve within n frames
-
-            :Parameters: image0, image1
-            :Returns: duration in frames
-            """
-            step = 1 / duration
-            alphas = [1 - (step * x) for x in range(0, duration)]
-            s = []
-            gamma = 1
-            for x in range(duration):
-                a = image0
-                b = image1
+        for x in range(duration):
+            if fadein:
                 alpha = alphas[x]
-                beta = 1 - alpha
-                dissolved = cv.addWeighted(a, alpha, b, beta, gamma)
-                s.append(dissolved)
-            return s
-
-        @staticmethod
-        def transition_fadeinout(image0, duration=5 * 15, fadein=True):
-            """
-            transition fade or out within n frames
-            :Parameters: image0, image1
-            :Returns: duration in frames, fade in or fade out
-            """
-            mask = np.zeros(image0.shape, dtype='uint8')
-            step = 1 / duration
-            alphas = [x * step for x in range(1, duration + 1)]
-            s = []
-            gamma = 1
-
-            for x in range(duration):
-                if fadein:
-                    alpha = alphas[x]
-                    beta = alphas[-x]
-                else:
-                    alpha = alphas[-x]
-                    beta = alphas[x]
-                combined = cv.addWeighted(image0, alpha, mask.copy(), beta, gamma)
-                s.append(combined)
-            return s
-
-        @staticmethod
-        def transition_wipe(image0, image1, duration=5 * 15, reverse=False, horizontal=True, showline=True):
-            """
-            transition wipe, reverse or not, horizontal or vertical
-            :Parameters: image0, image1
-            :Returns: duration in frames, reverse, horizontal
-            """
-            s = []
-
-            if horizontal == True:
-                w = image0.shape[1]
-                step = (w / duration)
+                beta = alphas[-x]
             else:
-                w = image0.shape[0]
-                step = (w / duration)
-
-            x = 0
-
-            frame0 = image0.copy()
-            frame1 = image1.copy()
-            for i in range(0, duration):
-                image0 = frame1.copy()
-                image1 = frame0.copy()
-                if reverse == False:
-                    x = int((i + 1) * step)
-                else:
-                    x = w - int((i + 1) * step)
-                cval = x
-                if (cval < 0):
-                    cval = 0
-                if (cval >= w):
-                    cval = w - 1
-                if horizontal == True:
-                    image0[0:image0.shape[0], cval:image0.shape[1]] = image1[0:image1.shape[0], cval:image1.shape[1]]
-                    if showline == True:
-                        cv.line(image0, (cval, 0), (cval, image0.shape[1]), (255, 255, 255), 1)
-                else:
-                    image0[cval:image0.shape[0], 0:image0.shape[1]] = image1[cval:image1.shape[0],
-                                                                      0:image1.shape[1]]  # note on np crop: y0,y1,x0,x1
-                    if showline == True:
-                        cv.line(image0, (0, cval), (image0.shape[1], cval), (255, 255, 255), 1)
-
-                # cv.line(image0, (cval, 0), (cval, image0.shape[1]), (255, 255, 255), 2)
-                s.append(image0)
-            return s
-
-        @staticmethod
-        def scroll_old(image0, zoomfactor=2,duration=5 * 15, horizontal=True,reverse=False):
-            """
-            Scroll left - DEPRECIATED
-            :Parameters: image0, zoomfactor
-            :Returns: frames
-            """
-            s=[]
-
+                alpha = alphas[-x]
+                beta = alphas[x]
+            combined = cv.addWeighted(image0, alpha, mask.copy(), beta, gamma)
+            s.append(combined)
+        return s
+
+    @staticmethod
+    def transition_wipe(image0, image1, duration=5 * 15, reverse=False, horizontal=True, showline=True):
+        """
+        transition wipe, reverse or not, horizontal or vertical
+        :Parameters: image0, image1
+        :Returns: duration in frames, reverse, horizontal
+        """
+        s = []
+
+        if horizontal == True:
+            w = image0.shape[1]
+            step = (w / duration)
+        else:
+            w = image0.shape[0]
+            step = (w / duration)
+
+        x = 0
+
+        frame0 = image0.copy()
+        frame1 = image1.copy()
+        for i in range(0, duration):
+            image0 = frame1.copy()
+            image1 = frame0.copy()
+            if reverse == False:
+                x = int((i + 1) * step)
+            else:
+                x = w - int((i + 1) * step)
+            cval = x
+            if (cval < 0):
+                cval = 0
+            if (cval >= w):
+                cval = w - 1
             if horizontal == True:
-                w = image0.shape[1]
-                step = (w / duration)
+                image0[0:image0.shape[0], cval:image0.shape[1]] = image1[0:image1.shape[0], cval:image1.shape[1]]
+                if showline == True:
+                    cv.line(image0, (cval, 0), (cval, image0.shape[1]), (255, 255, 255), 1)
             else:
-                h = image0.shape[0]
-                step = (h / duration)
-
-            x=0.5
-            y=0.5
-            frame0 = image0.copy()
-            for i in range(0, duration):
-                image0 = frame0.copy()
-                if horizontal==True:
-                    if reverse == False:
-                        x = (int((i + 1) * step))/frame0.shape[0]
-                    else:
-                        x = (w - int((i + 1) * step))/frame0.shape[0]
-                else:
-                    if reverse == False:
-                        y = (int((i + 1) * step))/frame0.shape[1]
-                    else:
-                        y = (h - int((i + 1) * step))/frame0.shape[1]
-                image1 = ims.Image.zoom(image0,factor=zoomfactor,cx=x,cy=y)
-                s.append(image1)
-                #Image.plot(image1)
-            return s
-
-        @staticmethod
-        def scroll(image0,image1, duration=5 * 15, horizontal=True,reverse=False):
-            """
-            Scroll left/right/top/down
-            :Parameters: image0, zoomfactor
-            :Returns: frames
-            """
-
-            s=[]
+                image0[cval:image0.shape[0], 0:image0.shape[1]] = image1[cval:image1.shape[0],
+                                                                  0:image1.shape[1]]  # note on np crop: y0,y1,x0,x1
+                if showline == True:
+                    cv.line(image0, (0, cval), (image0.shape[1], cval), (255, 255, 255), 1)
+
+            # cv.line(image0, (cval, 0), (cval, image0.shape[1]), (255, 255, 255), 2)
+            s.append(image0)
+        return s
+
+    @staticmethod
+    def scroll_old(image0, zoomfactor=2, duration=5 * 15, horizontal=True, reverse=False):
+        """
+        Scroll left - DEPRECIATED
+        :Parameters: image0, zoomfactor
+        :Returns: frames
+        """
+        s = []
+
+        if horizontal == True:
+            w = image0.shape[1]
+            step = (w / duration)
+        else:
+            h = image0.shape[0]
+            step = (h / duration)
+
+        x = 0.5
+        y = 0.5
+        frame0 = image0.copy()
+        for i in range(0, duration):
+            image0 = frame0.copy()
             if horizontal == True:
-                if reverse==True:
-                    imagen = ims.Image.Tools.patches2image([image1,image0],cols=2,overlappx=0,whitebackground=False)
+                if reverse == False:
+                    x = (int((i + 1) * step)) / frame0.shape[0]
                 else:
-                    imagen = ims.Image.Tools.patches2image([image0,image1],cols=2,overlappx=0,whitebackground=False)
-                w = image0.shape[1]
-                x_speed = (w / duration)
-                y_speed=0
-                h = image0.shape[0]
+                    x = (w - int((i + 1) * step)) / frame0.shape[0]
             else:
-                if reverse==True:
-                    imagen = ims.Image.Tools.patches2image([image1,image0],cols=1,overlappx=0,whitebackground=False)
+                if reverse == False:
+                    y = (int((i + 1) * step)) / frame0.shape[1]
                 else:
-                    imagen = ims.Image.Tools.patches2image([image0,image1],cols=1,overlappx=0,whitebackground=False)
-
-                h = image0.shape[0]
-                y_speed = (h / duration)
-                x_speed=0
-                w = image0.shape[1]
-
-            for i in range(0, duration):
-                x = int(max(0, min(w, 0 + round(x_speed * i))))
-                y = int(max(0, min(h, 0 + round(y_speed * i))))
-                imageout = imagen[y: y + h, x: x + w]
-                s.append(imageout)
-            return s
+                    y = (h - int((i + 1) * step)) / frame0.shape[1]
+            image1 = ims.Image.zoom(image0, factor=zoomfactor, cx=x, cy=y)
+            s.append(image1)
+            # Image.plot(image1)
+        return s
+
+    @staticmethod
+    def scroll(image0, image1, duration=5 * 15, horizontal=True, reverse=False):
+        """
+        Scroll left/right/top/down
+        :Parameters: image0, zoomfactor
+        :Returns: frames
+        """
+
+        s = []
+        if horizontal == True:
+            if reverse == True:
+                imagen = ims.Image.Tools.patches2image([image1, image0], cols=2, overlappx=0, whitebackground=False)
+            else:
+                imagen = ims.Image.Tools.patches2image([image0, image1], cols=2, overlappx=0, whitebackground=False)
+            w = image0.shape[1]
+            x_speed = (w / duration)
+            y_speed = 0
+            h = image0.shape[0]
+        else:
+            if reverse == True:
+                imagen = ims.Image.Tools.patches2image([image1, image0], cols=1, overlappx=0, whitebackground=False)
+            else:
+                imagen = ims.Image.Tools.patches2image([image0, image1], cols=1, overlappx=0, whitebackground=False)
 
+            h = image0.shape[0]
+            y_speed = (h / duration)
+            x_speed = 0
+            w = image0.shape[1]
+
+        for i in range(0, duration):
+            x = int(max(0, min(w, 0 + round(x_speed * i))))
+            y = int(max(0, min(h, 0 + round(y_speed * i))))
+            imageout = imagen[y: y + h, x: x + w]
+            s.append(imageout)
+        return s
+
+
+    @staticmethod
+    def create_dummy_imagestack(image0, slices=10, add_noise=0.2, add_translations=0.2, add_rotations=360):
+        """
+        create dummy slices for an image stack with noise or translations
+        noise sigma 0-1, 0=no noise
+        translations 0-1, 0= no translation, 1 is full image max
+        rotations 0-360, 0 = no rotations
+
+        :Parameters: image, slices, add_noise,add_translations
+        :Returns: frames
+        """
+        w = image0.shape[1]
+        h = image0.shape[0]
+        s=[]
+        for i in range(0, slices):
+            image1 = image0.copy()
+            if add_noise>0:
+                image1=ims.Image.Process.poisson_noise(image1,prob=add_noise)
+            if add_translations>0:
+                shiftx = int(-w*add_translations/2 + random.randint(0, int(w*add_translations)))
+                shifty = int(-h*add_translations/2 + random.randint(0, int(h*add_translations)))
+                image1=ims.Image.Transform.translate(image1,shiftx,shifty)
+            if add_rotations>0:
+                alpha = random.randint(0, add_rotations)
+                image1=ims.Image.Transform.rotate(image1,alpha)
+
+            s.append(image1)
+        return s
+
+
+    @staticmethod
+    def align_images(framelist, update_reference_image=True, high_precision=False):
+        """
+        Correct image shifts for a list of images in memory
+        Images should be of the same size
+
+        update_reference_image True: means the last aligned image acts as a reference. False the first image acts as a reference.
+        high precision uses a nonmaximum suppression algorithm: this is more precise but a lot slower
+
+        :Parameters: image list
+        :Returns: image list, correctiondata list(X,Y,Score)
+        """
+        framelist2 = []
+        correctiondatalist = []
+        frames = len(framelist)
+        frame0 = framelist[0]
+        framelist2.append(frame0)
+        correctiondatalist.append([0, 0, 1])
+        for i in range(1, frames):
+            frame1 = framelist[i]
+            if high_precision == True:
+                frame2, sx, sy, score = ims.Analyze.ImageAlignment.NONMAX(frame0, frame1)
+            else:
+                frame2, sx, sy, score = ims.Analyze.ImageAlignment.NCC(frame0, frame1)
+            framelist2.append(frame2)
+            correctiondatalist.append([sx, sy, score])
+            if update_reference_image == True:
+                frame0 = frame2.copy()
+        return framelist2, correctiondatalist
+
+    @staticmethod
+    def align_images_reapply(framelist, correctiondatalist):
+        """
+        Correct image shifts for a list of images in memory using a correctionlist in memory
+        the correction list can be loaded from disk.
+
+        :Parameters: image list, correctiondata list(X,Y,Score)
+        :Returns: image list
+        """
+
+        framelistnew = []
+        i = 0
+        for im in framelist:
+            x, y, score = correctiondatalist[i]
+            im2 = ims.Image.Transform.translate(im, x, y)
+            framelistnew.append(im2)
+            i = i + 1
+        return framelistnew
```

### Comparing `imsis-1.1/imsis/logging.py` & `IMSIS-1.1.2/imsis/logging.py`

 * *Files identical despite different names*

### Comparing `imsis-1.1/imsis/misc.py` & `IMSIS-1.1.2/imsis/misc.py`

 * *Files 26% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
         :Parameters:  path_in
         :Returns: file list
         """
 
         fn_list = []
         for file in sorted(os.listdir(path_in0)):
-            if file.endswith((".png", ".tif", ".tiff",".jpg",".bmp")):
+            if file.endswith(('.tiff', '.png', '.tif', '.bmp', '.jpg', '.TIFF', '.PNG', '.TIF', '.BMP', '.JPG')):
                 fn_list.append(os.path.join(path_in0, file))
         return fn_list
 
     @staticmethod
     def uniquetimestamp():
         """Create a unique timestamp
 
@@ -125,23 +125,59 @@
         """
         pw = base64.b64decode(input_string).decode("utf-8", "ignore")
         return pw
 
     @staticmethod
     def multicolumnlist2textfile(filename, itemlist):
         """Save string to textfile
+        DEPRECIATED
 
         :Parameters: path, itemlist
         """
 
         os.makedirs(os.path.dirname(filename), exist_ok=True)
 
         with open(filename, "w") as outfile:
             outfile.write("\n".join(str(item).lstrip('[').rstrip(']') for item in itemlist))
 
+    @staticmethod
+    def save_multicolumnlist(filename, itemlist,headerlist):
+        """Save list with array of string to each line
+        add header with properties if enabled
+
+        :Parameters: path, itemlist, header
+        """
+
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+
+        with open(filename, "w") as outfile:
+            if headerlist:
+                outfile.write(','.join(str(item) for item in headerlist)+"\n")
+            outfile.write("\n".join(str(item).lstrip('[').rstrip(']') for item in itemlist))
+
+    @staticmethod
+    def load_multicolumnlist(filename):
+        """load list with array of string to each line
+        header will be ignored (mainly for reading in notepad/excel etc.)
+
+        :Parameters: filename
+        :Returns: list
+        """
+
+        data = []
+        with open(filename) as f:
+            first_row = True
+            for line in f:
+                if first_row:
+                    first_row = False
+                    continue
+                columns = line.strip().split(",")
+                data.append([float(val) for val in columns])
+        return data
+
 
 
     @staticmethod
     def obj2dict(obj, verbose=False):
         """Convert Object to Dictionary
 
         can be used for json serialization of objects in a class
```

### Comparing `imsis-1.1/imsis/view.py` & `IMSIS-1.1.2/imsis/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,20 @@
 
         try:
             dummy = (img.shape)
         except:
             print('Error, image shape mismatch found in plot.')
 
         plt.figure(figsize=(8, 8))
-        plt.gcf().canvas.set_window_title(window_title)
+        try:
+            plt.gcf().canvas.set_window_title(window_title)
+        except:
+            plt.gcf().canvas.setWindowTitle(window_title)
+            print("ERROR: Matplotlib versioning errors..")
+
         plt.title(title)
 
         img = ims.Image.Convert.BGRtoRGB(img)
 
         if len(img.shape) == 2:
             plt.imshow(img, cmap='gray')
         else:
@@ -72,15 +77,20 @@
                 titlelist.append("")
 
         ln = len(imglist)
         rows = int(np.math.sqrt(ln))
         cols = int(ln / rows + 0.5)
 
         plt.figure(figsize=(cols * 4, rows * 4))
-        plt.gcf().canvas.set_window_title(window_title)
+
+        try:
+            plt.gcf().canvas.set_window_title(window_title)
+        except:
+            plt.gcf().canvas.setWindowTitle(window_title)
+            print("ERROR: Matplotlib versioning errors..")
 
         # print(rows,cols)
         i = 0
         j = 0
         m = 0
 
         for img in imglist:
```

### Comparing `imsis-1.1/README.md` & `IMSIS-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `imsis-1.1/setup.py` & `IMSIS-1.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from distutils.core import setup
 import setuptools
 
 setup(
   name = 'imsis',
   packages = ['imsis'],
-  version = '1.1',
+  version = '1.1.2',
   license='MIT',
   description = 'image analysis in Python',
   author = 'rengezri',
   author_email = 'rengezri@gmail.com',
   url = 'https://github.com/rengezri',
-  download_url = 'https://github.com/rengezri/imsis/archive/refs/tags/v1.0.0.tar.gz',
+  download_url = 'https://github.com/rengezri/imsis/archive/refs/tags/v1.1.2.tar.gz',
   keywords = ['image analysis', 'dialogs', 'batch processing'],   # Keywords that define your package best
   install_requires=['markdown'],
   classifiers=[
     'Topic :: Scientific/Engineering :: Image Processing',
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
   ],
 )
```

