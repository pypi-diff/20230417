# Comparing `tmp/cellmap-1.0.1.dev202304161147-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304170945-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1388287 bytes, number of entries: 6
+Zip file size: 1388592 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    53292 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304161147.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304161147.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304161147.dist-info/RECORD
-6 files, 4502656 bytes uncompressed, 1387401 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    54856 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304170945.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304170945.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304170945.dist-info/RECORD
+6 files, 4504220 bytes uncompressed, 1387706 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304161147.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304170945.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304161147.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304170945.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304161147.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304170945.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -190,26 +190,28 @@
     return cmap
 
 def edge_velocity(
         X,
         vel,
         source,
         target,
+        normalization = True,
 ):
     idx_vel = np.isnan(vel[0])==False
     X1,X2 = X[:,idx_vel][source],X[:,idx_vel][target]
     V1,V2 = vel[:,idx_vel][source],vel[:,idx_vel][target]
     Dis = np.linalg.norm(X2-X1,axis=1)
     Dis[Dis==0] = 1
     V1_p,V2_p = V1*(X2-X1),V2*(X2-X1)
     V1_p[V1_p<0] = 0
     V2_p[V2_p<0] = 0
     edge_vel = np.sum(0.5*(V1_p+V2_p),axis=1)/Dis/np.sum(idx_vel)
-    edge_vel_norm = np.linalg.norm(edge_vel)
-    if edge_vel_norm > 0: edge_vel= edge_vel/edge_vel_norm
+    if normalization:
+        edge_vel_norm = np.linalg.norm(edge_vel)
+        if edge_vel_norm > 0: edge_vel= edge_vel/edge_vel_norm
     return edge_vel
 
 def solve_vorticity_streamline(
     div_mat,
     edge_vel,
     vorticity_key = 'vorticity',
     stream_key = 'stream_line',
@@ -327,15 +329,16 @@
         tri_,idx_tri = create_graph(exp_LD[:,0],exp_LD[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
         source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
         for i in range(adata.shape[0]):
             idx_s = source == i
             idx_t = target == i
             ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
             ex_t = -(exp_LD[target[idx_t]]-exp_LD[source[idx_t]])/np.linalg.norm(exp_LD[target[idx_t]]-exp_LD[source[idx_t]],ord=2)
-            vel_potential[i] = 2*(np.sum((adata.obs[potential_key][source[idx_s]].values-adata.obs[potential_key][target[idx_s]].values)*ex_s.T,axis=1) + \
+            edge_vel = edge_velocity(exp_LD,vel_LD,source,target,normalization=False)
+            vel_potential[i] = 2*np.linalg.norm(edge_vel)*(np.sum((adata.obs[potential_key][source[idx_s]].values-adata.obs[potential_key][target[idx_s]].values)*ex_s.T,axis=1) + \
                                 np.sum((adata.obs[potential_key][target[idx_t]].values-adata.obs[potential_key][source[idx_t]].values)*ex_t.T,axis=1))
             # vel_rotation[i] = 2*(np.sum((adata.obs[rotation_key][source[idx_s]].values-adata.obs[rotation_key][target[idx_s]].values)*ex_s.T,axis=1) + \
             #                     np.sum((adata.obs[rotation_key][target[idx_t]].values-adata.obs[rotation_key][source[idx_t]].values)*ex_t.T,axis=1))
         adata.obsm[pot_vkey_] = vel_potential
         adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
         # adata.obsm[rot_vkey_] = vel_rotation
     elif graph_method == 'knn':
@@ -1071,44 +1074,72 @@
         print('There is no cluster key \"%s\" in adata.obs' % cluster_key)
 
 
 def write(
     adata,
     filename = 'CellMap',
     basis = 'umap',
+    vkey  = 'velocity',
+    exp_key = None,
     potential_key = 'potential',
+    rotation_key = 'rotation',
+    vorticity_key = 'vorticity',
+    streamline_key = 'stream_line',
     cluster_key = 'clusters',
     obs_key = None,
     genes = None,
-    expression_key = None,
     use_HVG = True,
     n_HVG = 10,
 ):
-    kwargs = check_arguments(adata,basis=basis,potential_key=potential_key,cluster_key=cluster_key,obs_key=obs_key,genes=genes,expression_key=expression_key)
+    kwargs = check_arguments(adata,basis=basis,potential_key=potential_key,cluster_key=cluster_key,obs_key=obs_key,genes=genes,expression_key=exp_key)
     basis,obs_key,genes = kwargs['basis'],kwargs['obs_key'],kwargs['genes']
     basis_key = 'X_%s' % basis
+    vkey_ = '%s_%s' % (vkey,basis)
+    pot_key_ = '%s' % (potential_key)
+    rot_key_ = '%s' % (rotation_key)
+    pot_vkey_ = '%s_%s_%s' % (potential_key,vkey,basis)
+    rot_vkey_ = '%s_%s_%s' % (rotation_key,vkey,basis)
+    vol_key_ = '%s_%s_%s' % (potential_key,vorticity_key,basis)
+    sl_key_ = '%s_%s_%s' % (potential_key,streamline_key,basis)
+    pot_vol_key_ = '%s_%s_%s' % (potential_key,vorticity_key,basis)
+    pot_sl_key_ = '%s_%s_%s' % (potential_key,streamline_key,basis)
+    rot_vol_key_ = '%s_%s_%s' % (rotation_key,vorticity_key,basis)
+    rot_sl_key_ = '%s_%s_%s' % (rotation_key,streamline_key,basis)
     
-    if expression_key == None:
+    
+    if exp_key == None:
         if scipy.sparse.issparse(adata.X): data_exp = adata.X.toarray()
         else: data_exp = adata.X
     else:
-        data_exp = adata.layers[expression_key]
+        data_exp = adata.layers[exp_key]
     
     pd_out = pd.DataFrame({
         'X':adata.obsm[basis_key][:,0],'Y':adata.obsm[basis_key][:,1],
-        'Potential':adata.obs[potential_key],
-        'Annotation':adata.obs[cluster_key]
+        'Potential':adata.obs[pot_key_],
+        'Annotation':adata.obs[cluster_key],
+        'Rotation':adata.obs[rot_key_],
+        'Streamline_Original':adata.obs[sl_key_],
+        'Streamline_Potential':adata.obs[pot_sl_key_],
+        'Streamline_Rotation':adata.obs[rot_sl_key_],
+        'Vorticity_Original':adata.obs[vol_key_],
+        'Vorticity_Potential':adata.obs[pot_vol_key_],
+        'Vorticity_Rotation':adata.obs[rot_vol_key_],
+        'Velocity_x':adata.obsm[vkey_][:,0],
+        'Velocity_y':adata.obsm[vkey_][:,1],
+        'Velocity_Potential_x':adata.obsm[pot_vkey_][:,0],
+        'Velocity_Potential_y':adata.obsm[pot_vkey_][:,1],
+        'Velocity_Rotation_x':adata.obsm[rot_vkey_][:,0],
+        'Velocity_Rotation_y':adata.obsm[rot_vkey_][:,1],
     },index=adata.obs.index)
     pd_out.index.name='CellID'
     
     if obs_key != None:
         for arg in obs_key:
             pd_out.insert(len(pd_out.columns), arg, adata.obs[arg])
     
-    
     if genes != None:
         for gene in genes:
             pd_out.insert(len(pd_out.columns), gene, data_exp[:,adata.var.index == gene])
     
     if use_HVG:
         scanpy.pp.highly_variable_genes(adata)
         min_mean = np.percentile(np.mean(adata.X.toarray(),axis=0)[np.mean(adata.X.toarray(),axis=0)>0],90)
```

## Comparing `cellmap-1.0.1.dev202304161147.dist-info/METADATA` & `cellmap-1.0.1.dev202304170945.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304161147
+Version: 1.0.1.dev202304170945
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

