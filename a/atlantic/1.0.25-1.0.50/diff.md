# Comparing `tmp/atlantic-1.0.25-py3-none-any.whl.zip` & `tmp/atlantic-1.0.50-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19015 bytes, number of entries: 12
+Zip file size: 18679 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      389 b- defN 23-Feb-20 00:15 atlantic/__init__.py
--rw-rw-rw-  2.0 fat     5510 b- defN 23-Feb-19 22:03 atlantic/atl_feat_eng.py
--rw-rw-rw-  2.0 fat     8705 b- defN 23-Feb-19 23:19 atlantic/atl_feat_selection.py
--rw-rw-rw-  2.0 fat     2351 b- defN 23-Feb-19 21:23 atlantic/atl_metrics.py
--rw-rw-rw-  2.0 fat     2889 b- defN 23-Feb-21 18:44 atlantic/atl_performance.py
--rw-rw-rw-  2.0 fat     8538 b- defN 23-Feb-19 23:06 atlantic/atl_pipeline.py
--rw-rw-rw-  2.0 fat    20380 b- defN 23-Feb-19 23:21 atlantic/atl_processing.py
--rw-rw-rw-  2.0 fat     1078 b- defN 23-Mar-12 15:57 atlantic-1.0.25.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    13159 b- defN 23-Mar-12 15:57 atlantic-1.0.25.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-12 15:57 atlantic-1.0.25.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Mar-12 15:57 atlantic-1.0.25.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      969 b- defN 23-Mar-12 15:57 atlantic-1.0.25.dist-info/RECORD
-12 files, 64069 bytes uncompressed, 17395 bytes compressed:  72.8%
+-rw-rw-rw-  2.0 fat     5510 b- defN 23-Apr-17 10:17 atlantic/atl_feat_eng.py
+-rw-rw-rw-  2.0 fat     8704 b- defN 23-Apr-17 10:49 atlantic/atl_feat_selection.py
+-rw-rw-rw-  2.0 fat     1563 b- defN 23-Apr-17 09:56 atlantic/atl_metrics.py
+-rw-rw-rw-  2.0 fat     2858 b- defN 23-Apr-17 10:11 atlantic/atl_performance.py
+-rw-rw-rw-  2.0 fat     8541 b- defN 23-Apr-17 10:17 atlantic/atl_pipeline.py
+-rw-rw-rw-  2.0 fat    20614 b- defN 23-Apr-17 11:27 atlantic/atl_processing.py
+-rw-rw-rw-  2.0 fat     1078 b- defN 23-Apr-17 13:24 atlantic-1.0.50.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    12367 b- defN 23-Apr-17 13:24 atlantic-1.0.50.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 13:24 atlantic-1.0.50.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-17 13:24 atlantic-1.0.50.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      969 b- defN 23-Apr-17 13:24 atlantic-1.0.50.dist-info/RECORD
+12 files, 62694 bytes uncompressed, 17059 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: atlantic/atl_pipeline.py
 Comment: 
 
 Filename: atlantic/atl_processing.py
 Comment: 
 
-Filename: atlantic-1.0.25.dist-info/LICENSE
+Filename: atlantic-1.0.50.dist-info/LICENSE
 Comment: 
 
-Filename: atlantic-1.0.25.dist-info/METADATA
+Filename: atlantic-1.0.50.dist-info/METADATA
 Comment: 
 
-Filename: atlantic-1.0.25.dist-info/WHEEL
+Filename: atlantic-1.0.50.dist-info/WHEEL
 Comment: 
 
-Filename: atlantic-1.0.25.dist-info/top_level.txt
+Filename: atlantic-1.0.50.dist-info/top_level.txt
 Comment: 
 
-Filename: atlantic-1.0.25.dist-info/RECORD
+Filename: atlantic-1.0.50.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atlantic/atl_feat_eng.py

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
-def split_dataset(Dataset:pd.DataFrame, Split_Racio:float):
+def split_dataset(dataset:pd.DataFrame, split_ratio:float):
     
-    assert Split_Racio>=0.5 and Split_Racio<=0.95 , 'Split_Racio value should be in [0.5,0.95[ interval'
+    assert split_ratio>=0.5 and split_ratio<=0.95 , 'split_ratio value should be in [0.5,0.95[ interval'
     
-    train, test= train_test_split(Dataset, train_size=Split_Racio)
+    train, test= train_test_split(dataset, train_size=split_ratio)
 
     return train,test
 
-def target_type(Dataset:pd.DataFrame, target:str):  
+def target_type(dataset:pd.DataFrame, target:str):  
     
-    df=Dataset[[target]]
+    df=dataset[[target]]
     reg_target,class_target=df.select_dtypes(include=['int','float']).columns.tolist(),df.select_dtypes(include=['object','category']).columns.tolist()
     if len(class_target)==1:
         pred_type='Class'
         eval_metric='Accuracy'
         
     elif len(reg_target)==1:
         pred_type='Reg'
@@ -34,40 +34,40 @@
     X_train = train.iloc[:, 0:(len(sel_cols)-1)].values
     X_test = test.iloc[:, 0:(len(sel_cols)-1)].values
     y_train = train.iloc[:, (len(sel_cols)-1)].values
     y_test = test.iloc[:, (len(sel_cols)-1)].values
     
     return X_train,X_test,y_train,y_test
 
-def slice_timestamp(Dataset:pd.DataFrame):
+def slice_timestamp(dataset:pd.DataFrame):
     
-    df=Dataset.copy()
+    df=dataset.copy()
     datetime_cols=list_date=list(df.select_dtypes(include=['datetime','datetime64[ns]']))
     for date_col in datetime_cols:
             df[date_col] = df[date_col].astype(str)
             df[date_col] = df[date_col].str.slice(0,19)
             df[date_col] = pd.to_datetime(df[date_col])
             
     return df
 
-def engin_date(Dataset:pd.DataFrame, drop:bool=True):
+def engin_date(dataset:pd.DataFrame, drop:bool=True):
     
     """
     The engin_date function takes a DataFrame and returns a DataFrame with the date features engineered.
     The function has two parameters: 
-    Dataset: A Pandas DataFrame containing at least one column of datetime data. 
+    dataset: A Pandas DataFrame containing at least one column of datetime data. 
     drop: A Boolean value indicating whether or not to drop the original datetime columns from the returned dataset.
     
-    :param Dataset:pd.DataFrame: Pass the dataset
+    :param dataset:pd.DataFrame: Pass the dataset
     :param drop:bool=False: Decide whether or not to drop the original datetime columns from the returned dataset
     :return: A dataframe with the date features engineered
     """
 
-    Dataset_=Dataset.copy()
-    Df=Dataset_.copy()
+    dataset_=dataset.copy()
+    Df=dataset_.copy()
     Df=slice_timestamp(Df)
     
     x=pd.DataFrame(Df.dtypes)
     x['column'] = x.index
     x=x.reset_index().drop(['index'], axis=1).rename(columns={0: 'dtype'})
     a=x.loc[x['dtype'] == 'datetime64[ns]']
 
@@ -106,44 +106,44 @@
             Df=Df.drop(elemento,axis=1)
     elif drop==False:
         for elemento in list_date_columns:
             Df=create_date_features(Df,elemento)
         
     return Df
 
-def num_cols(Dataset:pd.DataFrame, target:str):
+def num_cols(dataset:pd.DataFrame, target:str):
     
-    n_cols=Dataset.select_dtypes(include=['int','float']).columns.tolist()
+    n_cols=dataset.select_dtypes(include=['int','float']).columns.tolist()
     
     for col in n_cols:
         if col==target:
             n_cols.remove(target)
             
     return n_cols
 
-def cat_cols(Dataset:pd.DataFrame, target):
+def cat_cols(dataset:pd.DataFrame, target):
 
-    c_cols=Dataset.select_dtypes(include=['object']).columns.tolist()
+    c_cols=dataset.select_dtypes(include=['object']).columns.tolist()
 
     for col in c_cols:
         if col==target:
             c_cols.remove(target)
             
     return c_cols 
 
-def del_nulls_target(Dataset:pd.DataFrame, target:str):
+def del_nulls_target(dataset:pd.DataFrame, target:str):
         
-    Dataset=Dataset[Dataset[target].isnull()==False]
+    dataset=dataset[dataset[target].isnull()==False]
     
-    return Dataset
+    return dataset
 
-def remove_columns_by_nulls(Dataset:pd.DataFrame, percentage:int): ## Colunas 
+def remove_columns_by_nulls(dataset:pd.DataFrame, percentage:int): ## Colunas 
     
     assert percentage>0 and percentage<=100 , 'percentage should not exceed value of 100'
-    df=Dataset.copy()
+    df=dataset.copy()
     perc = percentage
     min_count =  int(((100-perc)/100)*df.shape[0] + 1)
     df = df.dropna( axis=1,
                 thresh=min_count)
     df = df.loc[:, (df==0).mean()*100 < perc]
     df = df.loc[:, ~(df.apply(pd.Series.value_counts, normalize=True).max() > perc/100)]
```

## atlantic/atl_feat_selection.py

```diff
@@ -8,23 +8,21 @@
 import h2o
 from h2o.automl import H2OAutoML
 from statsmodels.stats.outliers_influence import variance_inflation_factor
 from .atl_feat_eng import target_type, remove_columns_by_nulls
 from .atl_performance import pred_eval
 from .atl_processing import fit_Label_Encoding, transform_Label_Encoding
 
-#h2o.init()
-
 ###################################  H2O Feature Selection ######################################
 
-def feature_selection_h2o(Dataset:pd.DataFrame, target:str, total_vi :float=0.98, h2o_fs_models:int =7, encoding_fs:bool=True):
+def feature_selection_h2o(dataset:pd.DataFrame, target:str, total_vi :float=0.98, h2o_fs_models:int =7, encoding_fs:bool=True):
     """
     Function to select features using h2o's Autodml feature.
     Parameters:
-    Dataset: pandas DataFrame, shape = (n_samples,n_features)
+    dataset: pandas DataFrame, shape = (n_samples,n_features)
             Dataframe 
     target: str
             target variable
     total_vi : float
             total relative importance percentage of the selected columns, default is 0.98
     h2o_fs_models: int
             h2o Autodml feature models,default is 7
@@ -35,15 +33,17 @@
             list of selected features
     selected_importance: pandas DataFrame, shape = (n_features, 2)
             Dataframe with the relative importance and variables
     """
     assert total_vi>=0.5 and total_vi<=1 , 'total_vi value should be in [0.5,1] interval'
     assert h2o_fs_models>=1 and h2o_fs_models<=50 , 'h2o_fs_models value should be in [0,50] interval'
     
-    train_=Dataset.copy()
+    h2o.init()
+    
+    train_=dataset.copy()
     train=train_.copy()
     
     if encoding_fs==True:
         le_fit=fit_Label_Encoding(train_,target)   
         train_=transform_Label_Encoding(train_,le_fit)
         train=train_.copy()
         
@@ -115,45 +115,45 @@
     # Calculating VIF
     vif = pd.DataFrame()
     vif['variables'] = X.columns
     vif['VIF'] = [variance_inflation_factor(X.values, i) for i in range(X.shape[1])]
     vif = vif.sort_values(['VIF'], ascending=False)
     return vif
 
-def feature_selection_vif(Dataset:pd.DataFrame, target:str, VIF:float=10.0):
+def feature_selection_vif(dataset:pd.DataFrame, target:str, VIF:float=10.0):
     """
     Function to select features based on VIF 
     Parameters:
-    Dataset: pandas DataFrame, shape = (n_samples,n_features)
+    dataset: pandas DataFrame, shape = (n_samples,n_features)
             Dataframe 
     target: str
             target variable
     VIF: float
             vif threshold ratio, default is 10.0
     Returns:
     sel_cols: list
             list of selected features
     vif_df : pandas DataFrame, shape = (n_features, 2)
             Dataframe with the vif and variables
     """   
     assert VIF>=3 and VIF<=30 , 'VIF value should be in [3,30] interval'
     
-    input_cols= list(Dataset.columns)
+    input_cols= list(dataset.columns)
     input_cols.remove(target)
-    Dataset_=Dataset[input_cols]
-    vif_df=calc_vif(Dataset_)
+    dataset_=dataset[input_cols]
+    vif_df=calc_vif(dataset_)
     sel_cols=input_cols
     for line in range(0,len(vif_df['VIF'])):
         if vif_df['VIF'].loc[vif_df['VIF'].idxmax()]>=VIF:
             vif_df.drop(vif_df['variables'].loc[vif_df['VIF']==vif_df['VIF'].max()].index, inplace=True)
             sel_cols=[]
             for rows in vif_df['variables']:
                 sel_cols.append(rows)
-        Dataset_=Dataset_[sel_cols]
-        vif_df=calc_vif(Dataset_)
+        dataset_=dataset_[sel_cols]
+        vif_df=calc_vif(dataset_)
     sel_cols.append(target)
 
     return sel_cols,vif_df
 
 def vif_performance_selection(train:pd.DataFrame, 
                               test:pd.DataFrame, 
                               target:str, 
@@ -192,27 +192,28 @@
     perf_default = pred_eval(_train_, _test_,target)
     default_p=perf_default[eval_metric][0]
     
     _train__,_test__=train_.copy(),test_.copy()
 
     try:
         cols_vif,vif_df=feature_selection_vif(_train__,target,vif_ratio)
+        print('    ')
         print('Number of Selected VIF Columns: ', len(cols_vif), 
-              '\n Removed Columns with VIF (Feature Selection - VIF):', len(sel_cols) - len(cols_vif), 
-              '\n Selected Columns:', cols_vif)
+              '\nRemoved Columns with VIF :', len(sel_cols) - len(cols_vif)
+              ,'\n All Selected Columns:', cols_vif)
         _train__=_train__[cols_vif]
         _test__=_test__[cols_vif]
     except Exception:
         print('traceback.format_exc: ', traceback.format_exc())
         
     pred_vif = pred_eval(_train__, _test__,target)
     p_default_vif=pred_vif[eval_metric][0]
     print('   ')
     print('Default Performance:',round(default_p, 4))
-    print('Performance Default VIF:',round(p_default_vif, 4))
+    print('VIF Performance:',round(p_default_vif, 4))
     if pred_type=='Reg':
         if p_default_vif<default_p:
             print('The VIF filtering method was applied    ')
             _train_=_train_[cols_vif]
             _test_=_test_[cols_vif]
         else:
             print('The VIF filtering method was not applied    ')
```

## atlantic/atl_metrics.py

```diff
@@ -36,26 +36,7 @@
     
     metrics_class= {'Accuracy': accuracy_metric,
                     'Precision Micro': precision_metric,
                     'F1 Score Macro':f1_macro_metric,
                     }
     
     return metrics_class
-
-def metrics_binary_classification(y_true, y_pred):
-    
-    f1_metric=f1_score(y_true, y_pred)
-    accuracy_metric = accuracy_score(y_true, y_pred)
-    precision_metric = precision_score(y_true, y_pred)
-    recall_metric = recall_score(y_true, y_pred)
-    average_precision_metric = average_precision(y_true, y_pred)
-    balanced_accuracy_metric = balanced_accuracy(y_true, y_pred)
-    
-    metrics_class= {'Accuracy': accuracy_metric, 
-                    'Precision Score': precision_metric,
-                    'F1 Score': f1_metric,
-                    'Recall Score': recall_metric,
-                    'Average Precision': average_precision_metric, 
-                    'Balanced Accuracy': balanced_accuracy_metric
-                    }
-
-    return metrics_class
```

## atlantic/atl_performance.py

```diff
@@ -4,15 +4,15 @@
 from sklearn.preprocessing import OneHotEncoder, LabelEncoder, StandardScaler, MinMaxScaler, RobustScaler
 from sklearn.experimental import enable_iterative_imputer
 from sklearn.ensemble import RandomForestRegressor, ExtraTreesRegressor, RandomForestClassifier, ExtraTreesClassifier
 from sklearn.impute import KNNImputer, SimpleImputer, IterativeImputer
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import *
 from .atl_feat_eng import target_type, divide_dfs
-from .atl_metrics import metrics_regression, metrics_classification, metrics_binary_classification
+from .atl_metrics import metrics_regression, metrics_classification
 
 def pred_eval(train:pd.DataFrame, test:pd.DataFrame, target:str):
     
     X_train,X_test,y_train,y_test=divide_dfs(train,test,target)  
     
     list_estimators,rf,et=[100],[],[]
     pred_type, eval_metric=target_type(train, target)
```

## atlantic/atl_pipeline.py

```diff
@@ -4,15 +4,15 @@
 from h2o.automl import H2OAutoML
 from .atl_feat_eng import *
 from .atl_feat_selection import *
 from .atl_metrics import *
 from .atl_performance import * 
 from .atl_processing import *
 
-h2o.init()
+##h2o.init()
 
 """
 import cane
 from sklearn.preprocessing import OneHotEncoder, LabelEncoder, StandardScaler, MinMaxScaler, RobustScaler
 from sklearn.experimental import enable_iterative_imputer
 from sklearn.ensemble import RandomForestRegressor, ExtraTreesRegressor, RandomForestClassifier, ExtraTreesClassifier
 from sklearn.impute import KNNImputer, SimpleImputer, IterativeImputer
@@ -21,36 +21,36 @@
 from statsmodels.stats.outliers_influence import variance_inflation_factor
 """
 
 #############################################################################################################################################
 ###########################################################    Atlantic Pipeline   ##########################################################
 #############################################################################################################################################
 
-def fit_processing(Dataset:pd.DataFrame,
+def fit_processing(dataset:pd.DataFrame,
                    target:str, 
-                   Split_Racio:float,
+                   split_ratio:float,
                    total_vi:float=0.98,
                    h2o_fs_models:int =7,
                    encoding_fs:bool=True,
                    vif_ratio:float=10.0):
     
-    pred_type, eval_metric=target_type(Dataset, target) ## Prediction Contextualization
-    if pred_type=='Class': Dataset[target]=Dataset[target].astype(str)
+    pred_type, eval_metric=target_type(dataset, target) ## Prediction Contextualization
+    if pred_type=='Class': dataset[target]=dataset[target].astype(str)
     
-    Dataframe_=Dataset.copy()
-    Dataset_=Dataframe_.copy()
+    Dataframe_=dataset.copy()
+    dataset_=Dataframe_.copy()
 
-############################## Validation Procidment ##############################
-    Dataset_=remove_columns_by_nulls(Dataset_, 99.99)
-    sel_cols= list(Dataset_.columns)
+############################## Validation Proceedment ##############################
+    dataset_=remove_columns_by_nulls(dataset_, 99.99)
+    sel_cols= list(dataset_.columns)
     sel_cols.remove(target)
     sel_cols.append(target) 
-    Dataset_=Dataset_[sel_cols] ## target -> Last Column Index
+    dataset_=dataset_[sel_cols] ## target -> Last Column Index
 
-    train, test= split_dataset(Dataset_,Split_Racio)
+    train, test= split_dataset(dataset_,split_ratio)
 
     train_test_=train.copy(),test.copy()
 
     train=del_nulls_target(train,target) ## Delete target Null Values
     test=del_nulls_target(test,target) ## Delete target Null Values
     
 ############################## Feature Engineering Date Column ##############################
@@ -96,15 +96,15 @@
 
 ############################## Fit Procediment ##############################
 
     Dataframe=Dataframe_.copy()
     Dataframe=del_nulls_target(Dataframe,target) ## Delete target Null Values 
     Dataframe=engin_date(Dataframe)
     Dataframe=Dataframe[list(train.columns)]
-    train_df,test_df=split_dataset(Dataframe,Split_Racio)
+    train_df,test_df=split_dataset(Dataframe,split_ratio)
     train_df,n_cols=Dataframe.copy(),num_cols(Dataframe,target)
     
     n_cols,c_cols=num_cols(train_df,target),cat_cols(train_df,target) 
 
     if enc_method=='Encoding Version 1':
         if len(n_cols)>0:
             scaler,n_cols= fit_StandardScaler(train_df,target)
@@ -169,20 +169,20 @@
              'cols':(list(Dataframe.columns),c_cols,n_cols),
              'scaler':scaler,
              'encod':fit_pre,
              }
     
     return fit_atl
 
-def data_processing(Dataset:pd.DataFrame,
+def data_processing(dataset:pd.DataFrame,
                     fit_atl:dict):
     
-############################## Transformation Procediment ##############################
+############################## Transformation Proceedment ##############################
 
-    df=Dataset.copy()
+    df=dataset.copy()
     
     df=engin_date(df)
     cols,c_cols,n_cols=fit_atl["cols"]
     enc_method,imp_method,target=fit_atl["enc_version"]
     scaler,input_cols=fit_atl["scaler"],c_cols+n_cols
     fit_pre=fit_atl["encod"]
     imputer=fit_atl["null_imputer"]
```

## atlantic/atl_processing.py

```diff
@@ -2,104 +2,108 @@
 import pandas as pd
 import cane
 from sklearn.preprocessing import OneHotEncoder, LabelEncoder, StandardScaler, MinMaxScaler, RobustScaler
 from sklearn.impute import KNNImputer, SimpleImputer, IterativeImputer
 from .atl_feat_eng import num_cols, cat_cols, divide_dfs
 from .atl_performance import pred_eval
 
-def fit_SimpleImp(df:pd.DataFrame,
-                   target:str,
-                   strat:str='mean'):
+def fit_SimpleImp(dataset:pd.DataFrame,
+                  target:str,
+                  strat:str='mean'):
     """
     The fit_SimpleImp function fits a SimpleImputer to the dataframe. 
     The function returns the fitted SimpleImputer object.
     
     :param df:pd.DataFrame: Specify the dataframe that you want to fit
     :param target:str: Specify the target variable
     :param strat:str: Specify the strategy to use when replacing missing values
     :return: A simpleimputer object
     """
     
-    df_=df.copy()
+    df,df_=dataset.copy(),dataset.copy()
     df=df.loc[:, df.columns != target]
     input_cols= list(df.columns)
 
 
     imputer = SimpleImputer(missing_values=np.nan, strategy=strat)
     imputer.fit(df)
     
     return imputer
 
-def transform_SimpleImp(df:pd.DataFrame,
-                         target:str,
-                         imputer):
+def transform_SimpleImp(dataset:pd.DataFrame,
+                        target:str,
+                        imputer):
     """
     The transform_SimpleImp function takes a dataframe and imputes missing values using the SimpleImputer. 
     The function returns a new dataframe with the imputed values in place of NaN's.
 
     :param df:pd.DataFrame: Specify the dataframe that is to be transformed
     :param target:str: Specify the target column in the dataframe
     :param imputer: Select the imputer to be used
     :return: The dataframe with the imputed values in the columns that were transformed
     """
     
+    df=dataset.copy()
     df=df.reset_index(drop=True)  
     df_=df.copy()
     
     df=df.loc[:, df.columns != target]
     input_cols= list(df.columns)
     
     df = imputer.transform(df[input_cols])
     df = pd.DataFrame(df, columns = input_cols)
 
     df_[input_cols]=df[input_cols]
     
     return df_
 
-def fit_KnnImp(df:pd.DataFrame, 
-                target:str, 
-                neighbors:int=5):
+def fit_KnnImp(dataset:pd.DataFrame, 
+               target:str, 
+               neighbors:int=5):
     
-    df_=df.copy()
+    df,df_=dataset.copy(),dataset.copy()
     df=df.loc[:, df.columns != target]
     imputer = KNNImputer(n_neighbors=neighbors)
     imputer.fit(df)
     
     return imputer
 
-def transform_KnnImp(df:pd.DataFrame,
-                      target:str,
-                      imputer):
+def transform_KnnImp(dataset:pd.DataFrame,
+                     target:str,
+                     imputer):
     
+    df=dataset.copy()
     df=df.reset_index(drop=True)
     df_=df.copy()
     
     df=df.loc[:, df.columns != target]
     df = pd.DataFrame(imputer.transform(df),columns = df.columns) 
     
     input_cols= list(df.columns)
     df_[input_cols]=df[input_cols]
     
     return df_
 
-def fit_IterImp(df:pd.DataFrame, 
-                 target:str, 
-                 order:str='ascending'):
-
-    df_=df.copy()
+def fit_IterImp(dataset:pd.DataFrame, 
+                target:str, 
+                order:str='ascending'):
+    
+    df,df_=dataset.copy(),dataset.copy()
+    
     df=df.loc[:, df.columns != target]
     imputer = IterativeImputer(imputation_order=order,max_iter=10,random_state=0,n_nearest_features=None)
     imputer=imputer.fit(df)
 
     return imputer
 
-def transform_IterImp(df:pd.DataFrame,
+def transform_IterImp(dataset:pd.DataFrame,
                       target:str,
                       imputer):
     
+    df=dataset.copy()
     df=df.reset_index(drop=True)
     df_=df.copy()
     
     df=df.loc[:, df.columns != target]
     input_cols= list(df.columns)
     
     df = pd.DataFrame(imputer.transform(df))
@@ -148,15 +152,15 @@
     elif enc_method=='Encoding Version 2':
         train, test=encoding_v2(train, test,target)
     elif enc_method=='Encoding Version 3':
         train, test=encoding_v3(train, test,target)
     elif enc_method=='Encoding Version 4':
         train, test=encoding_v4(train, test,target)
         
-    
+    print('    ')   
     print('Simple Imputation Loading')
     imputer=fit_SimpleImp(train,
                           target=target,
                           strat='mean')
 
     train_simple=transform_SimpleImp(train,
                                      target=target,
@@ -200,18 +204,18 @@
     perf_imp=pd.concat(list_)
     perf_imp=perf_imp.reset_index()
     perf_imp = perf_imp.sort_values([eval_metric], ascending=True)
     
     mae_simple=simple_perf[eval_metric].sum()
     mae_knn=knn_perf[eval_metric].sum()
     mae_Iterartive=iter_perf[eval_metric].sum()
+    print('    ')   
+    print('Predictive Performance Null Imputation Versions:')
     
-    print('Null Imputation Methods Performance:')
-    
-    print('KNN Performance: ', round(mae_knn, 4), '\n Iterative Performance: ', 
+    print(' KNN Performance: ', round(mae_knn, 4), '\n Iterative Performance: ', 
           round(mae_Iterartive, 4),'\n Simple Performance: ', round(mae_simple, 4))
     
     list_imp=[mae_Iterartive,mae_knn,mae_simple]
     
     list_imp.sort()
     imp_method=''
     
@@ -226,15 +230,14 @@
         imp_method='KNN'
         train, test=train_knn.copy(), test_knn.copy()
         print('KNN Imputation Algorithm was chosen with an ', metric, ' of: ', round(mae_knn, 4))
     elif list_imp[0]==mae_simple:
         imp_method='Simple'  
         train, test=train_simple.copy(),test_simple.copy()
         print('Simple Imputation Algorithm was chosen with an ', metric, ' of: ', round(mae_simple, 4))
-
     return train, test,imp_method
 
 
 def encoding_v1(train:pd.DataFrame, test:pd.DataFrame, target:str):
     
     """
     Encoding method version 1.
@@ -314,76 +317,76 @@
         _train=transform_Label_Encoding(_train,le_fit)
         _test=transform_Label_Encoding(_test,le_fit)
     
     return _train,_test
 
 ######### MultiColumn LabelEncoding
 
-def fit_Label_Encoding(Dataset:pd.DataFrame,target:str):
+def fit_Label_Encoding(dataset:pd.DataFrame,target:str):
     """
     This function performs the Label Encoding for categorical variables in a dataset.
     Args:
-        Dataset (pd.DataFrame): The dataset that you want to encode.
+        dataset (pd.DataFrame): The dataset that you want to encode.
         target (str): The name of the target variable.
     Returns:
         le_dict (dict): A dictionary of label encoders for each categorical variable.
     """
-    encoders=cat_cols(Dataset,target)
-    df,list_cols,list_le=Dataset.copy(),[],[]
+    encoders=cat_cols(dataset,target)
+    df,list_cols,list_le=dataset.copy(),[],[]
     
     for c in encoders:
         le = LabelEncoder()
         list_cols.append(c),list_le.append(le.fit(df[c]))
     le_dict = {list_cols[i]: list_le[i] for i in range(len(list_cols))}
     
     return le_dict
 
-def transform_Label_Encoding(Dataset:pd.DataFrame,le_fit:dict):
+def transform_Label_Encoding(dataset:pd.DataFrame,le_fit:dict):
     """
     This function receives a dataset and a pre-trained label encoding dict.
     It maps any unseen values in the dataset to '<unknown>', appends it to the classes_
     array of the label encoder, and then applies the encoding to the dataframe.
     """
     encoders=list(le_fit.keys())
-    df=Dataset.copy()
+    df=dataset.copy()
 
     for c in encoders:
         le=le_fit[c]  
         df[c] = df[c].map(lambda s: '<unknown>' if s not in le.classes_ else s)
         le.classes_ = np.append(le.classes_, '<unknown>')
         df[c] = le.transform(df[c])
         
     return df 
 
 ######### MultiColumn IDF_Encoding 
 
-def fit_IDF_Encoding(Dataset:pd.DataFrame,target:str):
-    df=Dataset.copy()
+def fit_IDF_Encoding(dataset:pd.DataFrame,target:str):
+    df=dataset.copy()
     
     encoders=cat_cols(df,target)
-    IDF_filter = cane.idf(df, n_coresJob=2,disableLoadBar = False, columns_use = encoders)
+    IDF_filter = cane.idf(df, n_coresJob=2,disableLoadBar = True, columns_use = encoders)
     idf_fit = cane.idfDictionary(Original = df, Transformed = IDF_filter, columns_use = encoders)
 
     return idf_fit
 
-def transform_IDF_Encoding(Dataset:pd.DataFrame,idf_fit:dict):
+def transform_IDF_Encoding(dataset:pd.DataFrame,idf_fit:dict):
     
     encoders=list(idf_fit.keys())
-    df=Dataset.copy()
+    df=dataset.copy()
         
     for col in encoders:
         df[col] = (df[col].map(idf_fit[col]).fillna(max(idf_fit[col].values())))
         
     return df 
 
 ######### MultiColumn OneHotEncoding
 
-def fit_OneHot_Encoding(Dataset:pd.DataFrame,target:str,n_distinct:int=10):
+def fit_OneHot_Encoding(dataset:pd.DataFrame,target:str,n_distinct:int=10):
         
-    df,list_cols,list_le=Dataset.copy(),[],[]
+    df,list_cols,list_le=dataset.copy(),[],[]
     drop_org_cols,list_ohe=True,[] 
     encoders=cat_cols(df,target)
 
     if len(encoders)>0:
         for enc in encoders:
             if len(list(dict.fromkeys(df[enc].tolist())))<=n_distinct:  ## Less than n distinct elements in col
                 ohe = OneHotEncoder(handle_unknown = 'ignore')
@@ -391,17 +394,17 @@
                 list_cols.append(enc),list_le.append(ohe.fit(df[[enc]]))
     
     ohe_fit = {list_cols[i]: list_le[i] for i in range(len(list_cols))}
     ohe_fit["n_distinct"]=n_distinct
     
     return ohe_fit
 
-def transform_OneHot_Encoding(Dataset:pd.DataFrame,ohe_fit:dict):
+def transform_OneHot_Encoding(dataset:pd.DataFrame,ohe_fit:dict):
     
-    df= Dataset.copy()
+    df= dataset.copy()
     drop_org_cols,list_ohe,n_distinct=True,[],ohe_fit["n_distinct"]
     del ohe_fit["n_distinct"]
     encoders=list(ohe_fit.keys())
 
     if len(encoders)>0:
         for enc in encoders:
             col_n=[]
@@ -419,35 +422,35 @@
                 df = pd.concat([df, df_copy.set_index(df.index)], axis=1)
     df,ohe_fit['n_distinct']=df.drop(list_ohe, axis=1),n_distinct
     
     return df
 
 ############################# Scalers
 
-def fit_StandardScaler(Dataset:pd.DataFrame,target:str):
+def fit_StandardScaler(dataset:pd.DataFrame,target:str):
     
-    df,n_cols=Dataset.copy(),num_cols(Dataset,target)
+    df,n_cols=dataset.copy(),num_cols(dataset,target)
     
     scaler = StandardScaler()
     scaler = scaler.fit(df[n_cols])
 
     return scaler, n_cols
 
-def fit_MinmaxScaler(Dataset:pd.DataFrame,target:str):
+def fit_MinmaxScaler(dataset:pd.DataFrame,target:str):
     
-    df,n_cols=Dataset.copy(),num_cols(Dataset,target)
+    df,n_cols=dataset.copy(),num_cols(dataset,target)
     
     scaler = MinMaxScaler() 
     scaler = scaler.fit(df[n_cols])
 
     return scaler, n_cols
 
-def fit_RobustScaler(Dataset:pd.DataFrame,target:str):
+def fit_RobustScaler(dataset:pd.DataFrame,target:str):
     
-    df,n_cols=Dataset.copy(),num_cols(Dataset,target)
+    df,n_cols=dataset.copy(),num_cols(dataset,target)
     
     scaler = RobustScaler()
     scaler = scaler.fit(df[n_cols])
     
     return scaler, n_cols
 
 
@@ -544,10 +547,11 @@
     elif list_encoding[0]==p_v3:
         enc_method='Encoding Version 3'
         print('Encoding Version 3 was choosen with an ', metric, ' of: ', round(p_v3, 4))
     
     elif list_encoding[0]==p_v4:
         enc_method='Encoding Version 4'
         print('Encoding Version 4 was choosen with an ', metric, ' of: ', round(p_v4, 4))
-    
+        print(' ')
+        
     return enc_method
```

## Comparing `atlantic-1.0.25.dist-info/LICENSE` & `atlantic-1.0.50.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `atlantic-1.0.25.dist-info/METADATA` & `atlantic-1.0.50.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: atlantic
-Version: 1.0.25
-Summary: Atlantic is an automated preprocessing framework for supervised machine learning
+Version: 1.0.50
+Summary: Atlantic is an automated preprocessing framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/Atlantic
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data processing,predictive modeling,data preprocessing,automated data preprocessing,automated machine learning,automl
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas (>=1.2.0)
 Requires-Dist: numpy (>=1.19.5)
 Requires-Dist: cane (>=2.3.1)
-Requires-Dist: scikit-learn (>=1.0.2)
+Requires-Dist: scikit-learn (>=1.2.2)
 Requires-Dist: statsmodels (>=0.13.2)
 Requires-Dist: h2o (>=3.40.0.2)
 
 <br>
 <p align="center">
   <h2 align="center"> Atlantic - Automated Data Preprocessing Framework for Supervised Machine Learning
   <br>
@@ -48,22 +48,22 @@
     
    
 #### Main Development Tools <a name = "pre1"></a>
 
 Major frameworks used to built this project: 
    
 * [H2O.ai](https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html)
-* [Sklearn](https://scikit-learn.org/stable/)
+* [Scikit-learn](https://scikit-learn.org/stable/)
 * [Pandas](https://pandas.pydata.org/)
 
     
 ## Framework Architecture <a name = "ta"></a>
 
 <p align="center">
-  <img src="https://i.ibb.co/BjmYGrz/ATL-Architecture.png" align="center" width="800" height="650" />
+  <img src="https://i.ibb.co/nb3Wh2X/ATL-Architecture-Final.png" align="center" width="700" height="680" />
 </p>    
 
 ## Where to get it <a name = "ta"></a>
 
 Binary installer for the latest released version is available at the Python Package Index [PyPI](https://pypi.org/project/atlantic/).  
 
 The source code is currently hosted on GitHub at: https://github.com/TsLu1s/Atlantic
@@ -77,48 +77,48 @@
 ```
 
 # Usage Examples
     
 ## 1. Atlantic - Automated Data Preprocessing Pipeline
 
 In order to be able to apply the automated preprocessing `atlantic` pipeline you need first to import the package. 
-The following needed step is to load a dataset and define your to be predicted target column name into the variable `Target` and define split ratio for your Train and Test subsets.
+The following needed step is to load a dataset and define your to be predicted target column name into the variable `Target` and define split ratio for your Train and Validation subsets.
 You can customize the main function (customizable option) by altering the following running pipeline parameters:
-* Split_Racio: Division ratio in which the preprocessing methods will be evaluated within the loaded Dataset.
+* split_ratio: Division ratio in which the preprocessing methods will be evaluated within the loaded Dataset.
 * total_vi: Minimal value of the total sum of relative variable\feature importance percentage selected in the "H2O AutoML feature selection" step.
 * h2o_fs_models: Quantity of models generated for competition in step "H2O AutoML feature selection" to evaluate the relative importance of each feature (only leaderboard model will be selected for evaluation).
 * encoding_fs: You can choose if you want to encond your features in order to reduce loading time in "H2O AutoML feature selection" step. If in "True" mode label encoding is applied to categorical features.
 * vif_ratio: This value defines the minimal 'threshold' for Variance Inflation Factor filtering (default value=10).
  
 Importante Notes:
     
 * Default predictive evaluation metric for regression contexts is MAE (Mean Absolute Error) and classification is AUC (Accuracy).
 * Although functional, `Atlantic` data processing is not optimized for big data purposes yet.
-* Major update is now available in **versions>=1.0.1**
+* Major update is now available in **versions>=1.0.5**
     
 ```py
     
 import atlantic as atl
 import pandas as pd   
     
 data = pd.read_csv('csv_directory_path', encoding='latin', delimiter=',') # Dataframe Loading Example
 
-train,test=atl.split_dataset(data,Split_Racio=0.8) 
+train,test=atl.split_dataset(data,split_ratio=0.8) 
 
 ### Fit Data Processing
     
 # Simple Option
-fit_atl = atl.fit_processing(Dataset=train,           # Dataset:pd.DataFrame, target:str="Target_Column"
-                             target="Target_Column",  # Split_Racio:float=0.75 [0.5,0.95[ -> Recommended
-                             Split_Racio=0.75)
+fit_atl = atl.fit_processing(dataset=train,           # dataset:pd.DataFrame, target:str="Target_Column"
+                             target="Target_Column",  # split_ratio:float=0.75 [0.5,0.95[ -> Recommended
+                             split_ratio=0.75)
     
 # Customizable Option
-fit_atl = atl.fit_processing(Dataset=train,                  # Dataset:pd.DataFrame, 
+fit_atl = atl.fit_processing(dataset=train,                  # dataset:pd.DataFrame, 
                              target="Target_Column",         # target:str="Target_Column"
-                             Split_Racio=0.75,               # Split_Racio:float=0.75, total_vi:float=0.98 [0.5,1]
+                             split_ratio=0.75,               # split_ratio:float=0.75, total_vi:float=0.98 [0.5,1]
                              total_vi=0.98,                  # h2o_fs_models:int [1,50], encoding_fs:bool=True\False
                              h2o_fs_models=7,                # vif_ratio:float=10.0 [3,30]
                              encoding_fs=True,
                              vif_ratio=10.0)
 
 ### Transform Data Processing
     
@@ -137,16 +137,16 @@
  
 * Note : `n_distinct` costumizable parameter in `OneHotEncoder` function constitutes the max limiter of distinct elements in columns, this meaning, columns with higher distinct values then 'n_distinct' will not be encoded.    
 
 ```py
 import atlantic as atl
 import pandas as pd 
 
-train, test = atl.split_dataset(Dataset,Split_Racio=0.75) # Split Initial Dataframe
-                                                          # Dataset:pd.DataFrame, Split_Racio:float
+train, test = atl.split_dataset(dataset,split_ratio=0.75) # Split Initial Dataframe
+                                                          # dataset:pd.DataFrame, split_ratio:float
 target = "Target_Column" # -> target feature name
     
 ## Encoders
 # MultiColumn LabelEncoder
 
 le_fit=atl.fit_Label_Encoding(train,target)  
 train=atl.transform_Label_Encoding(train,le_fit)
@@ -177,89 +177,63 @@
     
     
 * [VIF Feature Selection (Variance Inflation Factor)](https://www.investopedia.com/terms/v/variance-inflation-factor.asp) - Variance inflation factor aims at measuring the amount of multicollinearity in a set of multiple regression variables or features, therefore for this filtering function to be applied all input variables need to be of numeric type. It can be customized by changing the column selection treshold (VIF:float) designated with a default value of 10.
     
     
 ```py    
     
-selected_columns, h2o_importance = atl.feature_selection_h2o(Dataset, # Dataset:pd.DataFrame ,target:str="Target_Column",
+selected_columns, h2o_importance = atl.feature_selection_h2o(dataset,     # dataset:pd.DataFrame ,target:str="Target_Column",
                                                              target,      #  total_vi:float [0.5,1], h2o_fs_models:int [1,50], encoding_fs:bool=True/False
                                                              total_vi=0.98,     
                                                              h2o_fs_models =7,
                                                              encoding_fs=True)
 
 
-selected_columns, vif_importance = atl.feature_selection_vif(Dataset, # Dataset:pd.DataFrame, target:str="Target_Column",
+selected_columns, vif_importance = atl.feature_selection_vif(dataset, # dataset:pd.DataFrame, target:str="Target_Column",
                                                              target,  # VIF:float [3,30]
                                                              VIF=10.0)
 ```
     
 ### 2.3 Datetime Feature Engineering
 
 The engin_date function converts and transforms columns of Datetime type into additional columns (Year, Day of the Year, Season, Month, Day of the month, Day of the week, Weekend, Hour, Minute) which will be added by association to the input dataset and subsequently deletes the original column if parameter drop=True.
     
     
 ```py   
     
-dataset = atl.engin_date(Dataset,drop=False) # Dataset:pd.DataFrame, drop:bool
+dataset = atl.engin_date(dataset,drop=False) # dataset:pd.DataFrame, drop:bool
     
 ```
 
-### 2.4 Predictive Performance Metrics
-
-You can analyse the obtained predictive performance results by using the given bellow functions witch contains the most used metrics for each supervised predictive context.
-    
-    
-```py  
-
-reg_performance = pd.DataFrame(atl.metrics_regression(y_true,y_pred),index=[0])    # y_true:list, y_pred:list
-    
-binary_class_Performance = pd.DataFrame(atl.metrics_binary_classification(y_true,y_pred),index=[0])    # y_true:list, y_pred:list
-    
-multiclass_performance = pd.DataFrame(atl.metrics_classification(y_true,y_pred),index=[0])    # y_true:list, y_pred:list
+### 2.4 Null Imputation Auxiliar Functions
     
-```
-
-### 2.5 Extra Auxiliar Functions
-    
-The following functions were used in the development of this project.
+The following simplified multivariate null imputation methods based from [Sklearn](https://scikit-learn.org/stable/modules/impute.html) can be used through this package.
     
 ```py  
     
-#### Data Preprocessing 
-
-atl.num_cols(Dataset:pd.DataFrame,
-             target:str) # return list_num_cols
-    
-atl.cat_cols(Dataset:pd.DataFrame,
-             target:str) # return list_cat_cols
-    
-atl.remove_columns_by_nulls(Dataset:pd.DataFrame,
-                            percentage:int) # return dataset
-
 ## Simplified Null Imputation (Only numeric features)
 
-imputer_knn=atl.fit_KnnImp(df:pd.DataFrame,
+imputer_knn=atl.fit_KnnImp(dataset:pd.DataFrame,
                            target:str,
                            neighbors:int=5)
-df=atl.transform_KnnImp(df:pd.DataFrame,
+df=atl.transform_KnnImp(dataset:pd.DataFrame,
                         target:str,
                         imputer=imputer_knn)
 
-imputer_simple=atl.fit_SimpleImp(df:pd.DataFrame,
+imputer_simple=atl.fit_SimpleImp(dataset:pd.DataFrame,
                                  target:str,
                                  strat:str='mean')
-df=atl.transform_SimpleImp(df:pd.DataFrame,
+df=atl.transform_SimpleImp(dataset:pd.DataFrame,
                            target:str,
                            imputer=imputer_simple)
     
-imputer_iter=atl.fit_IterImp(df:pd.DataFrame, 
+imputer_iter=atl.fit_IterImp(dataset:pd.DataFrame, 
                              target:str, 
                              order:str='ascending')
-df=atl.transform_IterImp(df:pd.DataFrame,
+df=atl.transform_IterImp(dataset:pd.DataFrame,
                          target:str,
                          imputer=imputer_iter)
 ```   
     
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/TsLu1s/Atlantic/blob/main/LICENSE) for more information.
```

## Comparing `atlantic-1.0.25.dist-info/RECORD` & `atlantic-1.0.50.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 atlantic/__init__.py,sha256=aJxiUy0U6d3cxOQQo5m4ATN4A3xAGwAFCqCl21JTvhM,389
-atlantic/atl_feat_eng.py,sha256=K50TMd3XuBC_RbKZh5P8El-nen9ixboTVKF9j1H1B4s,5510
-atlantic/atl_feat_selection.py,sha256=biaTXW6-1njQoutO_3MIb8WkzHWDpbB99U29PsuB92E,8705
-atlantic/atl_metrics.py,sha256=cw0XV2tdU8hTv3E5eyy3G2-FbPXSDsJpVIvsv62Gsfk,2351
-atlantic/atl_performance.py,sha256=F8AbtgwPALAhhI8iSRyW2-3zskMb0NLugMfdcTlE4o0,2889
-atlantic/atl_pipeline.py,sha256=1zHFcy6SXyxUSrEM8YQj0CP3ZrqDLS3QMMF1ncmgNeo,8538
-atlantic/atl_processing.py,sha256=flF82kihrJL8tMMasgrltBnLHXTLjl0Vc1TB8NWpB7o,20380
-atlantic-1.0.25.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
-atlantic-1.0.25.dist-info/METADATA,sha256=UqU_poQ50-FvwPSCWzFfzUx9DFKZm-pLnmy6PJtq67c,13159
-atlantic-1.0.25.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-atlantic-1.0.25.dist-info/top_level.txt,sha256=RAc3T5Fn4vx9TZ0hPSO3jINJDLLfOOLdANbFmLJQAnU,9
-atlantic-1.0.25.dist-info/RECORD,,
+atlantic/atl_feat_eng.py,sha256=qTxn3NxyT_GRR4gdmlLCIrNfL5xViqZEQ29iQpo8cug,5510
+atlantic/atl_feat_selection.py,sha256=r1H8N7DEbbNgo8jUT9kA-5JRmc9v1WVZ3Bf1zU-ACAI,8704
+atlantic/atl_metrics.py,sha256=ZbP98YCmgf0UTiCtozQDRzVARP4EWy9GvzqbQ1XcJ_s,1563
+atlantic/atl_performance.py,sha256=uhTLsE0yuzBGaCxisz30KdpqRSgpEIab3eYMMwsgd2w,2858
+atlantic/atl_pipeline.py,sha256=Fn77_CUA09jZNXkgUJc3yqGWBu7KNBXmcC6eLJU-7qc,8541
+atlantic/atl_processing.py,sha256=QkSVuSFLb3JtvCZbEuDckn4MGjQdeLAQJ2ZifKCp3TA,20614
+atlantic-1.0.50.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
+atlantic-1.0.50.dist-info/METADATA,sha256=AvRNxZoe1bt1Aj9UBitNzqABMNyjvWkl5JXVIXPx6PU,12367
+atlantic-1.0.50.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+atlantic-1.0.50.dist-info/top_level.txt,sha256=RAc3T5Fn4vx9TZ0hPSO3jINJDLLfOOLdANbFmLJQAnU,9
+atlantic-1.0.50.dist-info/RECORD,,
```

