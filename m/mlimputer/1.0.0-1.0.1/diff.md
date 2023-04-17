# Comparing `tmp/mlimputer-1.0.0-py3-none-any.whl.zip` & `tmp/mlimputer-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9269 bytes, number of entries: 9
+Zip file size: 9238 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      389 b- defN 23-Feb-20 00:15 mlimputer/__init__.py
--rw-rw-rw-  2.0 fat     4675 b- defN 23-Feb-20 15:35 mlimputer/mli_imputation.py
--rw-rw-rw-  2.0 fat     6396 b- defN 23-Feb-20 16:05 mlimputer/mli_model_selection.py
--rw-rw-rw-  2.0 fat     1402 b- defN 23-Mar-12 00:24 mlimputer/mli_parameters.py
--rw-rw-rw-  2.0 fat     1090 b- defN 23-Mar-12 16:18 mlimputer-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7003 b- defN 23-Mar-12 16:18 mlimputer-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-12 16:18 mlimputer-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Mar-12 16:18 mlimputer-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      730 b- defN 23-Mar-12 16:18 mlimputer-1.0.0.dist-info/RECORD
-9 files, 21787 bytes uncompressed, 8011 bytes compressed:  63.2%
+-rw-rw-rw-  2.0 fat     4690 b- defN 23-Apr-17 14:04 mlimputer/mli_imputation.py
+-rw-rw-rw-  2.0 fat     6326 b- defN 23-Apr-17 14:00 mlimputer/mli_model_selection.py
+-rw-rw-rw-  2.0 fat     1402 b- defN 23-Apr-17 14:19 mlimputer/mli_parameters.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 23-Apr-17 14:48 mlimputer-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7003 b- defN 23-Apr-17 14:48 mlimputer-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 14:48 mlimputer-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-17 14:48 mlimputer-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      730 b- defN 23-Apr-17 14:48 mlimputer-1.0.1.dist-info/RECORD
+9 files, 21732 bytes uncompressed, 7980 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: mlimputer/mli_model_selection.py
 Comment: 
 
 Filename: mlimputer/mli_parameters.py
 Comment: 
 
-Filename: mlimputer-1.0.0.dist-info/LICENSE
+Filename: mlimputer-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: mlimputer-1.0.0.dist-info/METADATA
+Filename: mlimputer-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: mlimputer-1.0.0.dist-info/WHEEL
+Filename: mlimputer-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: mlimputer-1.0.0.dist-info/top_level.txt
+Filename: mlimputer-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mlimputer-1.0.0.dist-info/RECORD
+Filename: mlimputer-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlimputer/mli_imputation.py

```diff
@@ -4,121 +4,121 @@
 from tqdm import tqdm
 import atlantic as atl
 from .mli_parameters import imputer_parameters
 from .mli_model_selection import missing_report, imput_models
 
 parameters=imputer_parameters()
 
-def fit_imput(Dataset:pd.DataFrame,
+def fit_imput(dataset:pd.DataFrame,
               imput_model:str,
               imputer_configs:dict=parameters):
     
     """
     This function fits missing data in a pandas dataframe using the imputation method specified by the user.
     
     Parameters:
-    Dataset (pd.DataFrame): The input pandas dataframe that needs to be imputed.
+    dataset (pd.DataFrame): The input pandas dataframe that needs to be imputed.
     imput_model (str, optional): The imputation method to be used. Default is "KNN".
     
     Returns:
     imp_config (dict): A dictionary containing the fitted imputation models for each column with missing data.
     """      
     
-    df=Dataset.copy()
+    df=dataset.copy()
 
     df_md,c=missing_report(df),0
     imp_targets=list(df_md['columns']) 
         
     # Iterate over each column with missing data and fit the imputation method
     for col in tqdm(imp_targets, desc="Fitting Missing Data Columns", ncols=80): ## imp_targets:
         #print("**** Fitting Column:", col)
-        Target=col
+        target=col
         
         # Split the data into train and test sets
         total_index = df.index.tolist()
-        test_index = df[df[Target].isnull()].index.tolist()
+        test_index = df[df[target].isnull()].index.tolist()
         train_index = [value for value in total_index if value not in test_index]
         
-        Train=df.iloc[train_index]
+        train=df.iloc[train_index]
         
         # Fit the label encoding method in categorical columns
-        le_fit=atl.fit_Label_Encoding(Train,Target)
-        Train=atl.transform_Label_Encoding(Train,le_fit)
+        le_fit=atl.fit_Label_Encoding(train,target)
+        train=atl.transform_Label_Encoding(train,le_fit)
         
         # Fit the simple imputation method in input columns
-        imputer_simple=atl.fit_SimpleImp(df=Train,
-                                         target=Target,
+        imputer_simple=atl.fit_SimpleImp(dataset=train,
+                                         target=target,
                                          strat='mean')
         
-        Train=atl.transform_SimpleImp(df=Train,
-                                      target=Target,
+        train=atl.transform_SimpleImp(dataset=train,
+                                      target=target,
                                       imputer=imputer_simple)
         # Fit the imputation model
-        model = imput_models(Train=Train,
-                             target=Target,
+        model = imput_models(train=train,
+                             target=target,
                              parameters=imputer_configs,
                              algo=imput_model)
         
         # Store the fitted model information in a dictionary
         if c==0:
-            imp_config = {Target:{'model_name':imput_model,
+            imp_config = {target:{'model_name':imput_model,
                                   'model':model,
                                   'pre_process':le_fit,
                                   'input_nulls':imputer_simple}}
         elif c>0:
-            imp_config_2 = {Target:{'model_name':imput_model,
+            imp_config_2 = {target:{'model_name':imput_model,
                                     'model':model,
                                     'pre_process':le_fit,
                                     'input_nulls':imputer_simple}}
             imp_config.update(imp_config_2)
         c+=1
         
     return imp_config
 
-def transform_imput(Dataset:pd.DataFrame,
+def transform_imput(dataset:pd.DataFrame,
                     fit_configs:dict):
     """
     Imputation of missing values in a dataset using a pre-fit imputation model.
     
     Parameters:
     -----------
-    Dataset: pd.DataFrame
+    dataset: pd.DataFrame
         The dataset containing missing values to be imputed.
     fit_configs: dict
         A dictionary of pre-fit imputation models and associated pre-processing information
         for each column with missing values in the dataset.
         
     Returns:
     --------
     df_: pd.DataFrame
         The original dataset with missing values imputed.
     """
-    df_,imp_cols=Dataset.copy(),list(fit_configs.keys()) #[0]
+    df_,imp_cols=dataset.copy(),list(fit_configs.keys()) #[0]
     
     for col in tqdm(imp_cols, desc="Imputing Missing Data", ncols=80):#in imp_cols:
         
-        Target=col
-        test_index = df_[df_[Target].isnull()].index.tolist()
+        target=col
+        test_index = df_[df_[target].isnull()].index.tolist()
         test_df=df_.iloc[test_index]
         
-        le_fit=fit_configs[Target]['pre_process']
+        le_fit=fit_configs[target]['pre_process']
         test_df=atl.transform_Label_Encoding(test_df,le_fit)
-        input_num_cols = atl.num_cols(test_df, Target)
+        input_num_cols = atl.num_cols(test_df, target)
         
-        imputer_simple=fit_configs[Target]['input_nulls']
-        test_df=atl.transform_SimpleImp(df=test_df,
-                                        target=Target,
+        imputer_simple=fit_configs[target]['input_nulls']
+        test_df=atl.transform_SimpleImp(dataset=test_df,
+                                        target=target,
                                         imputer=imputer_simple)
         
         sel_cols=list(test_df.columns)
-        sel_cols.remove(Target)
-        sel_cols.append(Target)
+        sel_cols.remove(target)
+        sel_cols.append(target)
         test_df=test_df[sel_cols]
         X_test = test_df.iloc[:, 0:(len(sel_cols)-1)].values
 
-        model=fit_configs[Target]['model']
+        model=fit_configs[target]['model']
     
         y_predict = model.predict(X_test)
 
-        df_[Target].iloc[test_index]=y_predict
+        df_[target].iloc[test_index]=y_predict
 
     return df_
```

## mlimputer/mli_model_selection.py

```diff
@@ -11,38 +11,38 @@
 import catboost as cb
 import xgboost
 import lightgbm as lgb 
 from .mli_parameters import imputer_parameters
 
 parameters=imputer_parameters()
 
-def imput_models(Train:pd.DataFrame,
+def imput_models(train:pd.DataFrame,
                  target:str="y",
                  algo:str='RandomForest',
                  parameters:dict=parameters):
     """
     This function trains and returns a regression model based on the input data and specified algorithm.
     
     Parameters:
-    Train (pd.DataFrame): The input training data
+    train (pd.DataFrame): The input training data
     target (str, optional): The target column name in the training data. Default is 'y'
     algo (str, optional): The algorithm to be used for training. Default is 'RandomForest'
     parameters (dict, optional): The hyperparameters for the specified algorithm. Default is 'parameters'
     
     Returns:
-    model: Trained machine learning model.
+    model: trained machine learning model.
     """
     
-    sel_cols=list(Train.columns)
+    sel_cols=list(train.columns)
     sel_cols.remove(target)
     sel_cols.append(target)
-    Train=Train[sel_cols]
+    train=train[sel_cols]
     
-    X_train = Train.iloc[:, 0:(len(sel_cols)-1)].values
-    y_train = Train.iloc[:, (len(sel_cols)-1)].values
+    X_train = train.iloc[:, 0:(len(sel_cols)-1)].values
+    y_train = train.iloc[:, (len(sel_cols)-1)].values
     
     if algo=='RandomForest':
         rf_params=parameters['RandomForest']
         model = RandomForestRegressor(**rf_params) 
         model.fit(X_train, y_train)
         
     elif algo=='ExtraTrees':
@@ -76,49 +76,49 @@
         model = lgb.train(lb_params, train_data, num_boost_round=100)
         
     else:
         raise ValueError('Invalid model')
    
     return model
 
-def missing_report(Dataset:pd.DataFrame):
+def missing_report(dataset:pd.DataFrame):
     """
     This function generates a report of missing values in a given dataset.
     
     Parameters:
-    Dataset (pd.DataFrame): The input data to be analyzed for missing values
+    dataset (pd.DataFrame): The input data to be analyzed for missing values
     
     Returns:
     df_md (pd.DataFrame): A dataframe containing the count and percentage of missing values 
     for each numerical column in the input dataset. 
     Sorted by the percentage of missing values in ascending order. <-***********
     """
     
-    df=Dataset.copy()
+    df=dataset.copy()
     
     num_cols=df.select_dtypes(include=['int','float']).columns.tolist()
     df_md = pd.DataFrame(df[num_cols].isna().sum().loc[df[num_cols].isna().sum() > 0], columns=['missing_data_count'])
     df_md['missing_data_percentage'] = df_md['missing_data_count'] / len(df)
     df_md = df_md.sort_values(by='missing_data_percentage', ascending=True)
     df_md['columns']=df_md.index
     df_md=df_md.reset_index(drop=True)
     
     return df_md
 
-def cross_validation(Dataset:pd.DataFrame, target:str, test_size:float=0.2, n_splits:int=5,models:list=[]):#=[LinearRegression(), RandomForestRegressor(), CatBoostRegressor()]):
+def cross_validation(dataset:pd.DataFrame, target:str, test_size:float=0.2, n_splits:int=5,models:list=[]):
     """
     This function performs cross-validation on the given dataset. The dataset is divided into training and test sets, 
     and then each model from the list is fit and evaluated on the test set. The performance of each model on the test
     set is recorded in the form of various metrics, such as accuracy, precision, recall, F1-score, etc. (depending on
     whether the target variable is a continuous variable or a categorical variable). The final result of the function
     is a leaderboard containing the metrics of each model for each fold of the cross-validation.
     
     Parameters:
     -----------
-    Dataset: pd.DataFrame
+    dataset: pd.DataFrame
         The input dataset to be evaluated.
     target: str
         The name of the target column.
     test_size: float, optional (default=0.2)
         The size of the test set, specified as a fraction of the input dataset.
     n_splits: int, optional (default=5)
         The number of folds for cross-validation.
@@ -127,18 +127,18 @@
         
     Returns:
     --------
     leaderboard: pd.DataFrame
         A dataframe containing the performance metrics of each model for each fold of the cross-validation.
     """
     
-    y,list_metrics=Dataset[target],[]
-    sv_pred=atl.target_type(Dataset, target)[0]
+    y,list_metrics=dataset[target],[]
+    sv_pred=atl.target_type(dataset, target)[0]
     for i in range(n_splits):
-        X_train, X_test, y_train, y_test = train_test_split(Dataset, y, test_size=test_size)
+        X_train, X_test, y_train, y_test = train_test_split(dataset, y, test_size=test_size)
         print(f"Fold number: {i + 1}")
 
         X_train,X_test=X_train.drop([target], axis=1),X_test.drop([target], axis=1)
         for model in models:
             print(f"Fitting {model.__class__.__name__} model")
             model.fit(X_train, y_train)
             y_pred = model.predict(X_test)
```

## Comparing `mlimputer-1.0.0.dist-info/LICENSE` & `mlimputer-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlimputer-1.0.0.dist-info/METADATA` & `mlimputer-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlimputer
-Version: 1.0.0
+Version: 1.0.1
 Summary: MLimputer - Null Imputation Framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/MLimputer
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data preprecessing,null imputation,predictive null imputation,multiple null imputation,automated machine learning
 Classifier: Intended Audience :: Education
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn (>=1.0.2)
-Requires-Dist: atlantic (>=1.0.12)
+Requires-Dist: atlantic (>=1.0.50)
 Requires-Dist: catboost (>=1.1.1)
 Requires-Dist: xgboost (>=1.7.3)
 Requires-Dist: lightgbm (>=3.3.5)
 
 <br>
 <p align="center">
   <h2 align="center"> MLimputer - Null Imputation Framework for Supervised Machine Learning
@@ -110,33 +110,33 @@
 # Customizing parameters settings
 hparameters["RandomForest"]["n_estimators"]=40
 hparameters["KNN"]["n_neighbors"]=5
 print(hparameters)
     
 # Imputation Example 1 : RandomForest
 
-imputer_rf=mli.fit_imput(Dataset=train,imput_model="RandomForest",imputer_configs=hparameters)
-train_rf=mli.transform_imput(Dataset=train,fit_configs=imputer_rf)
-test_rf=mli.transform_imput(Dataset=test,fit_configs=imputer_rf)
+imputer_rf=mli.fit_imput(dataset=train,imput_model="RandomForest",imputer_configs=hparameters)
+train_rf=mli.transform_imput(dataset=train,fit_configs=imputer_rf)
+test_rf=mli.transform_imput(dataset=test,fit_configs=imputer_rf)
 
 # Imputation Example 2 : KNN
 
-imputer_knn=mli.fit_imput(Dataset=train,imput_model="KNN",imputer_configs=hparameters)
-train_knn=mli.transform_imput(Dataset=train,fit_configs=imputer_knn)
-test_knn=mli.transform_imput(Dataset=test,fit_configs=imputer_knn)
+imputer_knn=mli.fit_imput(dataset=train,imput_model="KNN",imputer_configs=hparameters)
+train_knn=mli.transform_imput(dataset=train,fit_configs=imputer_knn)
+test_knn=mli.transform_imput(dataset=test,fit_configs=imputer_knn)
     
 #(...)
     
 ## Performance Evaluation Example - Imputation CrossValidation
 
 from sklearn.linear_model import LinearRegression
 from sklearn.ensemble import RandomForestRegressor
 from catboost import CatBoostRegressor
         
-leaderboard_knn_imp=mli.cross_validation(Dataset=train_knn,
+leaderboard_knn_imp=mli.cross_validation(dataset=train_knn,
                                          target="Target_Name_Col", 
                                          test_size=0.2,
                                          n_splits=3,
                                          models=[LinearRegression(), RandomForestRegressor(), CatBoostRegressor()])
 
 ## Export Imputation Metadata
```

## Comparing `mlimputer-1.0.0.dist-info/RECORD` & `mlimputer-1.0.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlimputer/__init__.py,sha256=aJxiUy0U6d3cxOQQo5m4ATN4A3xAGwAFCqCl21JTvhM,389
-mlimputer/mli_imputation.py,sha256=SgYHmmEvt8DaF1xEp6szzhofVfsYIBX0swD-Qy05Cmo,4675
-mlimputer/mli_model_selection.py,sha256=494B_MJ1Rgk3wtTQyZ0ALuITKEH16E-TQkYHvef9zrk,6396
+mlimputer/mli_imputation.py,sha256=yENGhTnMbEUDsiVigut_vRbVURIfavzxX7wSkM8sSjc,4690
+mlimputer/mli_model_selection.py,sha256=s9LzNJawB09psQ6LRzRWSDAegB8LT6RPWv2lSRv51_E,6326
 mlimputer/mli_parameters.py,sha256=G6x291YIhf--4jdv4gaBNsaxknTKjnqBdl73KEmTPfU,1402
-mlimputer-1.0.0.dist-info/LICENSE,sha256=BMKwnVd_OgrW1_Ls-_WlfHpr-s7KFtcT6t9t9tfFk8g,1090
-mlimputer-1.0.0.dist-info/METADATA,sha256=-KIhOffdOUu055zoScuQENi7Kx1fbH3VGflulzfB2sQ,7003
-mlimputer-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mlimputer-1.0.0.dist-info/top_level.txt,sha256=6qseujMDdh0A5GoDaKPU6kp9vnXciE1XKZIvz88dVzE,10
-mlimputer-1.0.0.dist-info/RECORD,,
+mlimputer-1.0.1.dist-info/LICENSE,sha256=BMKwnVd_OgrW1_Ls-_WlfHpr-s7KFtcT6t9t9tfFk8g,1090
+mlimputer-1.0.1.dist-info/METADATA,sha256=FDlwms_ysLJsvbnOmYcLl48brhRYlIfbyI7JlnREFFo,7003
+mlimputer-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mlimputer-1.0.1.dist-info/top_level.txt,sha256=6qseujMDdh0A5GoDaKPU6kp9vnXciE1XKZIvz88dVzE,10
+mlimputer-1.0.1.dist-info/RECORD,,
```

