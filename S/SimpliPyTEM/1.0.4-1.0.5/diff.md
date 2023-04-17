# Comparing `tmp/SimpliPyTEM-1.0.4.tar.gz` & `tmp/SimpliPyTEM-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpliPyTEM-1.0.4.tar", last modified: Thu Mar 23 11:34:49 2023, max compression
+gzip compressed data, was "SimpliPyTEM-1.0.5.tar", last modified: Mon Apr 17 09:37:50 2023, max compression
```

## Comparing `SimpliPyTEM-1.0.4.tar` & `SimpliPyTEM-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-03-23 11:34:49.755297 SimpliPyTEM-1.0.4/
--rw-r--r--   0 gabriel    (501) staff       (20)    35149 2023-01-20 17:02:41.000000 SimpliPyTEM-1.0.4/LICENSE
--rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-03-23 11:34:49.754979 SimpliPyTEM-1.0.4/PKG-INFO
--rw-r--r--   0 gabriel    (501) staff       (20)     1746 2023-01-17 17:53:42.000000 SimpliPyTEM-1.0.4/README.md
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-03-23 11:34:49.744719 SimpliPyTEM-1.0.4/SimpliPyTEM/
--rw-r--r--   0 gabriel    (501) staff       (20)    10035 2023-03-23 11:32:30.000000 SimpliPyTEM-1.0.4/SimpliPyTEM/App_functions.py
--rw-r--r--   0 gabriel    (501) staff       (20)    83687 2023-03-23 11:32:30.000000 SimpliPyTEM-1.0.4/SimpliPyTEM/MicroVideo_class.py
--rw-r--r--   0 gabriel    (501) staff       (20)    71140 2023-03-23 11:32:30.000000 SimpliPyTEM-1.0.4/SimpliPyTEM/Micrograph_class.py
--rw-r--r--   0 gabriel    (501) staff       (20)     3320 2023-03-20 17:44:55.000000 SimpliPyTEM-1.0.4/SimpliPyTEM/Motion_correction.py
--rw-r--r--   0 gabriel    (501) staff       (20)     7487 2023-01-13 10:50:18.000000 SimpliPyTEM-1.0.4/SimpliPyTEM/PDF_generator.py
--rw-r--r--   0 gabriel    (501) staff       (20)    18705 2023-03-23 11:32:30.000000 SimpliPyTEM-1.0.4/SimpliPyTEM/Particle_analysis.py
--rw-r--r--   0 gabriel    (501) staff       (20)     4875 2023-03-23 11:32:30.000000 SimpliPyTEM-1.0.4/SimpliPyTEM/Particle_tracking.py
--rwxr-xr-x   0 gabriel    (501) staff       (20)    22167 2023-03-23 11:32:30.000000 SimpliPyTEM-1.0.4/SimpliPyTEM/SimpliPyTEM_GUI.py
--rw-r--r--   0 gabriel    (501) staff       (20)     7182 2023-03-20 17:44:55.000000 SimpliPyTEM-1.0.4/SimpliPyTEM/html_writer.py
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-03-23 11:34:49.754571 SimpliPyTEM-1.0.4/SimpliPyTEM.egg-info/
--rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-03-23 11:34:49.000000 SimpliPyTEM-1.0.4/SimpliPyTEM.egg-info/PKG-INFO
--rw-r--r--   0 gabriel    (501) staff       (20)      517 2023-03-23 11:34:49.000000 SimpliPyTEM-1.0.4/SimpliPyTEM.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel    (501) staff       (20)        1 2023-03-23 11:34:49.000000 SimpliPyTEM-1.0.4/SimpliPyTEM.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       69 2023-03-23 11:34:49.000000 SimpliPyTEM-1.0.4/SimpliPyTEM.egg-info/entry_points.txt
--rw-r--r--   0 gabriel    (501) staff       (20)      166 2023-03-23 11:34:49.000000 SimpliPyTEM-1.0.4/SimpliPyTEM.egg-info/requires.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       12 2023-03-23 11:34:49.000000 SimpliPyTEM-1.0.4/SimpliPyTEM.egg-info/top_level.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       38 2023-03-23 11:34:49.755389 SimpliPyTEM-1.0.4/setup.cfg
--rw-r--r--   0 gabriel    (501) staff       (20)     2106 2023-03-20 17:44:55.000000 SimpliPyTEM-1.0.4/setup.py
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-04-17 09:37:50.541139 SimpliPyTEM-1.0.5/
+-rw-r--r--   0 gabriel    (501) staff       (20)    35149 2023-01-20 17:02:41.000000 SimpliPyTEM-1.0.5/LICENSE
+-rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-04-17 09:37:50.540743 SimpliPyTEM-1.0.5/PKG-INFO
+-rw-r--r--   0 gabriel    (501) staff       (20)     2373 2023-04-03 10:12:55.000000 SimpliPyTEM-1.0.5/README.md
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-04-17 09:37:50.525413 SimpliPyTEM-1.0.5/SimpliPyTEM/
+-rw-r--r--   0 gabriel    (501) staff       (20)    10120 2023-04-04 10:53:05.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/App_functions.py
+-rw-r--r--   0 gabriel    (501) staff       (20)    85128 2023-04-03 08:57:45.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/MicroVideo_class.py
+-rw-r--r--   0 gabriel    (501) staff       (20)    71639 2023-04-03 08:57:45.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/Micrograph_class.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     3320 2023-03-20 17:44:55.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/Motion_correction.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     7567 2023-04-17 09:25:52.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/PDF_generator.py
+-rw-r--r--   0 gabriel    (501) staff       (20)    18705 2023-03-23 11:32:30.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/Particle_analysis.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     4875 2023-03-23 11:32:30.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/Particle_tracking.py
+-rwxr-xr-x   0 gabriel    (501) staff       (20)    22560 2023-04-17 09:11:44.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/SimpliPyTEM_GUI.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     7182 2023-03-20 17:44:55.000000 SimpliPyTEM-1.0.5/SimpliPyTEM/html_writer.py
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-04-17 09:37:50.540197 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/
+-rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel    (501) staff       (20)      517 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)        1 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       69 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/entry_points.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)      166 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/requires.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       12 2023-04-17 09:37:50.000000 SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/top_level.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       38 2023-04-17 09:37:50.541262 SimpliPyTEM-1.0.5/setup.cfg
+-rw-r--r--   0 gabriel    (501) staff       (20)     2106 2023-04-17 09:34:20.000000 SimpliPyTEM-1.0.5/setup.py
```

### Comparing `SimpliPyTEM-1.0.4/LICENSE` & `SimpliPyTEM-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.4/PKG-INFO` & `SimpliPyTEM-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpliPyTEM
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python package to simplify the processing and analysis of TEM and in situ TEM images and videos
 Home-page: https://github/gabriel-ing/Micrograph-analysis-scripts
 Author: Gabriel Ing
 Author-email: ucbtgrb@ucl.ac.uk
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `SimpliPyTEM-1.0.4/README.md` & `SimpliPyTEM-1.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # SimpliPyTEM: an open source project to simplify python-based analysis of electron microscopy data with added focus on in situ videos 
 
 <img src=docs/Media/Images/SimpliPyTEM_figures.001.png width=700px, alt='Figure showing effect of SimpliPyTEM-GUI'>
 
-Please see full documentation at https://micrograph-analysis-scripts.readthedocs.io/en/latest/ 
+Please see full documentation at https://simplipytem.readthedocs.io/en/latest/
 
 SimpliPyTEM introduces the Micrograph and MicroVideo classes to process images and videos respectively. These aim to make many basic functions incredibly simple, without the need for knowledge of more complex libraries which are performing the functions. Functions included are adding scalebar, enhancing contrast and equalising histogram, converting to 8bit images, binning, filtering with many common filters (Median, gaussian, low-pass, weiner and non-local means). Video frames can easily be averaged together in both simple averaging and running averging ways. 
 
 The image data within these classes are kept in numpy arrays, which is the most common format for using images in other applications, which makes it easy to use the files for downstream processes like thresholding and particle analysis. 
 
 On top of the simplified python functions, I have also implemented an app to automate the image analysis - this allows all the files in a directory to be processed (eg. filtered, contrast enhanced, add scalebar, save as jpg) to make looking at, presenting and downloaded images much faster and the filesizes much smaller. This is also combined with outputting the images onto a pdf document or an html file which then allows for viewing images and videos as a webpage. This type of automation is designed to make viewing the results of an experiment a rapid and straightforward process 
 
+If there are any features that you would like to be added - for example compatibility with other filetypes, or if things aren't working as you expect them to, please feel free to open an issue and I will do my best to sort it for you! Please also be aware that I am a final year PhD student with my own research so I will help when I can find the time...
+
+I would also like to welcome any additions from potential contributors, whether it is practical examples of code being used, bugs being fixedd or the introduction of new functionalities. Again, feel free to raise an issue or contact me directly if you would like help with these things .
```

### Comparing `SimpliPyTEM-1.0.4/SimpliPyTEM/App_functions.py` & `SimpliPyTEM-1.0.5/SimpliPyTEM/App_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,20 +154,20 @@
             if running_time>max_running_time:
                 break
             time.sleep(30)      
 
     os.chdir(cwd)
 
 '''
-def video_processing(filename, output_folder_name,xybin, medfilter, gaussian_filter, video_status, topaz_denoise, denoise_with_cuda):
+def video_processing(filename, output_folder_name,xybin, medfilter, gaussian_filter,scalebar_on, video_status, topaz_denoise, denoise_with_cuda):
     if video_status=='Save Average':
 
-        default_image_pipeline(filename, xybin = xybin, medfilter=medfilter, gaussfilter=gaussian_filter,outdir=output_folder_name, topaz_denoise=topaz_on, denoise_with_cuda=cuda_on)
+        default_image_pipeline(filename, xybin = xybin, medfilter=medfilter, gaussfilter=gaussian_filter,scalebar=scalebar_on, outdir=output_folder_name, topaz_denoise=topaz_denoise, denoise_with_cuda=denoise_with_cuda)
     else:
-        default_video_pipeline(filename,output_type=video_status, xybin = xybin, medfilter=medfilter, gaussfilter=gaussian_filter,outdir=output_folder_name, topaz_denoise=topaz_on, denoise_with_cuda=cuda_on) #output folder = output_folder+videos
+        default_video_pipeline(filename,output_type=video_status, xybin = xybin, medfilter=medfilter, gaussfilter=gaussian_filter,outdir=output_folder_name, scalebar=scalebar_on,topaz_denoise=topaz_denoise, denoise_with_cuda=denoise_with_cuda) #output folder = output_folder+videos
      
 
 
 
 def isvideo(dmfile):
     try:
         f = nci.dm.fileDM(dmfile)
```

### Comparing `SimpliPyTEM-1.0.4/SimpliPyTEM/MicroVideo_class.py` & `SimpliPyTEM-1.0.5/SimpliPyTEM/MicroVideo_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -350,18 +350,24 @@
 
         if name:
             if name[-4:]!='.tif':
                 name+='.tif'        
         else:
             name = '.'.join(self.filename.split('.')[:-1])+'.tif'    
         
+        if pixel_unit!='nm':
+            pu = 'um'
+        else:
+            pu='nm'
+
+
         if outdir:
             make_outdir(outdir)
             name = outdir+'/'+name
-        tifffile.imsave(name, self.frames,imagej=True, resolution=(1/self.pixel_size, 1/self.pixel_size), metadata={'unit':self.pixel_unit})
+        tifffile.imsave(name, self.frames,imagej=True, resolution=(1/self.pixel_size, 1/self.pixel_size), metadata={'unit':pu})
 
 
     def save_tif_sequence(self, name=None, outdir=None):
         '''        
         Saves each frame of the video as a tif, this is saved in the current format, so if an 8bit tif is required, run video.convert_to_8bit() before use.
         nameand outdir can be included to give a name (prefix) and  the output directory. 
         
@@ -376,30 +382,34 @@
         Outputs
         -------
 
             Saves a sequence of Tif files into the output directory listed (cwd is default)
 
         '''
         if name:
-            name = kwargs['name']
             if name[-4:]=='.tif':
                 name= name.strip('.tif')
         else: 
             name = '.'.join(self.filename.split('.')[:1]) 
 
         if outdir:
             make_outdir(outdir)
             name = outdir+'/'+name
 
+        if self.pixel_unit!='nm':
+            pu = 'um'
+        else:
+            pu='nm'
+
         for i in range(len(self.frames)):
             j=4-len(str(i))
             zeros = '0000'
             count = str(zeros[:j])+str(i)
             savename = name+'_{}'.format(count)+'.tif'
-            tifffile.imsave(savename, self.frames[i],imagej=True, resolution=(1/self.pixel_size, 1/self.pixel_size), metadata={'unit':self.pixel_unit, 'Labels':'{}/{} -{}'.format(i, len(self.frames),self.filename)})
+            tifffile.imsave(savename, self.frames[i],imagej=True, resolution=(1/self.pixel_size, 1/self.pixel_size), metadata={'unit':pu, 'Labels':'{}/{} -{}'.format(i, len(self.frames),self.filename)})
 
     def save_gif(self, fps=5,**kwargs ):
 
         if 'name' in kwargs:
             name = kwargs['name']
             if name[-4:]!='.gif':
                 name= name+'.gif'
@@ -498,33 +508,35 @@
                 If not saving the average (average=False), this chooses which frame to save - index starts at zero and negative numbers count from the end
 
         '''
 
 
         if outdir:
             make_outdir(outdir)
-            name =outdir+name    
+            name =outdir+'/'+name    
         print('Start name :', name)
         if name:
                 print('if name : ',name)
-                if name[-3:]=='jpg':
+                if name[-4:]=='.jpg':
                     ftype='jpg'
-                elif name[-3:]=='tif':
-                    ftype='tif'    
+                    name=name[:-4]
+                elif name[-4:]=='.tif':
+                    ftype='tif' 
+                    name = name[:-4]   
                 if len(name.split('.'))>2:
                     name='.'.join(name.split('.')[:-1])
                     print('if len name: ', name)
                     print('.'.join(name.split('.')[:-1]))
         else:
                 name = '.'.join(self.filename.split('.')[:-1])
                 print('else_name = ',name)
-        try:
-            name += '_'+self.scalebar_size+'scale.{}'.format(ftype)
-        except AttributeError:
-            name+='.'+ftype
+        #try:
+        #    name += '_'+self.scalebar_size+'scale.{}'.format(ftype)
+        #except AttributeError:
+        name+='.'+ftype
         #if self.foldername!='':
         #        name = '/'+self.foldername.strip('/n') + '/' + name.split('/')[-1]
         #if self.foldername=='':
         #    newname = self.filename.split('.dm')[0]+'_'+self.text+'scale.jpg'
         #else:
         #    newname = self.foldername.strip('\n') + '/' +self.filename.split('.dm')[0]+'_'+self.text+'scale.jpg'
         if average:
@@ -1082,143 +1094,171 @@
             unit : str
                 Unit of measurement
 
         '''
         self.pixel_size=dist/pixels
         self.pixel_unit=unit
 
-
     def choose_scalebar_size(self):
         '''
         Function for choosing scalebar size, called through make_scalebar(), not a standalone function.
+
+        Returns
+        -------
+            scalebar_x: int
+                x coordinate for the scalebar 
+            scalebar_y: int
+                y coordinate for the scalebar 
+            width:int
+                width of scalebar
+            height:int
+                height of the scalebar
+            scalebar_size:int (or float)
+                Size of the scalebar in scaled units (pixel_unit)
         '''
-       
+        y,x = self.frames.shape[1], self.frames.shape[2]
         
         #make coordinates for the scalebar, currently set to y-12.5%,x-5% of image size from the bottom right corner 
         #of the image to bottom left of the scalebar - change this by editing /20 and /7.5 values (this just looked good to me)
-        scalebar_y = self.y-int(self.y/25)
-        scalebar_x = self.x-int(self.x/6.5)
+        scalebar_y = y-int(y/25)
+        scalebar_x = x-int(x/6.5)
         #print(x,scalebar_x)
-        #possible scalebar sizes are given here, if its >500nm it should be in unit micron, hopefully this should only fail with very extreme examples
+
+        #possible scalebar sizes are given here, if its >500nm it should be in unit micron
         
-        possible_sizes = [0.5, 1,2,5,10,25,50,100,250,500]
+        possible_sizes = [0.5, 1,2,5,10,25,50,100,250,500,1000]
         
         #to select sizes, iterate through possible sizes, if the width of the resulting scalebar (n*pixelsize) 
         #is over 15% of the image size, the size is chose, if none are over 15% of image size
         #the largest size is chosen as default
-        
         for n in possible_sizes:
-            width = n*1/self.pixel_size
+            width = int(n*1/self.pixel_size)
             #print(n, image.shape([0]/10)
-            if width>(self.x/15):
+            if width>(x/16):
                 break
-                #print(width, x/15)
+        
+        # This if statement checks whether the scalebar is too close to the edge or bigger than the size. 
+        # This should ensure it is at least one 100th of the image width away from the edge.
+
+        if scalebar_x+width>=x:
+            print(True)
+            diff = x - scalebar_x+width
+            scalebar_x=scalebar_x-diff - x/100
+        elif scalebar_x+width+x/100 > x:
+            scalebar_x=scalebar_x-x/100
+
         #choose height of scalebar (default is scalebar width/6), convert width into an integer
-        height = int(self.y/60)
+        height = int(y/60)
         width = int(width)   
-        self.scalebar_x = int(scalebar_x)
-        self.scalebar_y = int(scalebar_y)
-        self.height = int(height)
-        self.width = int(width)
-        self.n = n
-    #return int(scalebar_x/xybin), int(scalebar_y/xybin), int(height/xybin), int(width/xybin), n
+        scalebar_x = int(scalebar_x)
+        scalebar_y = int(scalebar_y)
+        scalebar_size = n
+        #return int(scalebar_x/xybin), int(scalebar_y/xybin), int(height/xybin), int(width/xybin), n
+        return scalebar_x, scalebar_y, width, height, scalebar_size
+
 
 
 
-    def choose_scalebar_color(self,color):
+    def choose_scalebar_color(self,color,scalebar_x, scalebar_y , width, height):
         '''
         Function for choosing the scalebar color and returns the pixelvalue and text color for the annotation.
         Called through make_scalebar(), not a standalone function
         '''
         if color=='black':
-            self.pixvalue = 0
-            self.textcolor = 'black'
+            pixvalue = 0
+            textcolor = 'black'
         elif color=='white':
-            self.pixvalue = 255
-            self.textcolor='white'
+            pixvalue = 255
+            textcolor='white'
         elif color=='grey':
-            self.pixvalue = 150
-            self.textcolor='grey'
+            pixvalue = 150
+            textcolor='grey'
         else: #default is black, unless it is a particularly dark area - if the mean pixvalue of the scale bar region is significantly less than the overall image mean, the scalebar will be white
             
-            if np.mean(self.frames[0][self.scalebar_y:self.scalebar_y+self.height,self.scalebar_x:self.scalebar_x+self.width])<np.mean(self.frames[0])/1.5:
-                self.pixvalue = 255
-                self.textcolor='white'
+            if np.mean(self.frames[0][scalebar_y:scalebar_y+height,scalebar_x:scalebar_x+width])<np.mean(self.frames[0])/1.5:
+                pixvalue = 255
+                textcolor='white'
             else:
-                self.pixvalue = 0
-                self.textcolor = 'black'
+                pixvalue = 0
+                textcolor = 'black'
         #add scalebar (set pixels to color) 
 
-        #return pixvalue, textcolor        
+        return pixvalue, textcolor        
 
 
     def make_scalebar(self, texton=True, color='Auto', fontsize='M'):
         '''
         Automated method to create a scalebar of a suitable size, shape and color. Returns a new object with a scalebar. 
         The color will be selected between black and white based on mean value of the region of the scalebar compared to the mean value of the whole video. To override this the color can be defined as black white or grey.
         This will work best for 8-bit images, as the scalebar will be given values of 0 or 255. 
+
+        You can change the fontsize of the scalebar label with the fontsize option, this is medium ('M') by default but can be made larger or smaller ('S','L', 'XL'), if none of these look good to you, you can choose the fontsize by entering an integer instead of these options. For reference, the fontsize given by these values (calculated based on image size) is printed.
         
         Parameters
         ----------
 
             color : str
                 The color of the scalebar, the options are 'white'. 'black' or 'grey'
             texton : bool
                 Text can be turned off using texton=False, the selected size of the scalebar can be accessed using micrograph.scalebar_size
             fontsize: str
-                Choose the fontsize from S,M,L,XL 
+                Choose the fontsize from S,M,L,XL or give an integer value 
         Returns
         -------
             Micrograph_object_with_scalebar: Micrograph
                 Copy of the micrograph object with a scale bar.
         '''
         #print(pixvalue, textcolor)
         vidSB = deepcopy(self)
-        vidSB.choose_scalebar_size()
-        vidSB.choose_scalebar_color(color)
+        scalebar_x, scalebar_y , width, height, scalebar_size = self.choose_scalebar_size()
+        pixvalue, textcolor = self.choose_scalebar_color(color,scalebar_x, scalebar_y , width, height)
+        textposition = ((scalebar_x+width/2),scalebar_y-5)
+
+        if fontsize=='M':
+            fontsize=int(scalebar_x/(22))
+        elif fontsize=='L':
+            fontsize=int(scalebar_x/(18))
+        elif fontsize=='XL':
+            fontsize=int(scalebar_x/(15))
+        elif fontsize=='S':
+            fontsize=int(scalebar_x/(27))
+
+
         for i in range(len(self.frames)):
             #print(self.frames[i])
-            vidSB.frames[i][vidSB.scalebar_y:vidSB.scalebar_y+vidSB.height,vidSB.scalebar_x:vidSB.scalebar_x+vidSB.width]=vidSB.pixvalue
+            vidSB.frames[i][scalebar_y:scalebar_y+height,scalebar_x:scalebar_x+width]=pixvalue
+            
             
-            textposition = ((vidSB.scalebar_x+vidSB.width/2),vidSB.scalebar_y-5)
             
             #if pixel_unit!='nm':
              #   Utext = str(n)+u'\u00b5'+ 'm'
               #  text = str(n)+'microns'
             #else:
-            vidSB.text = '{}{}'.format(vidSB.n,vidSB.pixel_unit) 
+            vidSB.scalebar_size = '{}{}'.format(scalebar_size,vidSB.pixel_unit) 
              
 
             pil_image = Image.fromarray(vidSB.frames[i])
 
             if texton==True:
                 #print('TEXTON!')
-                if fontsize=='M':
-                    fontsize=int(vidSB.scalebar_x/(25))
-                elif fontsize=='L':
-                    fontsize=int(vidSB.scalebar_x/(20))
-                elif fontsize=='XL':
-                    fontsize=int(vidSB.scalebar_x/(17))
-                elif fontsize=='S':
-                    fontsize=int(vidSB.scalebar_x/(30))
-
                 draw = ImageDraw.Draw(pil_image)        
                     
                 #fontsize=int(vidSB.scalebar_x/(25))
                 try:
-                    file = font_manager.findfont('Helvetica Neue')
+                    file = font_manager.findfont('Helvetica')
                     font = ImageFont.truetype(file, fontsize)
                 except:
                     font_search = font_manager.FontProperties(family='sans-serif', weight='normal')
                     file = font_manager.findfont(font_search)
                     font = ImageFont.truetype(file, fontsize)
 
-                draw.text(textposition, vidSB.text, anchor ='mb', fill=vidSB.textcolor, font=font, stroke_width=1)
+                draw.text(textposition, vidSB.scalebar_size, anchor ='mb', fill=textcolor, font=font, stroke_width=1)
                 vidSB.frames[i] = np.array(pil_image)    
-        
+            else:
+                print('The scalebar added is {}'.format(vidSB.scalebar_size))
         print('Fontsize:',fontsize)
         vidSB.log.append('make_scalebar()')
         return vidSB
 
 
     '''------------------------------------------------------------------------------------------------------------------------
         SECTION: IMAGE FILTERS
@@ -1269,16 +1309,17 @@
             fft = np.fft.fft2(filtered_object.frames[i])
             fshift = np.fft.fftshift(fft)
             magnitude_spectrum = np.log(np.abs(fshift))
             crow, ccol = int(self.y/2), int(self.x/2)
             fshift_filtered=np.copy(fshift)
             mask = np.zeros_like(self.frames[i])
 
-            mask = cv.circle(mask, (crow, ccol),radius*2, 1, -1) 
+            mask = cv.circle(cv.UMat(mask), (crow, ccol),radius*2, 1, -1) 
             #print(fshift_filtered)
+            mask = mask.get()
             fcomplex = fshift[:,:]*1j
             fshift_filtered = mask*fcomplex
             f_filtered_shifted = np.fft.fftshift(fshift_filtered)
             #magnitude_spectrum_filter = np.log(np.abs(f_filtered_shifted))
             inv_image = np.fft.ifft2(f_filtered_shifted)
             filtered_object.frames[i] = np.abs(inv_image)
             filtered_object.frames[i] -= filtered_object.frames[i].min()
```

### Comparing `SimpliPyTEM-1.0.4/SimpliPyTEM/Micrograph_class.py` & `SimpliPyTEM-1.0.5/SimpliPyTEM/Micrograph_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         print(mrc.voxel_size)
         voxel_size = mrc.voxel_size
         self.pixel_size = float(str(voxel_size).split(',')[0].strip('('))
         self.image = mrc.data
         self.image.setflags(write=1)
         self.x = self.image.shape[1]
         self.y = self.image.shape[0]
-        self.image = np.flip(self.image, axis=0)
+        #self.image = np.flip(self.image, axis=0)
         self.pixel_unit='nm'
         self.filename = file
         if pixel_correction:
             self.image[self.image>self.image.mean()+self.image.std()*20]=self.image.mean()
         # this line converts the image to a float32 datatype, this will make it run slower if it starts out as a 8 or 16 bit, I maybe should account for this, but its also required for median filter and others, so I'm performing as default. 
         self.image = self.image.astype('float32')
         self.shape=self.image.shape
@@ -387,50 +387,57 @@
         ''' 
         if outdir:
             make_outdir(outdir)
             name = outdir+'/'+name
         #print('Start name :', name)
         if name:
                 #print('if name : ',name)
-                if name[-3:]=='jpg':
+                if name[-4:]=='.jpg':
                     ftype='jpg'
-                elif name[-3:]=='tif':
+                    name = name[:-4]
+                elif name[-4:]=='.tif':
                     ftype='tif'    
+                    name = name[:-4]
+
                 if len(name.split('.'))>=2 and name[-4]=='.':
                     name='.'.join(name.split('.')[:-1])
                     #print('if len name: ', name)
                     #print('.'.join(name.split('.')[:-1]))
         else:
                 name = '.'.join(self.filename.split('.')[:-1])
+                name+='.'+ftype
                 #print('else_name = ',name)
         #try:
         #    name += '_'+self.scalebar_size.replace('µ','u')+'scale.{}'.format(ftype)
         #except AttributeError:
-        name+='.'+ftype
+        
         #if self.foldername!='':
         #        name = '/'+self.foldername.strip('/n') + '/' + name.split('/')[-1]
         #if self.foldername=='':
         #    newname = self.filename.split('.dm')[0]+'_'+self.text+'scale.jpg'
         #else:
         #    newname = self.foldername.strip('\n') + '/' +self.filename.split('.dm')[0]+'_'+self.text+'scale.jpg'
         
+        name+='.'+ftype
         if self.pixel_unit=='µm':
             pixel_unit='um'
         else:
             pixel_unit=self.pixel_unit
 
         if ftype=='jpg':
             if self.image.max()!=255 or self.image.min()!=0:
                 print(self.image.max(), self.image.min())
                 self = self.convert_to_8bit()
                 print('converting to 8bit')
             cv.imwrite(name,self.image)
 
         elif ftype=='tif':
-            tifffile.imsave(name, self.image,imagej=True, resolution=(1/self.pixel_size, 1/self.pixel_size), metadata={'unit':pixel_unit})
+            metadata= self.metadata_tags
+            metadata['unit':pixel_unit]
+            tifffile.imsave(name, self.image,imagej=True, resolution=(1/self.pixel_size, 1/self.pixel_size), metadata=metadata)
 
         #self.pil_image.save(name, quality=self.quality)
         print(name, 'Done!')
 
         #    def average_video(self):
         #       self.image = np.average(image, axis=0)
     
@@ -798,35 +805,43 @@
         y,x = self.image.shape
         
         #make coordinates for the scalebar, currently set to y-12.5%,x-5% of image size from the bottom right corner 
         #of the image to bottom left of the scalebar - change this by editing /20 and /7.5 values (this just looked good to me)
         scalebar_y = y-int(y/25)
         scalebar_x = x-int(x/6.5)
         #print(x,scalebar_x)
-        #possible scalebar sizes are given here, if its >500nm it should be in unit micron, hopefully this should only fail with very extreme examples
+
+        #possible scalebar sizes are given here, if its >500nm it should be in unit micron
         
         possible_sizes = [0.5, 1,2,5,10,25,50,100,250,500,1000]
         
         #to select sizes, iterate through possible sizes, if the width of the resulting scalebar (n*pixelsize) 
         #is over 15% of the image size, the size is chose, if none are over 15% of image size
         #the largest size is chosen as default
-        
         for n in possible_sizes:
-            width = n*1/self.pixel_size
+            width = int(n*1/self.pixel_size)
             #print(n, image.shape([0]/10)
             if width>(x/15):
                 break
-                #print(width, x/15)
+        
+        # This if statement checks whether the scalebar is too close to the edge or bigger than the size. 
+        # This should ensure it is at least one 100th of the image width away from the edge.
+
+        if scalebar_x+width>=x:
+            print(True)
+            diff = x - scalebar_x+width
+            scalebar_x=scalebar_x-diff - x/100
+        elif scalebar_x+width+x/100 > x:
+            scalebar_x=scalebar_x-x/100
+
         #choose height of scalebar (default is scalebar width/6), convert width into an integer
         height = int(y/60)
         width = int(width)   
         scalebar_x = int(scalebar_x)
         scalebar_y = int(scalebar_y)
-        height = int(height)
-        width = int(width)
         scalebar_size = n
         #return int(scalebar_x/xybin), int(scalebar_y/xybin), int(height/xybin), int(width/xybin), n
         return scalebar_x, scalebar_y, width, height, scalebar_size
 
 
     def choose_scalebar_color(self,color, scalebar_x, scalebar_y, width, height):
         '''
@@ -920,15 +935,15 @@
             elif fontsize=='S':
                 fontsize=int(scalebar_x/(30))
             print(fontsize)
             draw = ImageDraw.Draw(pil_image)        
             
             #fontsize=int(scalebar_x/(25))
             try:
-                file = font_manager.findfont('Helvetica Neue')
+                file = font_manager.findfont('Helvetica')
                 font = ImageFont.truetype(file, fontsize)
             except:
                 font_search = font_manager.FontProperties(family='sans-serif', weight='normal')
                 file = font_manager.findfont(font_search)
                 font = ImageFont.truetype(file, fontsize)
             draw.text(textposition, micrograph_SB.scalebar_size, anchor ='mb', fill=textcolor, font=font, stroke_width=1)
             micrograph_SB.image = np.array(pil_image)    
@@ -985,16 +1000,17 @@
         fshift = np.fft.fftshift(fft)
         magnitude_spectrum = np.log(np.abs(fshift))
         rows, cols = self.image.shape
         crow, ccol = int(rows/2), int(cols/2)
         fshift_filtered=np.copy(fshift)
         mask = np.zeros_like(self.image)
 
-        mask = cv.circle(mask, (crow, ccol),radius*2, 1, -1) 
+        mask = cv.circle(cv.UMat(mask), (crow, ccol),radius*2, 1, -1) 
         #print(fshift_filtered)
+        mask = mask.get()
         fcomplex = fshift[:,:]*1j
         fshift_filtered = mask*fcomplex
         f_filtered_shifted = np.fft.fftshift(fshift_filtered)
         #magnitude_spectrum_filter = np.log(np.abs(f_filtered_shifted))
         inv_image = np.fft.ifft2(f_filtered_shifted)
         filtered_image = np.abs(inv_image)
         filtered_image -= filtered_image.min()
```

### Comparing `SimpliPyTEM-1.0.4/SimpliPyTEM/Motion_correction.py` & `SimpliPyTEM-1.0.5/SimpliPyTEM/Motion_correction.py`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.4/SimpliPyTEM/PDF_generator.py` & `SimpliPyTEM-1.0.5/SimpliPyTEM/PDF_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,28 +143,30 @@
             The ID number of the image 
 
         prefix:str
             The prefix to the image id - normally contains details about the sample. 
 
     
     '''
-    lstring = string.split('_')
-
+    nstring= string.replace('.', '_')
+    lstring = nstring.split('_')
+    #print(lstring)
     success = False
     for item in lstring:
-        if len(item)==4 and item.isdigit:
+        if len(item)==4 and item.isdigit():
                 im_id = item
                 ind = lstring.index(im_id)
                 #print(ind)
                 success=True
     if success==False:
         ind = -2
         im_id = lstring[ind]
 
     prefix = ' '.join(lstring[:ind])
+    #print(success)
     return im_id, prefix
 #print(im_prefix)
 
 def group_images(images):
     '''
     Sorts a number of images into a dictionary with images separated by the sample name, these can then be separated onto different pages.
```

### Comparing `SimpliPyTEM-1.0.4/SimpliPyTEM/Particle_analysis.py` & `SimpliPyTEM-1.0.5/SimpliPyTEM/Particle_analysis.py`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.4/SimpliPyTEM/Particle_tracking.py` & `SimpliPyTEM-1.0.5/SimpliPyTEM/Particle_tracking.py`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.4/SimpliPyTEM/SimpliPyTEM_GUI.py` & `SimpliPyTEM-1.0.5/SimpliPyTEM/SimpliPyTEM_GUI.py`

 * *Files 3% similar despite different names*

```diff
@@ -337,14 +337,16 @@
             print('Please select a folder/file')
             return 1
 
         cwd = os.getcwd()
         os.chdir(self.folderpath+'/'+outdir)
 
         title = self.title_box.text()
+        if title=='':
+            title = 'Default_title'
         notes = self.notes_box.toPlainText()
         print('Writing html and css files')
         try: 
             image_files, video_files = get_files('Images', 'Videos')
         except FileNotFoundError: 
             print('The Images folder was not found, please make sure that the output folder defined above has a folder of images called images.')
             os.chdir(cwd)
@@ -372,15 +374,15 @@
 
         title = self.title_box.text()
         notes = self.notes_box.toPlainText()
         
         print(os.getcwd())
         print(os.listdir('.'))
         try: 
-            images = ['Images/'+x for x in os.listdir('Images')]
+            images = ['Images/'+x for x in os.listdir('Images') if 'jpg' in x]
         except FileNotFoundError: 
             print('The Images folder was not found, please make sure that the output folder defined above has a folder of images called images.')
             os.chdir(cwd)
             return 1
         print(images)
         try:
             pdf_generator(images, title, notes)
@@ -415,30 +417,30 @@
             print('Please select a folder/file')
             return 1
         print(self.folderpath)
         
         try: 
             if self.folder_option=='Folder':
                     print('Running folder?')
-                    thread = threading.Thread(target =self.process_folder, args=(self.folderpath, outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.video_status, self.topaz_on, self.cuda_on ))
+                    thread = threading.Thread(target =self.process_folder, args=(self.folderpath, outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.scalebar_on, self.video_status, self.topaz_on, self.cuda_on ))
                     thread.start()
             elif self.folder_option=='File':
                     print(self.live)    
-                    self.process_file(self.folderpath, outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.video_status,self.topaz_on, self.cuda_on  )
+                    self.process_file(self.folderpath, outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.scalebar_on,self.video_status,self.topaz_on, self.cuda_on  )
             elif self.folder_option =='Live Processing':
                     #live_process_folder(self.folderpath, outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.video_status )
                     print('Live processing')
-                    thread = threading.Thread(target=self.live_process, args=(self.folderpath,outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.video_status,self.topaz_on, self.cuda_on  ))
+                    thread = threading.Thread(target=self.live_process, args=(self.folderpath,outdir, self.bin_value, self.med_filter_value, self.gauss_filter_value,self.scalebar_on,self.video_status,self.topaz_on, self.cuda_on  ))
                     thread.start()
         except Exception as e:
 
             print('Whoops there is an error, check the terminal and your inputs and try again.')
             print(e)
 
-    def process_folder(self,folder, output_folder_name,xybin, medfilter, gaussian_filter, video_status, topaz_on, cuda_on):
+    def process_folder(self,folder, output_folder_name,xybin, medfilter, gaussian_filter,scalebar_on, video_status, topaz_on, cuda_on):
         start_time = time.time()
         print('Processing folder!')
         cwd = os.getcwd()
 
         os.chdir(folder)
 
 #        dm_files = [x for x in os.listdir('.') if x[-4:-1]=='.dm']
@@ -460,30 +462,30 @@
             os.mkdir(output_folder_name)
 
         for file in vid_files:
             print(self.stopSignal)
             if self.eval_stop():
                 return 1 
             print('Processing: ', file)
-            video_processing(file,output_folder_name,xybin, medfilter, gaussian_filter, video_status, topaz_on, cuda_on )
+            video_processing(filename=file,output_folder_name=output_folder_name,xybin=xybin, medfilter=medfilter, gaussian_filter=gaussian_filter,scalebar_on=scalebar_on, video_status=video_status, topaz_denoise=topaz_on, denoise_with_cuda=cuda_on )
 
         for  file in im_files:
             if self.eval_stop():
                 return 1 
-            default_image_pipeline(file, xybin = xybin, medfilter=medfilter, gaussfilter=gaussian_filter,outdir=output_folder_name, topaz_denoise=topaz_on, denoise_with_cuda=cuda_on)
+            default_image_pipeline(file, xybin = xybin, medfilter=medfilter, gaussfilter=gaussian_filter,scalebar=scalebar_on,outdir=output_folder_name, topaz_denoise=topaz_on, denoise_with_cuda=cuda_on)
         if len(dm_frames)!=0: 
             print(dm_frames)
             frames_processing(dm_frames,output_folder_name,xybin, medfilter, gaussian_filter, video_status )
         print('All files in folder complete!')  
         running_time = time.time()-start_time
         print('Running time for {} images and {} videos: {}'.format(len(im_files),len(vid_files), running_time))
         os.chdir(cwd)
 
 
-    def live_process(self, folder, output_folder_name,xybin, medfilter, gaussian_filter, video_status, topaz_on, cuda_on):
+    def live_process(self, folder, output_folder_name,xybin, medfilter, gaussian_filter, scalebar_on,video_status, topaz_on, cuda_on):
         cwd = os.getcwd()
         #print('calling function')
         os.chdir(folder)
         files = os.listdir('.')
         file_set = set(files)
         start_time = time.time()
         max_running_time = 3600
@@ -512,15 +514,15 @@
                         time.sleep(1)      
                         if os.path.getsize(file)>currentsize:
                             break
 
 
 
                         if isvideo(file) and video_status!='Save Average':
-                            video_processing(file,output_folder_name,xybin, medfilter, gaussian_filter, video_status,topaz_denoise=topaz_on, denoise_with_cuda=cuda_on)
+                            video_processing(file,output_folder_name,xybin, medfilter, gaussian_filter, scalebar_on=scalebar_on,video_status=video_status,topaz_denoise=topaz_on, denoise_with_cuda=cuda_on)
                         else:
                             default_image_pipeline(file, xybin = xybin, medfilter=medfilter, gaussfilter=gaussian_filter,outdir=output_folder_name,topaz_denoise=topaz_on, denoise_with_cuda=cuda_on)
                     
                         
 
                     file_set.add(file)
                 
@@ -530,19 +532,19 @@
             if running_time>max_running_time:
                 break
             time.sleep(10)
             #print('Looping')      
         print('Time out reached, exiting now')
         os.chdir(cwd)
 
-    def process_file(self,folderpath, outdir, bin_value, med_filter_value, gauss_filter_value,video_status ):
+    def process_file(self,folderpath, outdir, bin_value, med_filter_value, gauss_filter_value,scalebar_on, video_status ):
         if isvideo(file):
-            video_processing(folderpath, outdir, xybin =bin_value, medfilter=med_filter_value, gaussian_filter=gauss_filter_value, video_status= video_status)
+            video_processing(folderpath, outdir, xybin =bin_value, medfilter=med_filter_value, gaussian_filter=gauss_filter_value, scalebar_on=scalebar_on,video_status= video_status)
         else:
-            default_image_pipeline(filename, xybin = xybin, medfilter=med_filter_value, gaussfilter=gauss_filter_value,outdir=outdir)
+            default_image_pipeline(filename, xybin = xybin, medfilter=med_filter_value, gaussfilter=gauss_filter_value,scalebar=scalebar_on,outdir=outdir)
 
 '''
 class JobRunner(QRunnable):
 
     signals = WorkerSignals()
 
     def __init__(self):
```

### Comparing `SimpliPyTEM-1.0.4/SimpliPyTEM/html_writer.py` & `SimpliPyTEM-1.0.5/SimpliPyTEM/html_writer.py`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.4/SimpliPyTEM.egg-info/PKG-INFO` & `SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpliPyTEM
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python package to simplify the processing and analysis of TEM and in situ TEM images and videos
 Home-page: https://github/gabriel-ing/Micrograph-analysis-scripts
 Author: Gabriel Ing
 Author-email: ucbtgrb@ucl.ac.uk
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `SimpliPyTEM-1.0.4/SimpliPyTEM.egg-info/SOURCES.txt` & `SimpliPyTEM-1.0.5/SimpliPyTEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.4/setup.py` & `SimpliPyTEM-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup 
 
 setup(
 	name='SimpliPyTEM',
-	version='1.0.4',
+	version='1.0.5',
 	description='A python package to simplify the processing and analysis of TEM and in situ TEM images and videos',
 	long_description='''SimpliPyTEM is a python package to make python-based analysis of Transmission electron microscopy images easier and more approachable. Although TEM is the focus, this could also easily be adapted to other microscopy images. Importantly, SimpliPyTEM is designed to make automated, basic work accessible for beginners (through a simple GUI), while more complicated methods can be accessed through simple python code. This package centers around the image data being held in a Numpy array which makes the image data easy to access for further analysis.
 	This project aims to make use of the rapid automation of image analysis methods available through python while making it approachable for the user.
 	Functions to generate pdf and html files containing images and videos are also included in this package. This allows easy viewing and sharing of all the images/videos taken in an imaging session, making experiment evaluation significantly easier. 
 	For more info, please see: https://micrograph-analysis-scripts.readthedocs.io/en/latest/''',
 	url='https://github/gabriel-ing/Micrograph-analysis-scripts',
 	author='Gabriel Ing',
```

