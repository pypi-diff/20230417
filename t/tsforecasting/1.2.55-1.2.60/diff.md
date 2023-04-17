# Comparing `tmp/tsforecasting-1.2.55-py3-none-any.whl.zip` & `tmp/tsforecasting-1.2.60-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18951 bytes, number of entries: 12
+Zip file size: 18625 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      393 b- defN 23-Feb-21 11:35 tsforecasting/__init__.py
--rw-rw-rw-  2.0 fat    10033 b- defN 23-Feb-21 11:43 tsforecasting/tsf_data_eng.py
--rw-rw-rw-  2.0 fat    10117 b- defN 23-Mar-12 17:15 tsforecasting/tsf_expanding_window.py
+-rw-rw-rw-  2.0 fat    10033 b- defN 23-Apr-17 15:36 tsforecasting/tsf_data_eng.py
+-rw-rw-rw-  2.0 fat    10134 b- defN 23-Apr-17 16:08 tsforecasting/tsf_expanding_window.py
 -rw-rw-rw-  2.0 fat     1684 b- defN 23-Mar-02 11:05 tsforecasting/tsf_model_configs.py
--rw-rw-rw-  2.0 fat     4009 b- defN 23-Mar-12 17:43 tsforecasting/tsf_model_selection.py
--rw-rw-rw-  2.0 fat     7891 b- defN 23-Mar-01 16:13 tsforecasting/tsf_performance.py
--rw-rw-rw-  2.0 fat     8386 b- defN 23-Mar-12 17:15 tsforecasting/tsf_predictions.py
--rw-rw-rw-  2.0 fat     1078 b- defN 23-Mar-12 17:50 tsforecasting-1.2.55.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    12346 b- defN 23-Mar-12 17:50 tsforecasting-1.2.55.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-12 17:50 tsforecasting-1.2.55.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Mar-12 17:50 tsforecasting-1.2.55.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1047 b- defN 23-Mar-12 17:50 tsforecasting-1.2.55.dist-info/RECORD
-12 files, 57090 bytes uncompressed, 17179 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 fat     4009 b- defN 23-Apr-17 15:43 tsforecasting/tsf_model_selection.py
+-rw-rw-rw-  2.0 fat     7891 b- defN 23-Apr-17 15:44 tsforecasting/tsf_performance.py
+-rw-rw-rw-  2.0 fat     8381 b- defN 23-Apr-17 15:57 tsforecasting/tsf_predictions.py
+-rw-rw-rw-  2.0 fat     1078 b- defN 23-Apr-17 16:25 tsforecasting-1.2.60.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11282 b- defN 23-Apr-17 16:25 tsforecasting-1.2.60.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 16:25 tsforecasting-1.2.60.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-17 16:25 tsforecasting-1.2.60.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1047 b- defN 23-Apr-17 16:25 tsforecasting-1.2.60.dist-info/RECORD
+12 files, 56038 bytes uncompressed, 16853 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tsforecasting/tsf_performance.py
 Comment: 
 
 Filename: tsforecasting/tsf_predictions.py
 Comment: 
 
-Filename: tsforecasting-1.2.55.dist-info/LICENSE
+Filename: tsforecasting-1.2.60.dist-info/LICENSE
 Comment: 
 
-Filename: tsforecasting-1.2.55.dist-info/METADATA
+Filename: tsforecasting-1.2.60.dist-info/METADATA
 Comment: 
 
-Filename: tsforecasting-1.2.55.dist-info/WHEEL
+Filename: tsforecasting-1.2.60.dist-info/WHEEL
 Comment: 
 
-Filename: tsforecasting-1.2.55.dist-info/top_level.txt
+Filename: tsforecasting-1.2.60.dist-info/top_level.txt
 Comment: 
 
-Filename: tsforecasting-1.2.55.dist-info/RECORD
+Filename: tsforecasting-1.2.60.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tsforecasting/tsf_data_eng.py

```diff
@@ -4,72 +4,72 @@
 import datetime
 from datetime import timedelta
 from dateutil.relativedelta import relativedelta
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.feature_selection import SelectFromModel
 from sklearn.ensemble import RandomForestRegressor, ExtraTreesRegressor, GradientBoostingRegressor
 
-def slice_timestamp(Dataset:pd.DataFrame,date_col:str='Date'):
+def slice_timestamp(dataset:pd.DataFrame,date_col:str='Date'):
     """
     The slice_timestamp function takes a dataframe and returns the same dataframe with the date column sliced to just include
     the year, month, day and hour. This is done by converting all of the values in that column to strings then slicing them 
     accordingly. The function then converts those slices back into datetime objects so they can be used for further analysis.
     
-    :param Dataset:pd.DataFrame: Pass the dataset to be sliced
+    :param dataset:pd.DataFrame: Pass the dataset to be sliced
     :param date_col:str='Date': Specify the name of the column that contains the date information
     :return: A dataframe with the timestamp column sliced to only include the year, month and day
     """
-    df=Dataset.copy()
+    df=dataset.copy()
     cols=list(df.columns)
     for col in cols:
         if col==date_col:
             df[date_col] = df[date_col].astype(str)
             df[date_col] = df[date_col].str.slice(0,19)
             df[date_col] = pd.to_datetime(df[date_col])
     return df
 
-def round_cols(Dataset:pd.DataFrame,
+def round_cols(dataset:pd.DataFrame,
                target,round_:int=4):
     """
-    The round_cols function rounds the numeric columns of a Dataset to a specified number of decimal places.
+    The round_cols function rounds the numeric columns of a dataset to a specified number of decimal places.
     The function takes two arguments:
-    Dataset: A pandas DataFrame object.
+    dataset: A pandas DataFrame object.
     target: The name of the target column in the dataframe that will not be rounded.  This argument is required for safety reasons, so that no other columns are accidentally rounded.
     
-    :param Dataset:pd.DataFrame: Pass the dataframe that will be transformed
+    :param dataset:pd.DataFrame: Pass the dataframe that will be transformed
     :param target: Indicate the target variable
     :param round_:int=4: Round the numbers to a certain number of decimal places
     :return: A dataframe with the same columns as the original one, but with all numeric columns rounded to 4 decimals
     """
-    df_=Dataset.copy()
+    df_=dataset.copy()
     df_round=df_.copy()
     list_num_cols=df_round.select_dtypes(include=['float']).columns.tolist()
     
     for elemento in list_num_cols:
         if elemento==target:
             list_num_cols.remove(target)
     for col in list_num_cols:
         df_round[[col]]=df_round[[col]].round(round_)
         
     return df_round
 
-def engin_date(Dataset:pd.DataFrame,
-               Drop:bool=False):
+def engin_date(dataset:pd.DataFrame,
+               drop:bool=False):
     """
     The engin_date function takes a DataFrame and returns a DataFrame with the date features engineered.
     The function has two parameters: 
-    Dataset: A Pandas DataFrame containing at least one column of datetime data. 
-    Drop: A Boolean value indicating whether or not to drop the original datetime columns from the returned dataset.
+    dataset: A Pandas DataFrame containing at least one column of datetime data. 
+    drop: A Boolean value indicating whether or not to drop the original datetime columns from the returned dataset.
     
-    :param Dataset:pd.DataFrame: Pass the dataset
-    :param Drop:bool=False: Drop the original timestamp columns
+    :param dataset:pd.DataFrame: Pass the dataset
+    :param drop:bool=False: drop the original timestamp columns
     :return: The dataframe with the date features generated
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
 
@@ -98,47 +98,47 @@
         df.loc[(df[elemento + '_day_of_year'].isin(summer)), elemento + '_Season'] = '3'
         df.loc[(df[elemento + '_day_of_year'].isin(fall)), elemento + '_Season'] = '4'
         df.loc[(df[elemento + '_day_of_year'].isin(winter)), elemento + '_Season'] = '1'
         df[elemento + '_Season']=df[elemento + '_Season'].astype(np.int64)
         
         return df 
     
-    if Drop==True:
+    if drop==True:
         for elemento in list_date_columns:
             Df=create_date_features(Df,elemento)
             Df=Df.drop(elemento,axis=1)
-    elif Drop==False:
+    elif drop==False:
         for elemento in list_date_columns:
             Df=create_date_features(Df,elemento)
         
     return Df
 
-def multivariable_lag(Dataset:pd.DataFrame,
+def multivariable_lag(dataset:pd.DataFrame,
                       target:str="y",
                       range_lags:list=[1,10],
                       drop_na:bool=True):
     
     """
     The multivariable_lag function takes a Pandas DataFrame and returns a new DataFrame with the target variable 
     lagged by the number of periods specified in range_lags. The function also removes NaN values from the dataset, 
     and can be used to remove all NaN values or just those at the end of a time series. The default is to drop rows with any 
     NaNs, but this can be changed by setting drop_na=False.
     
-    :param Dataset:pd.DataFrame: Pass the dataset to be used in the function
+    :param dataset:pd.DataFrame: Pass the dataset to be used in the function
     :param target:str: Indicate the name of the column that will be used as target
     :param range_lags:list=[1: Define the range of lags to be used
     :param 10]: Indicate the maximum lag to be used
     :param drop_na:bool=True: Drop the rows with nan values
     :return: A dataframe with the lags specified by the user
     """
     
     assert range_lags[0]>=1, "Range lags first interval value should be bigger then 1"
     assert range_lags[0]<=range_lags[1], "Range lags first interval value should be bigger then second"
     
-    Df=Dataset.copy()
+    Df=dataset.copy()
     Df_=Df.copy()
     Df_=slice_timestamp(Df_)
     
     lag_str,list_dfs='',[]
 
     for elemento in range(range_lags[0],range_lags[1]+1):
         lag_str=str(elemento)
@@ -158,41 +158,41 @@
     for col in cols:
         if col=='Date':
             Df_=Df_.set_index(['Date']) 
             break
         
     return Df_
 
-def feature_selection_tb(Dataset:pd.DataFrame,
+def feature_selection_tb(dataset:pd.DataFrame,
                          target:str="y",
                          total_vi:float=0.99,
                          algo:str="ExtraTrees",
                          estimators:int=250):
     """
     The feature_selection_tb function takes in a pandas dataframe and returns the selected columns.
     The function uses ExtraTreesRegressor to select the most important features from a dataset. 
     The user can specify how much of the total variance they want explained by their model, as well as what algorithm they would like to use for feature selection.
     
-    :param Dataset:pd.DataFrame: Pass the dataset
+    :param dataset:pd.DataFrame: Pass the dataset
     :param target:str=&quot;y&quot;: Specify the target variable name
     :param total_vi:float=0.99: Set the total variable importance that needs to be achieved
     :param algo:str=&quot;ExtraTrees&quot;: Select the algorithm to be used for feature selection
     :param estimators:int=250: Set the number of estimators in the randomforest and extratrees algorithms
     :return: A list of columns that are selected by the algorithm
     """
     assert total_vi>=0.5 and total_vi<=1 , "total_vi value should be in [0.5,1[ interval"
     
-    Train=Dataset.copy()
-    sel_cols= list(Train.columns)
+    train=dataset.copy()
+    sel_cols= list(train.columns)
     sel_cols.remove(target)
     sel_cols.append(target)
-    Train=Train[sel_cols]
+    train=train[sel_cols]
    
-    X_train = Train.iloc[:, 0:(len(sel_cols)-1)].values
-    y_train = Train.iloc[:, (len(sel_cols)-1)].values
+    X_train = train.iloc[:, 0:(len(sel_cols)-1)].values
+    y_train = train.iloc[:, (len(sel_cols)-1)].values
     
     if algo=='ExtraTrees':
         fs_model = ExtraTreesRegressor(n_estimators=estimators)
         fs_model.fit(X_train, y_train)
     elif algo=="RandomForest":
         fs_model = RandomForestRegressor(n_estimators=estimators)
         fs_model.fit(X_train, y_train)
@@ -200,18 +200,18 @@
         fs_model = GradientBoostingRegressor(n_estimators=estimators)
         fs_model.fit(X_train, y_train)
 
     column_imp=fs_model.feature_importances_
     column_names=sel_cols.copy()
     column_names.remove(target)
     
-    Feat_imp = pd.Series(column_imp)
+    feat_imp = pd.Series(column_imp)
     Columns = pd.Series(column_names)
     
-    df=pd.concat([Feat_imp,Columns],axis=1)
+    df=pd.concat([feat_imp,Columns],axis=1)
     df = df.rename(columns={0: 'percentage',1: 'variable'})
     
     n=0.015
     va_df = df[df['percentage'] > n]
     var_importance=va_df['percentage'].sum()
     for iteration in range(0,10):
```

## tsforecasting/tsf_expanding_window.py

```diff
@@ -7,86 +7,86 @@
 from pmdarima.arima import auto_arima
 from .tsf_model_selection import model_prediction
 from .tsf_data_eng import slice_timestamp, engin_date, multivariable_lag
 from .tsf_model_configs import model_configurations
 
 h_parameters=model_configurations()
 
-def Univariate_Forecast(Dataset:pd.DataFrame,
+def Univariate_Forecast(dataset:pd.DataFrame,
                         train_length:float,
                         forecast_length:int,
                         rolling_window_size:int,
                         algo:str,
                         model_configs:dict=h_parameters,
                         granularity:str="1d"):
     """
     The Univariate_Forecast function takes a dataset and makes a forecast for the target variable.
     The function returns a dataframe with the predictions of the target variable.
-    Parameters: Dataset, train_length, forecast_length, rolling_window_size, algo (Prophet or AutoArima), model configs (dict) and granularity(int). 
+    Parameters: dataset, train_length, forecast_length, rolling_window_size, algo (Prophet or AutoArima), model configs (dict) and granularity(int). 
     
-    :param Dataset:pd.DataFrame: Pass the dataset to be used for forecasting
+    :param dataset:pd.DataFrame: Pass the dataset to be used for forecasting
     :param train_length:float: Specify the percentage of data to be used as train
     :param forecast_length:int: Indicate the number of periods to forecast
     :param rolling_window_size:int: Define the size of the window used to evaluate the performance of each algorithm
     :param algo:str: Select the forecasting algorithm to be used
     :param model_configs:dict: Configure the models
     :param granularity:str=&quot;1m&quot;: Set the granularity of the time series
     :return: A dataframe with the predictions
     """
     dfs_list,list_y_true,list_y_pred=[],[],[]
     
     target='y'
     
-    Dataset=slice_timestamp(Dataset)
-    Dataframe=Dataset.copy()
-    Dataframe=Dataframe.iloc[forecast_length*3:,:]  ## Equal data lenght to Multivariate Approach given the rows drop in multivariate lags*  
+    dataset=slice_timestamp(dataset)
+    dataset_=dataset.copy()
+    dataset_=dataset_.iloc[forecast_length*3:,:]  ## Equal data lenght to Multivariate Approach given the rows drop in multivariate lags*  
     
-    df_final = Dataframe[['Date', target]]
+    df_final = dataset_[['Date', target]]
     df_final = df_final.rename(columns={'Date': 'ds'}) 
     
-    size_Train=int((train_length*len(df_final)))
+    size_train=int((train_length*len(df_final)))
     
-    Train=df_final.iloc[:size_Train,:]
-    Test=df_final.iloc[size_Train:,:]
+    train=df_final.iloc[:size_train,:]
+    test=df_final.iloc[size_train:,:]
     
-    Train[target]=Train[target].astype(np.int64)
-    Test[target]=Test[target].astype(np.int64)
+    train[target]=train[target].astype(np.int64)
+    test[target]=test[target].astype(np.int64)
     
-    assert len(Test)>=forecast_length , "forecast_length>=len(Test), try to reduce your train_size ratio"
+    assert len(test)>=forecast_length , "forecast_length>=len(Test), try to reduce your train_size ratio"
     
-    iterations,iters = (int((len(Test))/rolling_window_size)),(int((len(Test)-forecast_length)/rolling_window_size))+1
+    iterations,iters = (int((len(test))/rolling_window_size)),(int((len(test)-forecast_length)/rolling_window_size))+1
     
     if algo=='AutoArima':
     
         aa_params=model_configs['AutoArima']
-        model_arima=auto_arima(Train[[target]], **aa_params)
+        model_arima=auto_arima(train[[target]], **aa_params)
     
     for rolling_cycle in range(0, iterations):
         
         if rolling_cycle==0:
             window=0
         else:
             window=rolling_window_size
         
-        size_Train=size_Train+window
+        size_train=size_train+window
         
-        Train=df_final.iloc[:size_Train,:]
-        Test=df_final.iloc[size_Train:,:]
+        train=df_final.iloc[:size_train,:]
+        test=df_final.iloc[size_train:,:]
         
-        if len(Test[target])>=forecast_length:
+        if len(test[target])>=forecast_length:
             
             print('Algorithm Evaluation:', algo,'|| Window Iteration:', rolling_cycle + 1, "of", iters)
             
-            print('Rows Train:', len(Train))
+            print('Rows Train:', len(train))
             
-            print('Rows Test:', len(Test))
+            print('Rows Test:', len(test))
 
-            Train[[target]]=Train[[target]].astype('int32')
+            train[[target]]=train[[target]].astype('int32')
             
-            train_=Train.copy()
+            train_=train.copy()
             train_=train_[['ds', target]]
             
             if granularity=="1m":
                 frequency='min'
             elif granularity=="30m":
                 frequency='30min'
             elif granularity=="1h":
@@ -110,140 +110,140 @@
                 y_pred=forecast.iloc[len(forecast)-forecast_length:,:]
 
             elif algo=='AutoArima':
                 
                 model_arima.fit(train_[[target]])
             
                 forecast = model_arima.predict(n_periods=forecast_length)
-                y_pred=pd.DataFrame(forecast, columns = [0]) #y_pred=forecast.to_frame()
+                y_pred=pd.DataFrame(forecast, columns = [0]) 
                 col=0
                 
             y_pred=y_pred[col]
                         
-            y_true=Test[target][0:forecast_length]
+            y_true=test[target][0:forecast_length]
             
             y_pred_list = y_pred.tolist()
             y_true_list = y_true.tolist()
 
             list_y_true.append(y_true)
             list_y_pred.append(y_pred)
             x,y=pd.concat(list_y_true),pd.concat(list_y_pred) 
             x,y=x.reset_index(drop=True),y.reset_index(drop=True)
             df = pd.DataFrame()
             df = pd.DataFrame({'y_true': x,'y_pred': y,'Window':rolling_cycle})
             df_=df.iloc[len(df)-forecast_length:,:]
             
-            df_.index=Test['ds'][0:forecast_length]
+            df_.index=test['ds'][0:forecast_length]
             dfs_list.append(df_)
 
     df_pred=pd.concat(dfs_list)
     df_pred['Window']=df_pred['Window']+1
 
     return df_pred
 
 
-def Multivariate_Forecast(Dataset:pd.DataFrame,
+def Multivariate_Forecast(dataset:pd.DataFrame,
                           train_length:float,
                           forecast_length:int,
                           rolling_window_size:int,
                           algo:str,
                           model_configs:dict=h_parameters,
                           granularity:str='1d'):
     """
     The Multivariate_Forecast function takes a dataset, the length of the train period, 
     the forecast length and a rolling window size as input. It then splits the data into train and test sets. 
     It then applies an algorithm to predict future values based on past patterns in the data. The function returns 
     a DataFrame with actual values (y_true) and predicted values (y_pred). 
     
-    :param Dataset:pd.DataFrame: Pass the dataset to be used in the model
+    :param dataset:pd.DataFrame: Pass the dataset to be used in the model
     :param train_length:float: Define the length of the train dataset
     :param forecast_length:int: Define the number of periods to forecast
     :param rolling_window_size:int: Define the size of the window that will be used to split the dataset
     :param algo:str: Select the algorithm to be used for training and forecasting
     :param model_configs:dict: Configure the model
     :param granularity:str='1m': Define the time interval of the data
     :return: A dataframe with the predicted values and the window number
     """
     assert train_length>=0.3 and train_length<=1 , "train_length value should be in [0.3,1[ interval"
 
     dfs_list,list_y_true,list_y_pred=[],[],[]
     
     target='y'   
     
-    Df=Dataset.copy()
-    Df=slice_timestamp(Df)
+    dataset_=dataset.copy()
+    dataset_=slice_timestamp(dataset_)
     
-    Df=engin_date(Df)
+    dataset_=engin_date(dataset_)
 
-    Df = multivariable_lag(Df,target,range_lags=[forecast_length,forecast_length*3])
+    dataset_ = multivariable_lag(dataset_,target,range_lags=[forecast_length,forecast_length*3])
 
-    df_final = Df.copy()
+    df_final = dataset_.copy()
     
-    size_Train=int((train_length*len(df_final)))
+    size_train=int((train_length*len(df_final)))
 
-    Train=df_final.iloc[:size_Train,:]
-    Test=df_final.iloc[size_Train:,:]
+    train=df_final.iloc[:size_train,:]
+    test=df_final.iloc[size_train:,:]
     
-    Train[target]=Train[target].astype(np.int64)
-    Test[target]=Test[target].astype(np.int64)    
+    train[target]=train[target].astype(np.int64)
+    test[target]=test[target].astype(np.int64)    
     
-    assert len(Test)>=forecast_length , "forecast_length>=len(Test), try to reduce your train_size ratio"
+    assert len(test)>=forecast_length , "forecast_length>=len(Test), try to reduce your train_size ratio"
     
-    iterations,iters = (int((len(Test))/rolling_window_size)),(int((len(Test)-forecast_length)/rolling_window_size))+1
+    iterations,iters = (int((len(test))/rolling_window_size)),(int((len(test)-forecast_length)/rolling_window_size))+1
       
     for rolling_cycle in range(0, iterations):
             
         if rolling_cycle==0:
             window=0
         else:
             window=rolling_window_size
         
-        size_Train=size_Train+window
+        size_train=size_train+window
         
-        Train=df_final.iloc[:size_Train,:]
-        Test=df_final.iloc[size_Train:,:]
+        train=df_final.iloc[:size_train,:]
+        test=df_final.iloc[size_train:,:]
         
-        if (len(Test[target])>=forecast_length):
+        if (len(test[target])>=forecast_length):
             
             print('Algorithm Evaluation:', algo,'|| Window Iteration:', rolling_cycle + 1, "of", iters)
             
-            print('Rows Train:', len(Train))
+            print('Rows Train:', len(train))
             
-            print('Rows Test:', len(Test))
+            print('Rows Test:', len(test))
             
-            Train[[target]]=Train[[target]].astype('int32')
+            train[[target]]=train[[target]].astype('int32')
             
-            input_cols=list(Train.columns)
+            input_cols=list(train.columns)
             input_cols.remove(target)
 
             scaler = MinMaxScaler() 
 
-            scaler = scaler.fit(Train[input_cols])
-            Train[input_cols] = scaler.transform(Train[input_cols])
-            Test[input_cols] = scaler.transform(Test[input_cols])            
+            scaler = scaler.fit(train[input_cols])
+            train[input_cols] = scaler.transform(train[input_cols])
+            test[input_cols] = scaler.transform(test[input_cols])            
 
-            y_pred=model_prediction(Train, Test,target,model_configs=model_configs,algo=algo)
+            y_pred=model_prediction(train, test,target,model_configs=model_configs,algo=algo)
             y_pred=y_pred[0:forecast_length]
             y_pred= pd.Series(y_pred.tolist())
             y_pred_list = y_pred.tolist()
             
-            y_true=Test[target][0:forecast_length]
+            y_true=test[target][0:forecast_length]
             y_true = pd.Series(y_true)
             y_true_list = y_true.tolist()
             
-            y_t_axys=list(Test.index[0:forecast_length])
+            y_t_axys=list(test.index[0:forecast_length])
             
             list_y_true.append(y_true)
             list_y_pred.append(y_pred)
             x,y=pd.concat(list_y_true),pd.concat(list_y_pred) 
             x,y=x.reset_index(drop=True),y.reset_index(drop=True)
             df = pd.DataFrame()
             df = pd.DataFrame({'y_true': x,'y_pred': y,'Window':rolling_cycle})
             df_=df.iloc[len(df)-forecast_length:,:]
-            df_.index=Test.index[0:forecast_length]
+            df_.index=test.index[0:forecast_length]
 
             dfs_list.append(df_)
 
     df_pred=pd.concat(dfs_list)
 
     df_pred['Window'] = df_pred['Window']+1
     df_pred['y_pred'] = df_pred['y_pred'].astype(str)
```

## tsforecasting/tsf_model_selection.py

```diff
@@ -8,41 +8,41 @@
 import xgboost
 import h2o
 from h2o.automl import H2OAutoML
 from .tsf_model_configs import model_configurations
 
 h_parameters=model_configurations()
 
-def model_prediction(Train:pd.DataFrame,
-                     Test:pd.DataFrame,
+def model_prediction(train:pd.DataFrame,
+                     test:pd.DataFrame,
                      target:str="y",
                      model_configs:dict=h_parameters,
                      algo:str='RandomForest'):
     """
-    The model_prediction function takes in a Train and Test dataframe, as well as the name of the target column. 
+    The model_prediction function takes in a train and test dataframe, as well as the name of the target column. 
     It then trains a model using the specified algorithm (RandomForest by default) and returns predictions for 
     the test set.
     
-    :param Train:pd.DataFrame: Pass the train dataframe
-    :param Test:pd.DataFrame: Test the model with a different dataset
+    :param train:pd.DataFrame: Pass the train dataframe
+    :param test:pd.DataFrame: test the model with a different dataset
     :param target:str: Specify the column name of the target variable
     :param model_configs:dict: Pass the parameters of each model
     :param algo:str='RandomForest': Select the model to be used
     :return: The predictions of the model
     """
-    sel_cols= list(Train.columns)
+    sel_cols= list(train.columns)
     sel_cols.remove(target)
     sel_cols.append(target) 
-    Train=Train[sel_cols]
-    Test=Test[sel_cols]   
+    train=train[sel_cols]
+    test=test[sel_cols]   
     
-    X_train = Train.iloc[:, 0:(len(sel_cols)-1)].values
-    X_test = Test.iloc[:, 0:(len(sel_cols)-1)].values
-    y_train = Train.iloc[:, (len(sel_cols)-1)].values
-    y_test = Test.iloc[:, (len(sel_cols)-1)].values
+    X_train = train.iloc[:, 0:(len(sel_cols)-1)].values
+    X_test = test.iloc[:, 0:(len(sel_cols)-1)].values
+    y_train = train.iloc[:, (len(sel_cols)-1)].values
+    y_test = test.iloc[:, (len(sel_cols)-1)].values
     
     if algo=='RandomForest':
         rf_params=model_configs['RandomForest']
         regressor_RF = RandomForestRegressor(**rf_params) 
         regressor_RF.fit(X_train, y_train)
         y_predict = regressor_RF.predict(X_test)
         
@@ -67,29 +67,29 @@
     elif algo=='GeneralizedLR':
         td_params=model_configs['GeneralizedLR']
         regressor_TD = TweedieRegressor(**td_params)
         regressor_TD.fit(X_train, y_train)
         y_predict = regressor_TD.predict(X_test)
         
     elif algo=='H2O_AutoML':
-        Test[target]=Test[target].fillna(0) ## Avoid H2O OS_Error
-        Test[target]=Test[target].astype(float) ## Avoid H2O OS_Error
-        Train_h2o,Test_h2o=h2o.H2OFrame(Train),h2o.H2OFrame(Test)
+        test[target]=test[target].fillna(0) ## Avoid H2O OS_Error
+        test[target]=test[target].astype(float) ## Avoid H2O OS_Error
+        train_h2o,test_h2o=h2o.H2OFrame(train),h2o.H2OFrame(test)
         input_cols=sel_cols.copy()
         input_cols.remove("y")
         aml_params=model_configs['H2O_AutoML']
         aml = H2OAutoML(**aml_params) 
-        aml.train(x=input_cols ,y=target ,training_frame=Train_h2o)
+        aml.train(x=input_cols ,y=target ,training_frame=train_h2o)
         
         leaderboards = aml.leaderboard
         leaderboard_df= leaderboards.as_data_frame()
         id_leader_model=leaderboard_df['model_id'][0]
         h2o_leader_model=h2o.get_model(id_leader_model)
         
-        pred_col = h2o_leader_model.predict(Test_h2o)
+        pred_col = h2o_leader_model.predict(test_h2o)
         pred_col = pred_col.asnumeric()
         y_predict= pred_col.as_data_frame()['predict']
         
     elif algo=='XGBoost':
         xg_params=model_configs['XGBoost']
         regressor_XG = xgboost.XGBRegressor(**xg_params)
         regressor_XG.fit(X_train, y_train)
```

## tsforecasting/tsf_performance.py

```diff
@@ -27,25 +27,25 @@
                    'Mean Absolute Percentage Error': mape,
                    'Mean Squared Error': mse,
                    'Explained Variance Score': evs, 
                    'Max Error': maximo_error}
     
     return metrics_reg
 
-def vertical_univariated_performance(Dataset:pd.DataFrame,
+def vertical_univariated_performance(dataset:pd.DataFrame,
                                      forecast_length:int):
     """
     The vertical_univariated_performance function takes a dataframe and the forecast length as inputs.
     It returns a dataframe with the metrics for each step ahead, for all steps in the forecast_length.
     
-    :param Dataset:pd.DataFrame: Pass the dataset that will be used to calculate the performance metrics
+    :param dataset:pd.DataFrame: Pass the dataset that will be used to calculate the performance metrics
     :param forecast_length:int: Indicate the number of steps ahead that we want to forecast
     :return: A dataframe with the metrics of performance for each step ahead
     """
-    df_=Dataset.copy()
+    df_=dataset.copy()
 
     target="y"
     ahead_forecast_list,steps_list,list_dfs=list(range(1,forecast_length+1)),(list(dict.fromkeys(df_['Window'].tolist()))),[]
 
     for elemento_step in steps_list:
         df_filter=df_[df_['Window']==elemento_step]
         df_filter['V_Window']=ahead_forecast_list
@@ -60,66 +60,66 @@
         vertical_metrics[['Forecast_Length']]=element
         list_metrics.append(vertical_metrics)
 
     total_vertical_metrics = pd.concat(list_metrics)
 
     return total_vertical_metrics
 
-def select_best_model(Dataset:pd.DataFrame,
+def select_best_model(dataset:pd.DataFrame,
                       eval_metric:str='MAE'): #'Mean Absolute Percentage Error','Mean Squared Error','Max Error'
     """
-    The select_best_model function takes a Dataset containing the results of 
+    The select_best_model function takes a dataset containing the results of 
     several models and returns the best model based on an evaluation metric.
     
     
-    :param Dataset:pd.DataFrame: Pass the dataframe to be evaluated
+    :param dataset:pd.DataFrame: Pass the dataframe to be evaluated
     :param eval_metric:str='MAE': Select the evaluation metric to be used in the function
     :return: The best model (the one with the lowest mean absolute error)
     """ 
-    df=Dataset.copy()
+    df=dataset.copy()
     model_perf = {}
     
     if eval_metric == "MAE":
         eval_metric_='Mean Absolute Error'
     elif eval_metric == "MAPE":
         eval_metric_='Mean Absolute Percentage Error'
     elif eval_metric == "MSE":
         eval_metric_='Mean Squared Error'
     
-    list_models=(list(dict.fromkeys(Dataset['Model'].tolist())))
+    list_models=(list(dict.fromkeys(dataset['Model'].tolist())))
 
     for model in list_models:
         
-        df=Dataset.copy()
+        df=dataset.copy()
         df=df.loc[df['Model'] == model]
         metric_model=round(df[eval_metric_].mean(),4)
         
         model_perf[model] = metric_model
     print("Models Predictive Performance:", model_perf)
     best_model=min(model_perf, key=model_perf.get)
     perf_metric=model_perf[best_model]
     if len(list_models)>1:
         print("The model with best performance was", best_model, "with an (mean)", 
               eval_metric_, "of", perf_metric )
     return best_model
 
-def pred_performance(Dataset:pd.DataFrame,
+def pred_performance(dataset:pd.DataFrame,
                      train_size:float,
                      forecast_size:int,
                      window_size:int,
                      list_models:list,
                      model_configs:dict=h_parameters,
                      granularity:str="1d",
                      eval_metric:str="MAE"):
     """
     The pred_performance function takes as input a dataframe, list of models and model configurations.
     It returns the best model based on the evaluation metric specified by the user (default is MAEs), 
     the performance metrics for all models, and predictions for each model.
     
-    :param Dataset:pd.DataFrame: Pass the dataset to be used for forecasting
+    :param dataset:pd.DataFrame: Pass the dataset to be used for forecasting
     :param list_models:list: Specify the list of models that will be used for the prediction
     :param model_configs:dict: Pass the parameters of the model that is going to be used
     :param train_size:float: Define the size of the training set
     :param forecast_size:int: Define the forecast horizon
     :param window_size:int: Define the size of the rolling window used to train and predict
     :param granularity:str: Specify the time series granularity
     :param eval_metric:str=&quot;MAE&quot;: Select the best model based on the selected eval_metric
@@ -130,29 +130,29 @@
     list_mv=['RandomForest','ExtraTrees','GBR','KNN','GeneralizedLR','XGBoost','H2O_AutoML']
     list_uv=['Prophet','AutoArima']
     
     for elemento in list_models:
     
         if elemento in list_mv:
 
-            results=Multivariate_Forecast(Dataset,
+            results=Multivariate_Forecast(dataset,
                                           train_length=train_size,
                                           forecast_length=forecast_size,
                                           rolling_window_size=window_size,
                                           algo=elemento,
                                           model_configs=model_configs,
                                           granularity=granularity)
             pred_perfomance=vertical_univariated_performance(results,forecast_size)
             pred_perfomance['Model']=elemento
             pred_dfs.append(pred_perfomance)
             results['Model']=elemento
             pred_values.append(results)
         
         if elemento in list_uv:
-            results=Univariate_Forecast(Dataset,
+            results=Univariate_Forecast(dataset,
                                         train_length=train_size,
                                         forecast_length=forecast_size,
                                         rolling_window_size=window_size,
                                         algo=elemento,
                                         model_configs=model_configs,
                                         granularity=granularity)
             pred_perfomance=vertical_univariated_performance(results,forecast_size)
```

## tsforecasting/tsf_predictions.py

```diff
@@ -9,32 +9,32 @@
 from pmdarima.arima import auto_arima
 from .tsf_data_eng import slice_timestamp, round_cols, engin_date, multivariable_lag
 from .tsf_model_selection import model_prediction
 from .tsf_model_configs import model_configurations
 
 h_parameters=model_configurations()
 
-def pred_dataset(Dataset:pd.DataFrame,
+def pred_dataset(dataset:pd.DataFrame,
                  forecast_size:int,
                  granularity:str='1d'):
     """
     The pred_dataset function takes a dataset and returns a dataframe with the timestamp column 
     extended to include the next forecast_size number of rows. The granularity parameter determines 
     how far apart each row is timewise. For example, if granularity='30m' then each new row will be 30 minutes 
     apart from the previous row.
     
-    :param Dataset:pd.DataFrame: Pass the dataset that is to be used for forecasting
+    :param dataset:pd.DataFrame: Pass the dataset that is to be used for forecasting
     :param forecast_size:int: Specify the number of rows in the forecast dataset
     :param granularity:str='1d': Specify the frequency of the time series
     :return: A dataframe with the timestamp of the last row of our dataset, and a number of rows equal to forecast_size
     """
-    Dataframe=Dataset.copy()
-    Dataframe=slice_timestamp(Dataframe)
+    dataset_=dataset.copy()
+    dataset_=slice_timestamp(dataset_)
 
-    timestamp,timestamp_list=list((Dataframe.Date[len(Dataframe)-1:]))[0],[]
+    timestamp,timestamp_list=list((dataset_.Date[len(dataset_)-1:]))[0],[]
     
     if granularity=='1m':
     
         def generate_datetimes(date_from_str=timestamp, days=1000):
            date_from = datetime.datetime.strptime(str(date_from_str), '%Y-%m-%d %H:%M:%S')
            for n in range(1,1420*days):
                yield date_from + datetime.timedelta(minutes=n)
@@ -90,46 +90,46 @@
     df['Date']=timestamp_list
     df['Date']=pd.to_datetime(df['Date'])
     
     df=df.iloc[0:forecast_size,:]
     
     return df
 
-def pred_results(Dataset:pd.DataFrame,
+def pred_results(dataset:pd.DataFrame,
                  forecast_size:int,
                  model_configs:dict=h_parameters,
                  granularity:str='1d',
                  selected_model:str='RandomForest'):
     """
     The pred_results function takes in a dataset, the name of the model to be used for prediction, 
     the forecast size and a dictionary containing all parameters needed to run the selected model.
     The function returns a dataframe with real values and predicted values from the specified model.
     
-    :param Dataset:pd.DataFrame: Pass the dataset to be used for prediction
+    :param dataset:pd.DataFrame: Pass the dataset to be used for prediction
     :param selected_model:str: Select the model that will be used for the prediction
     :param forecast_size:int: Define the number of periods to forecast
     :param model_configs:dict: Pass the parameters of the model
     :param granularity:str: Define the time interval of the data
     :return: A dataframe with the predicted values
     """
-    Dataset=slice_timestamp(Dataset)
-    df_pred=pred_dataset(Dataset,forecast_size,granularity)
-    Dataset["Values"]=0
+    dataset=slice_timestamp(dataset)
+    df_pred=pred_dataset(dataset,forecast_size,granularity)
+    dataset["Values"]=0
     df_pred["Values"]=1
-    df_final= pd.concat([Dataset,df_pred])
+    df_final= pd.concat([dataset,df_pred])
     df_final.index=df_final['Date']
     
     list_mv=['RandomForest','ExtraTrees','GBR','KNN','GeneralizedLR','XGBoost','H2O_AutoML']
     list_uv=['Prophet','AutoArima']
     
     target='y'
 
     if selected_model in list_uv:
         
-        df=Dataset.copy()
+        df=dataset.copy()
         df = df.rename(columns={'Date': 'ds'})
         df = df[['ds', target]]
         
         if granularity=="1m":
             frequency='min'
         elif granularity=="30m":
             frequency='30min'
@@ -164,36 +164,36 @@
         df_final['y'][len(df_final)-forecast_size:]=y_pred
         df_final['Values']=df_final['Values'].replace(0,'Real')
         df_final['Values']=df_final['Values'].replace(1,'Predicted')
         df_final=round_cols(df_final, target)
 
     elif selected_model in list_mv:
 
-        df_final=engin_date(df_final,Drop=False)
+        df_final=engin_date(df_final,drop=False)
         df_final=multivariable_lag(df_final,target,range_lags=[forecast_size,forecast_size*3]) 
         
-        Train=df_final.iloc[:len(df_final)-forecast_size,:]
-        Test=df_final.iloc[len(df_final)-forecast_size:,:]
+        train=df_final.iloc[:len(df_final)-forecast_size,:]
+        test=df_final.iloc[len(df_final)-forecast_size:,:]
 
         input_cols=list(df_final.columns)
         input_cols.remove(target)  
         
         scaler = MinMaxScaler()
-        scaler = scaler.fit(Train[input_cols])
+        scaler = scaler.fit(train[input_cols])
         
-        Train[input_cols] = scaler.transform(Train[input_cols])
-        Test[input_cols] = scaler.transform(Test[input_cols])
+        train[input_cols] = scaler.transform(train[input_cols])
+        test[input_cols] = scaler.transform(test[input_cols])
 
-        y_pred=model_prediction(Train, Test,target,model_configs=model_configs,algo=selected_model)
+        y_pred=model_prediction(train, test,target,model_configs=model_configs,algo=selected_model)
         df_final['y'][len(df_final)-forecast_size:]=y_pred
         df_final['Values']=df_final['Values'].replace(0,'Real')
         df_final['Values']=df_final['Values'].replace(1,'Predicted')
         df_final['Date']=df_final.index
         df_final=df_final[['Date','y','Values']]
-        df_=Dataset.head(forecast_size*3)
+        df_=dataset.head(forecast_size*3)
         df_.index=df_.Date
         df_['Values']='Real'
 
         df_final = pd.concat([df_,df_final])
         df_final = df_final.reset_index(drop=True)
         
     return df_final
```

## Comparing `tsforecasting-1.2.55.dist-info/LICENSE` & `tsforecasting-1.2.60.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tsforecasting-1.2.55.dist-info/METADATA` & `tsforecasting-1.2.60.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tsforecasting
-Version: 1.2.55
-Summary: TSForecasting is an automated time series forecasting framework
+Version: 1.2.60
+Summary: TSForecasting is an Automated Time Series Forecasting Framework
 Home-page: https://github.com/TsLu1s/TSForecasting
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,time series forecasting,automated time series,multivariate time series,univariate time series,automated machine learning,automl
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
@@ -92,15 +92,15 @@
     
 ## 1. TSForecasting - Automated Time Series Forecasting
     
 The first needed step after importing the package is to load a dataset and define your DataTime and to be predicted Target column and rename them to 'Date' and 'y', respectively.
 The following step is to define your future running pipeline parameters variables, this being:
 * train_size: Length of Train data in which will be applied the first Expanding Window iteration;  
 * forecast_size: Full length of test/future ahead predictions;
-* window_size: Length of sliding window, Window_Size>=Forecast_Size is recommended;
+* window_size: Length of sliding window, window_size>=forecast_size is suggested;
 * granularity: Valid interval of periods correlated to data -> 1m,30m,1h,1d,1wk,1mo (default='1d');
 * eval_metric: Default predictive evaluation metric (eval_metric) is "MAE" (Mean Absolute Error), other options are "MAPE" (Mean Absolute Percentage Error) and "MSE"
 (Mean Squared Error);
 * list_models: Select all the models intented do run in `pred_performance` function. To compare predictive performance of all available models set paramater `list_models`=['RandomForest','ExtraTrees','GBR',
 'KNN','GeneralizedLR','XGBoost','H2O_AutoML','AutoArima','Prophet'];
 * model_configs: Nested dictionary in which are contained all models and specific hyperparameters configurations. Feel free to customize each model as you see fit (customization example shown bellow); 
  
@@ -126,102 +126,78 @@
 data = pd.read_csv('csv_directory_path') # Dataframe Loading Example
     
 data = data.rename(columns={'DateTime_Column': 'Date','Target_Name_Column':'y'})
 data=data[['Date',"y"]]
     
 train_size_=0.95
 forecast_size_=15
-window_size_=Forecast_Size # Recommended
+window_size_=forecast_size_ # Recommended
 granularity_='1d' # 1m,30m,1h,1d,1wk,1mo
 eval_metric_="MAE" # MAPE, MSE
 list_models_=['RandomForest','ExtraTrees','KNN','XGBoost','AutoArima'] # Ensemble Example
     
 ## Get models hyperparameters configurations
     
 models_hparameters=tsf.model_configurations()
 print(models_hparameters)
 
 # Customization Example
 models_hparameters["RandomForest"]["n_estimators"]=100
 models_hparameters["ExtraTrees"]["n_estimators"]=100
 
 ## Performance Evaluation
-best_model,perf_results,predictions=tsf.pred_performance(Dataset=data,
+best_model,perf_results,predictions=tsf.pred_performance(dataset=data,
                                                          train_size=train_size_,
                                                          forecast_size=forecast_size_,
                                                          window_size=window_size_,
                                                          list_models=list_models_,
                                                          model_configs=models_hparameters,
                                                          granularity=granularity_,
                                                          eval_metric=eval_metric_)
 ## Forecast
-dataset_pred=tsf.pred_results(Dataset=data,
+dataset_pred=tsf.pred_results(dataset=data,
                               forecast_size=forecast_size_,
                               model_configs=models_hparameters,
                               granularity=granularity_,
                               selected_model=best_model)
 ```  
 
 ## 2. TSForecasting - Extra Auxiliar Functions
-
-The `model_prediction` function predicts your Test target column based on the input DataFrames, Train and Test, model configuration set by the parameter `model_configs` and the selected running algorithm in the parameter `algo` (default='RandomForest'). Note, you can select and customize any of the 11 models available in `Model_Configs` dictionary.
-    
-```py     
- 
-# Automated Model Predictions
- 
-y_predict = tsf.model_prediction(Train:pd.DataFrame,
-                                 Test:pd.DataFrame,
-                                 target:str="y",
-                                 model_configs:dict=models_hparameters,
-                                 algo:str='RandomForest')
-```       
-    
     
 The `engin_date` function converts and transforms columns of Datetime type into additional columns (Year, Day of the  Year, Season, Month, Day of the month, Day of the week, Weekend, Hour, Minute) which will be added by association to the input dataset and subsequently deletes the original column if variable Drop=True.
 
 The `multivariable_lag` function creats all the past lags automatically (in accordance to `range_lags` parameter) and adds each column into the input DataFrame.
  
 ```py   
 
 # Feature Engineering 
     
-dataset = tsf.engin_date(Dataset:pd.DataFrame,
-                         Drop:bool=False) 
+dataset = tsf.engin_date(dataset:pd.DataFrame,
+                         drop:bool=False) 
 
-dataset = tsf.multivariable_lag(Dataset:pd.DataFrame,
+dataset = tsf.multivariable_lag(dataset:pd.DataFrame,
                                 target:str="y",
                                 range_lags:list=[1,10],
                                 drop_na:bool=True)
     
 ```
 
 This `feature_selection_tb` function filters the most valuable features from the dataset. It's based on calculated variable importance in tree based regression models from Scikit-Learn and it can be customized by use of the parameter `total_vi` (total sum of relative variable\feature importance percentage selected) and `algo` selecting the model for evaluation ('ExtraTrees','RandomForest' and 'GBR').
 
 ```py  
 
 # Feature Selection 
 
-selected_columns, selected_importance_df=tsf.feature_selection_tb(Dataset:pd.DataFrame,
+selected_columns, selected_importance_df=tsf.feature_selection_tb(dataset:pd.DataFrame,
                                                                   target:str="y",
                                                                   total_vi:float=0.99,
                                                                   algo:str="ExtraTrees",
                                                                   estimators:int=250)
  ```   
     
-You can analyse the obtained performance results by using the `metrics_regression` function wich contains the most used metrics for regression predictive contexts.
-    
-```py  
- 
-# Regression Performance Metrics
-
-reg_performance = pd.DataFrame(tsf.metrics_regression(y_true,y_pred),index=[0])    # y_true:list, y_pred:list
-        
-```
-
     
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/TsLu1s/TSForecasting/blob/main/LICENSE) for more information.
 
 ## Contact
```

## Comparing `tsforecasting-1.2.55.dist-info/RECORD` & `tsforecasting-1.2.60.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 tsforecasting/__init__.py,sha256=RIdya5qTwjBffBeeNTSBTSaeSGma5i4XGXmiFzswJQs,393
-tsforecasting/tsf_data_eng.py,sha256=1VOn_UrG-lX-9jVm4jwqRjg8kZEj1IfBZP94o9unMdE,10033
-tsforecasting/tsf_expanding_window.py,sha256=RkpvvNqLAuVUfSDVSAyMgevP6pTAwsK_emSJybQnfWQ,10117
+tsforecasting/tsf_data_eng.py,sha256=83glbKi5r3xLavkck2ssz5W1Pp1KyhQDhvfzAD_c_9Y,10033
+tsforecasting/tsf_expanding_window.py,sha256=9PyKRozW8AnWDC56Ry21SbCra4VO3WezUpctBXQ7DN8,10134
 tsforecasting/tsf_model_configs.py,sha256=vSsZuNQkmcrie_HEpsg1PCT565BPAUjlgj2w3IkhlD4,1684
-tsforecasting/tsf_model_selection.py,sha256=nTBV-FDqBI-1jexxkqGL9Dra3XwVCTTOCoCprrSZHmw,4009
-tsforecasting/tsf_performance.py,sha256=1Db8oUAjh7mhCfNftyzl8E8wg0hdVWJ8cnmnZPCNR44,7891
-tsforecasting/tsf_predictions.py,sha256=Ak8j-xh9FXe-DyqexsPeC9roQHa_HWUIqudwtR-aBJ8,8386
-tsforecasting-1.2.55.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
-tsforecasting-1.2.55.dist-info/METADATA,sha256=cL1eikx0zB8S-QOMYCUMVVKFDk3ohJrN6lHxiJYt_Mk,12346
-tsforecasting-1.2.55.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-tsforecasting-1.2.55.dist-info/top_level.txt,sha256=oKWWwpca0QkvqhgDcYBoVWqcFDLNSkSOuCvuEcZFABY,14
-tsforecasting-1.2.55.dist-info/RECORD,,
+tsforecasting/tsf_model_selection.py,sha256=3fI9tXKw5XA-YEn3cycOKQeLMj5Dq4ICNpJj8dEnmxQ,4009
+tsforecasting/tsf_performance.py,sha256=Wru_7VWLO1NDieeVm8AcA2P3Kd3yEhI8wz0yNUH6gQE,7891
+tsforecasting/tsf_predictions.py,sha256=cCml6sfvRhTKj7cyOj49EmcvT-THxEeSMFRSke34QYI,8381
+tsforecasting-1.2.60.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
+tsforecasting-1.2.60.dist-info/METADATA,sha256=FBf3a81KOgny8GGkVwT3adKzU0P5_jq9D87SmdKVEjA,11282
+tsforecasting-1.2.60.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+tsforecasting-1.2.60.dist-info/top_level.txt,sha256=oKWWwpca0QkvqhgDcYBoVWqcFDLNSkSOuCvuEcZFABY,14
+tsforecasting-1.2.60.dist-info/RECORD,,
```

