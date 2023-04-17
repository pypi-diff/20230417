# Comparing `tmp/veetility-0.1.8.tar.gz` & `tmp/veetility-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veetility-0.1.8.tar", last modified: Wed Jan 25 16:29:56 2023, max compression
+gzip compressed data, was "veetility-0.1.9.tar", last modified: Fri Jan 27 12:16:41 2023, max compression
```

## Comparing `veetility-0.1.8.tar` & `veetility-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-25 16:29:56.098833 veetility-0.1.8/
--rw-r--r--   0 willbutler   (502) staff       (20)      822 2023-01-25 16:29:56.098661 veetility-0.1.8/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      166 2023-01-04 11:21:38.000000 veetility-0.1.8/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-01-25 16:29:56.098886 veetility-0.1.8/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1424 2023-01-25 16:29:49.000000 veetility-0.1.8/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-25 16:29:56.097287 veetility-0.1.8/veetility/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-01-16 18:08:11.000000 veetility-0.1.8/veetility/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    32676 2023-01-25 16:26:30.000000 veetility-0.1.8/veetility/utility_functions.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-25 16:29:56.098440 veetility-0.1.8/veetility.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)      822 2023-01-25 16:29:55.000000 veetility-0.1.8/veetility.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      235 2023-01-25 16:29:56.000000 veetility-0.1.8/veetility.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-01-25 16:29:55.000000 veetility-0.1.8/veetility.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       90 2023-01-25 16:29:55.000000 veetility-0.1.8/veetility.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-01-25 16:29:56.000000 veetility-0.1.8/veetility.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-27 12:16:41.142082 veetility-0.1.9/
+-rw-r--r--   0 willbutler   (502) staff       (20)      822 2023-01-27 12:16:41.141929 veetility-0.1.9/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      166 2023-01-04 11:21:38.000000 veetility-0.1.9/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-01-27 12:16:41.142139 veetility-0.1.9/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1424 2023-01-27 12:16:27.000000 veetility-0.1.9/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-27 12:16:41.140419 veetility-0.1.9/veetility/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-01-16 18:08:11.000000 veetility-0.1.9/veetility/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    32811 2023-01-27 12:11:54.000000 veetility-0.1.9/veetility/utility_functions.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-01-27 12:16:41.141660 veetility-0.1.9/veetility.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)      822 2023-01-27 12:16:40.000000 veetility-0.1.9/veetility.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      235 2023-01-27 12:16:41.000000 veetility-0.1.9/veetility.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-01-27 12:16:40.000000 veetility-0.1.9/veetility.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       90 2023-01-27 12:16:41.000000 veetility-0.1.9/veetility.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-01-27 12:16:41.000000 veetility-0.1.9/veetility.egg-info/top_level.txt
```

### Comparing `veetility-0.1.8/PKG-INFO` & `veetility-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.8
+Version: 0.1.9
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.8/setup.py` & `veetility-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="veetility",
-    version="0.1.8",
+    version="0.1.9",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Vaynermedia",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `veetility-0.1.8/veetility/utility_functions.py` & `veetility-0.1.9/veetility/utility_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,28 @@
 
 file_handler = logging.FileHandler(f'./logs/UtilityFunctions.log')
 file_handler.setFormatter(formatter)
 logger.addHandler(file_handler)
 
 class UtilityFunctions():
 
-    def __init__(self, gspread_filepath=None,db_user=None,db_password=None,db_host=None,
+    def __init__(self, gspread_auth_dict=None,db_user=None,db_password=None,db_host=None,
                         db_port=None,db_name=None):
         """Initialise a gspread email account from reading from a json file contaning authorisation details
-            and provide login details for a postgreSQL table
-            This means you can only connect to one google account and one database per instance 
-            of the UtilityFunctions class
-            
-            Parameters 
-            -----------------
-            gspread_filepath : str
+        and provide login details for a postgreSQL table
+        This means you can only connect to one google account and one database per instance 
+        of the UtilityFunctions class
+        
+        Parameters 
+        -----------------
+        gspread_filepath : str
 
             """
-        if gspread_filepath != None:
-            self.sa = gspread.service_account(filename=gspread_filepath)              
+        if gspread_auth_dict != None:
+            self.sa = gspread.service_account_from_dict(gspread_auth_dict)         
         if db_user != None:
             self.db_user, self.db_password, self.db_host, self.db_port, self.db_name = \
             db_user, db_password, db_host, db_port, db_name
             postgres_str = f'postgresql://{self.db_user}:{self.db_password}@{self.db_host}:{self.db_port}/{self.db_name}'
             self.postgresql_engine = sa.create_engine(postgres_str)
         #if root_path != None:
         if os.path.isdir('logs') == False:
@@ -72,28 +72,28 @@
         file_handler = logging.FileHandler(f'./logs/UtilLog.log')
         file_handler.setFormatter(formatter)
         logger.addHandler(file_handler)
         self.logger = logger
     
     def prepare_string_matching(self,string, is_url=False):
         """Prepare strings for matching say in a merge function by removing unnecessary 
-                detail, whitespaces and converting to lower case
-            Remove emojis as sometimes they can not come through properly in Tracer data
+        detail, whitespaces and converting to lower case
+        Remove emojis as sometimes they can not come through properly in Tracer data
 
-            Parameters
-            -----------------
-            string : str
-                The string to be cleaned
-            is_url : bool
-                If True then remove characters after the '?' which are utm parameters
-                These can be present in some urls we recieve
-            
-            Returns
-            -----------------
-            string : The cleaned string containing no spaces, punctuation or utm parameters
+        Parameters
+        -----------------
+        string : str
+            The string to be cleaned
+        is_url : bool
+            If True then remove characters after the '?' which are utm parameters
+            These can be present in some urls we recieve
+        
+        Returns
+        -----------------
+        string : The cleaned string containing no spaces, punctuation or utm parameters
         """
         string = string.lower()
         if is_url:
             # get rid of everything after they start to be utm parameters
             string = string.split('?')[0]
         string = emoji_pattern.sub(r'', string)
         string = string.replace(' ', '',)
@@ -101,53 +101,53 @@
         return string
 
     def match_ads(self,df_1, df_2, df_1_exact_col, df_2_exact_col,
                 df_1_fuzzy_col=None, df_2_fuzzy_col=None, is_exact_col_link=True, 
                 matched_col_name='boosted', merge=False,cols_to_merge =['platform'],pickle_name='NoStore'):
 
         """Match row items in df_2 onto row items in df_1 based on two sets of columns, first the dataframes will be tried to match
-            using the first set of columns using an exact match
-            Then for the row items that haven't matched then use the second set of columns and try to match them 
-            using fuzzy matching
+        using the first set of columns using an exact match
+        Then for the row items that haven't matched then use the second set of columns and try to match them 
+        using fuzzy matching
+        
+        Parameters
+        -----------------
+        df_1 : DataFrame
+            The Dataframe that will be searched to see if any corresponding values in df_2, if merge=True df_2 will be left joined onto df_1
+        df_2 : df 
+            The Dataframe that if merge = True will be left joined onto df_1
+        df_1_exact_col : str
+            The Column name from df_1 that will be first attempted to find exact matches
+        df_2_exact_col : str
+            The Column name from df_2 that will be first attempted to find exact matches
+        df_1_fuzzy_col : str
+            The Column name from df_1 that will be attempted to fuzzy match if there was no exact match before
+        df_2_fuzzy_col : str
+            The Column name from df_2 that will be attempted to fuzzy match if there was no exact match before
+        is_exact_col_link : bool
+            Boolean Flag, is the set of columns to be exact matched hyperlinks? If so they will be cleaned to remove utm parameters
+        matched_col_name : str
+            String to name the column which will contain boolean values to indicate whether row items in df_1 found a match in df_2
+        merge : bool
+            Boolean Flag, if true then df_2 will be left joined onto df_1. Else df_1 will be left unchanged apart from column indicating whether there is a match
+        cols_to_merge : list, str
+            List of strings to merge on if 'merge' = True
+        pickle_name : 
+            Name of the dictionary of best matches found by fuzzy matching to be stored as a pickle file. The next time the function is 
+            run with the same pickle_name, the pickle file is used to find matches without having to do slow fuzzy matching from scratch
             
-            Parameters
-            -----------------
-                df_1 : DataFrame
-                    The Dataframe that will be searched to see if any corresponding values in df_2, if merge=True df_2 will be left joined onto df_1
-                df_2 : df 
-                    The Dataframe that if merge = True will be left joined onto df_1
-                df_1_exact_col : str
-                    The Column name from df_1 that will be first attempted to find exact matches
-                df_2_exact_col : str
-                    The Column name from df_2 that will be first attempted to find exact matches
-                df_1_fuzzy_col : str
-                    The Column name from df_1 that will be attempted to fuzzy match if there was no exact match before
-                df_2_fuzzy_col : str
-                    The Column name from df_2 that will be attempted to fuzzy match if there was no exact match before
-                is_exact_col_link : bool
-                    Boolean Flag, is the set of columns to be exact matched hyperlinks? If so they will be cleaned to remove utm parameters
-                matched_col_name : str
-                    String to name the column which will contain boolean values to indicate whether row items in df_1 found a match in df_2
-                merge : bool
-                    Boolean Flag, if true then df_2 will be left joined onto df_1. Else df_1 will be left unchanged apart from column indicating whether there is a match
-                cols_to_merge : list, str
-                    List of strings to merge on if 'merge' = True
-                pickle_name : 
-                    Name of the dictionary of best matches found by fuzzy matching to be stored as a pickle file. The next time the function is 
-                    run with the same pickle_name, the pickle file is used to find matches without having to do slow fuzzy matching from scratch
-                
-            Returns
-            ----------------
-                df_1 : DataFrame
-                    The original df_1 with just a column to indicate whether a match has occured if merge = False else df_1 will have df_2 left joined on
-                df_2 : DataFrame
-                    The original df_2 with cleaned columns and 'Match String' column to help quality check why some rows have or haven't matched
-                df_2_no_match : DataFrame
-                    A dataframe of df_2 row items that haven't found a match in df_1
-                """
+        Returns
+        ----------------
+        df_1 : DataFrame
+            The original df_1 with just a column to indicate whether a match has occured if merge = False else df_1 will have df_2 left joined on
+        df_2 : DataFrame
+            The original df_2 with cleaned columns and 'Match String' column to help quality check why some rows have or haven't matched
+        df_2_no_match : DataFrame
+            A dataframe of df_2 row items that haven't found a match in df_1
+            """
                 
         df_1_num_rows = df_1.shape[0] #Used later to check we don't lose of rows by merging
         if df_1_fuzzy_col == None:
             df_1_fuzzy_col = df_1_exact_col
             df_2_fuzzy_col = df_2_exact_col
 
         #create new columns for the columns to match on, the text in the column will get cleaned later
@@ -244,35 +244,35 @@
         logger.info(f"Number of df_2 that need to match {num_df_2_to_match}")
         logger.info(f"Percentage of df_2 that were matched = {round((matched_df_1_nunique * 100)/num_df_2_to_match,2)}")
 
         return df_1, df_2, df_2_no_match
 
     def best_fuzzy_match(self,list_1, list_2, threshold, pickle_name):
         """Takes in two lists of strings and every string in list_1 is fuzzy matched onto every item in list_2
-            The fuzzy match of a string in list_1 with a string in list_2 with the highest score will count as the 
-            match as long as it is above the threshold. The match is then stored as a key value pair in a dictionary
+        The fuzzy match of a string in list_1 with a string in list_2 with the highest score will count as the 
+        match as long as it is above the threshold. The match is then stored as a key value pair in a dictionary
 
-            The dictionary of matches will be saved as a pickle file to be used next time the function is run to save
-            having to do searches on a string if we've already found a match in the past
+        The dictionary of matches will be saved as a pickle file to be used next time the function is run to save
+        having to do searches on a string if we've already found a match in the past
 
-            Paramaters
-            -------------------
-                list_1 : list
-                    First List of strings, every item will be searched for a fuzzy match in list_2
-                list_2 : list
-                    Second List of strings, every item in list_1 will be fuzzy matched with every item in list 2 and best fuzzy match score wins
-                threshold : integer between 0 and 100
-                    value between 0 and 100 signifying percentage fuzzy match score at which a match is considered sufficiently close
-                pickle_name : str 
-                    name of pickle_file to create or add to if a pickle of the dictionary already exists
-            
-            Returns:
-                best_match_dict : Dictionary
-                    Dictionary of matches (with highest fuzzy match score) between strings in list_1 and list_2 
-                    key = string in list_1, value = string in list_2 """
+        Paramaters
+        -------------------
+        list_1 : list
+            First List of strings, every item will be searched for a fuzzy match in list_2
+        list_2 : list
+            Second List of strings, every item in list_1 will be fuzzy matched with every item in list 2 and best fuzzy match score wins
+        threshold : integer between 0 and 100
+            value between 0 and 100 signifying percentage fuzzy match score at which a match is considered sufficiently close
+        pickle_name : str 
+            name of pickle_file to create or add to if a pickle of the dictionary already exists
+        
+        Returns:
+        best_match_dict : Dictionary
+            Dictionary of matches (with highest fuzzy match score) between strings in list_1 and list_2 
+            key = string in list_1, value = string in list_2 """
 
         best_match_dict = {} 
         stored_best_dict = {} #
         if pickle_name != 'NoStore':
             if os.path.isfile(f'Pickled Files/best_match_dict_{pickle_name}'):
                 stored_best_dict = self.unpickle_data(f'best_match_dict_{pickle_name}')
                 logger.info(f"loaded dict of len :{len(stored_best_dict)}")
@@ -316,30 +316,30 @@
             #best_match_dict_none_removed = {k:v for k,v in best_match_dict.items() if v != 'None'}
             self.pickle_data(best_match_dict,f'best_match_dict_{pickle_name}')
 
         return best_match_dict
 
     def write_to_postgresql(self,df,table_name, if_exists='replace'):
         """Writes a dataframe to a PostgreSQL database table using a SQLalchemy engine defined elsewhere.
-            If writing fails it waits 10 seconds then trys again
+        If writing fails it waits 10 seconds then trys again
             
-            Paramaters
-            --------------
-                df : DataFrame
-                    The Dataframe to send to the PostGreSQL table
-                table_name : str
-                    The name of the table to write the dataframe to
-                if_exists : str
-                    Either 'replace' or 'append' which describes what to do if a table with
-                    that name already exists
-                                        
-            Returns
-            --------------
-                error_message : str
-                    An error message saying that the connection has failed """
+        Paramaters
+        --------------
+        df : DataFrame
+            The Dataframe to send to the PostGreSQL table
+        table_name : str
+            The name of the table to write the dataframe to
+        if_exists : str
+            Either 'replace' or 'append' which describes what to do if a table with
+            that name already exists
+                                    
+        Returns
+        --------------
+        error_message : str
+            An error message saying that the connection has failed """
         # create a SQL alchemy engine to write the data to the database after cleaning
         
         error_message = ''
         try:
             now = time.time()
             df.to_sql(table_name, con=self.postgresql_engine, index=False, if_exists=if_exists)
             time_taken = round(time.time() - now,2)
@@ -362,36 +362,36 @@
         """Determine whether a table called 'table_name' exists"""
         all_table_names = sa.inspect(self.postgresql_engine).get_table_names()
         return (table_name in all_table_names)
     
     def store_daily_organic_data(self,df,output_table_name,num_days_to_store=30,date_column_name='date',
                                     check_created_col=True,created_col='created',refresh_lag=1):
         """Takes in an organic data table with each row item reflecting an organic post with the metric totals
-            updating and increasing in the same row item each day rather than creating a new row item each day.
-            Returns an organic table which has a row item  
+        updating and increasing in the same row item each day rather than creating a new row item each day.
+        Returns an organic table which has a row item  
             
-            Parameters
-            ----------------
-                df : DataFrame
-                    The Dataframe source of organic data
-                output_table : str
-                    The name of the output table to write the data to
-                num_days_to_store : integer
-                    The number of days to look back
-                date_column_name : str
-                    The name of the column which contains the date that the post was originally posted
-                check_created_col : bool
-                    If true then we should check whether the created column in Tracer is up to date, because 
-                    there is no point sending a days worth of data if the row items have not been refreshed
-                created_col : str
-                    The name of the column in the dataset which indicates the date that it was last updated
-            Returns
-            ----------------
-                df : DataFrame
-                    Outputs a table to the 'output_table_name', appends if already exists or creates from scratch if not"""
+        Parameters
+        ----------------
+        df : DataFrame
+            The Dataframe source of organic data
+        output_table : str
+            The name of the output table to write the data to
+        num_days_to_store : integer
+            The number of days to look back
+        date_column_name : str
+            The name of the column which contains the date that the post was originally posted
+        check_created_col : bool
+            If true then we should check whether the created column in Tracer is up to date, because 
+            there is no point sending a days worth of data if the row items have not been refreshed
+        created_col : str
+            The name of the column in the dataset which indicates the date that it was last updated
+        Returns
+        ----------------
+        df : DataFrame
+            Outputs a table to the 'output_table_name', appends if already exists or creates from scratch if not"""
         today_datetime = datetime.today()
         today_date = today_datetime.date() 
         if today_datetime.hour < 15: #Before 3 o'clock in the afternoon
             logger.info("It may be better to run the API later on in the day to make sure the USA data has had time to refresh")
         #Check Tracer data has actually updated
         if self.table_exists(output_table_name):
 
@@ -411,15 +411,15 @@
                 df = df.drop(columns=['datetemp']) #drop temporary date column used for filtering dates
                 self.write_to_postgresql(df,output_table_name,if_exists='append')
         else: #if the table doesn't exist create it with the whole dataset for the first time
             df['date_updated'] = today_datetime
             self.write_to_postgresql(df,output_table_name,if_exists='replace')
 
 
-    def read_from_postgresql(self,table_name,clean_date=True,date_col='date',
+    def read_from_postgresql(self,table_name,clean_date=True,date_col='EnterValue',
                                 dayfirst='EnterValue',yearfirst='EnterValue',format=None,errors='raise'):
         """Reads a table from a PostgreSQL database table using a pscopg2 connection.
             If fails it waits 10 seconds and tries again"""
         conn = pg.connect(dbname=self.db_name, host=self.db_host,
                     port=self.db_port, user=self.db_user, password=self.db_password)
         try:
             now = time.time()
@@ -439,32 +439,55 @@
         conn.close()
         if clean_date:
             df[date_col] = pd.to_datetime(df[date_col],dayfirst=dayfirst,yearfirst=yearfirst,
                                         format=format,errors=errors)
         return df
 
     def write_to_gsheet(self,workbook_name, sheet_name, df, if_exists='replace', sheet_prefix=''):
+        """Write dataframe to google sheet
+
+        Parameters
+        ----------
+        workbook_name : str
+            The name of the google sheet workbook.
+        sheet_name : str
+            The name of the sheet to write data to.
+        df : pandas.DataFrame
+            The dataframe to be written to the google sheet.
+        if_exists : str, optional (default='replace')
+            Determines the behavior when the sheet already exists, options are 'replace' or 'append'.
+        sheet_prefix : str, optional (default='')
+            A prefix to be added to the sheet name.
+
+        Returns
+        -------
+        None"""
         now = datetime.now()
         dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
         df['SheetUpdated'] = dt_string
         try:
+            # Adding the sheet prefix to the sheet name
             sheet_name = sheet_prefix + sheet_name
+            # Open the worksheet
             sheet = self.sa.open(workbook_name).worksheet(sheet_name)
             if if_exists == 'replace': 
+                # Clear the sheet if if_exists is set to 'replace'
                 sheet.clear()
             now = time.time()
+            # Write the dataframe to the sheet
             gd.set_with_dataframe(sheet, df)
             time_taken = round(time.time() - now,2)
             logger.info(f"Time Taken to write to google sheet {sheet_name} = {time_taken}secs")
         except Exception as error_message:
             logger.error(error_message,exc_info=True)
             time.sleep(10)
             gd.set_with_dataframe(sheet, df)
 
-    def read_from_gsheet(self,workbook_name, sheet_name,clean_date=True,date_col='date',
+
+    def read_from_gsheet(self,workbook_name, sheet_name,clean_date=True,date_col='EnterValue',
                             dayfirst='EnterValue',yearfirst='EnterValue',format=None,errors='raise'):
         try:
             spreadsheet = self.sa.open(workbook_name)
         except Exception as error_message:
             logger.info(error_message)
             time.sleep(10)
             spreadsheet = self.sa.open(workbook_name)
```

### Comparing `veetility-0.1.8/veetility.egg-info/PKG-INFO` & `veetility-0.1.9/veetility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.8
+Version: 0.1.9
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

