# Comparing `tmp/arabica-1.4.1.tar.gz` & `tmp/arabica-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.4.1.tar", last modified: Tue Mar 21 20:33:17 2023, max compression
+gzip compressed data, was "arabica-1.4.2.tar", last modified: Sun Apr 16 22:12:54 2023, max compression
```

## Comparing `arabica-1.4.1.tar` & `arabica-1.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 20:33:17.197887 arabica-1.4.1/
--rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     7463 2023-03-21 20:33:17.197887 arabica-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     6685 2023-03-14 23:12:54.000000 arabica-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 20:33:17.168109 arabica-1.4.1/arabica/
--rw-rw-rw-   0        0        0      105 2023-03-14 23:09:59.000000 arabica-1.4.1/arabica/__init__.py
--rw-rw-rw-   0        0        0    11869 2023-03-18 22:29:57.000000 arabica-1.4.1/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    29587 2023-03-21 19:21:05.000000 arabica-1.4.1/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.1/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.1/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     7226 2023-03-20 23:44:26.000000 arabica-1.4.1/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.1/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.1/arabica/preprocess.py
--rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.1/arabica/sentiment.py
--rw-rw-rw-   0        0        0      449 2022-10-18 19:06:35.000000 arabica-1.4.1/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-03-21 20:33:17.195888 arabica-1.4.1/arabica.egg-info/
--rw-rw-rw-   0        0        0     7463 2023-03-21 20:33:17.000000 arabica-1.4.1/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-03-21 20:33:17.000000 arabica-1.4.1/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 20:33:17.000000 arabica-1.4.1/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-03-21 20:33:17.000000 arabica-1.4.1/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-21 20:33:17.000000 arabica-1.4.1/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-03-21 20:30:34.000000 arabica-1.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-21 20:33:17.200885 arabica-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-03-21 20:30:34.000000 arabica-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:12:54.102485 arabica-1.4.2/
+-rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     7913 2023-04-16 22:12:54.102485 arabica-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7132 2023-04-16 22:11:13.000000 arabica-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 22:12:54.072851 arabica-1.4.2/arabica/
+-rw-rw-rw-   0        0        0      105 2023-04-16 21:43:12.000000 arabica-1.4.2/arabica/__init__.py
+-rw-rw-rw-   0        0        0    11740 2023-04-16 21:14:18.000000 arabica-1.4.2/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    29482 2023-04-16 21:15:43.000000 arabica-1.4.2/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.2/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.2/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.2/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.2/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.2/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.2/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      449 2022-10-18 19:06:35.000000 arabica-1.4.2/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:12:54.102485 arabica-1.4.2/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7913 2023-04-16 22:12:53.000000 arabica-1.4.2/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-16 22:12:54.000000 arabica-1.4.2/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 22:12:53.000000 arabica-1.4.2/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-04-16 22:12:53.000000 arabica-1.4.2/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 22:12:54.000000 arabica-1.4.2/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-04-16 22:12:19.000000 arabica-1.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 22:12:54.102485 arabica-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-04-16 22:12:19.000000 arabica-1.4.2/setup.py
```

### Comparing `arabica-1.4.1/PKG-INFO` & `arabica-1.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
@@ -21,22 +21,21 @@
 
 Text data is often recorded as a time series with significant variability over time. Some examples of time-series text data include Twitter tweets, research article metadata, product reviews, and newspaper headlines. Arabica makes exploratory analysis of these time-series text datasets simple by providing:
 
 * **Descriptive n-gram analysis**: n-gram frequencies
 * **Time-series n-gram analysis**: n-gram frequencies over a period
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
-*  **Structural breaks identification**: Jenks Optimization Method
+* **Structural breaks identification**: Jenks Optimization Method
 
-It can apply all or a selected combination of the following cleaning operations:
+It automatically cleans data from punctuation on input. Furthermore, it can apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
-* Remove punctuation from the text
-* Remove standard list of stopwords
-* Remove an additional specific list of words
+* Remove the standard list(s) of stopwords
+* Remove an additional list of specific strings
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
 It reads dates in:
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
 * **European-style**: *DD/MM/YYYY* (2013-31-12, 09-Feb-2009, 2013-31-12 11:46:17, etc.) date and datetime formats.
@@ -75,54 +74,53 @@
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
-                 max_words: int = '',      # Max number for most frequent n-grams displayed for each period
+                 max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
                  stopwords: [],            # Languages for stop words
                  skip: [],                 # Remove additional strings
                  numbers: bool = False,    # Remove all digits
-                 punct: bool = False,      # Remove all punctuation
                  lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
 ) 
 ```
 
-**cappuccino**  enables standard cleaning operations (stop words, numbers, and punctuation removal) and provides
+**cappuccino**  enables standard cleaning operations (stop words, numbers, and punctuation removal) and provides 
 plots for descriptive (word cloud) and time-series (heatmap, line plot) text data visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
-               max_words int = '',       # Max number for most frequent n-grams displayed for each period
+               max_words int = '',       # Maximum of most frequent n-grams displayed for each period
                stopwords: [],            # Languages for stop words
                skip: [] ,                # Remove additional strings
                numbers: bool = False,    # Remove numbers
-               punct: bool = False,      # Remove punctuation
                lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
 )
 ```
-**coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment.
+**coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
 The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media.
 
-It was developed by:
+It was developed by: 
 *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14).*
 
 Structural breaks in the time series are identified with the Fisher-Jenks algorithm, or **Jenks Optimisation Method** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
+                 skip: [] ,                 # Remove additional strings
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
                  n_breaks: int =''          # Number of breaks: min. 2
 )
 ```
 
 
@@ -133,20 +131,25 @@
 ```
 
 It is possible to remove more sets of stopwords at once by `stopwords = ['language 1', 'language2','etc..']`
 
 
 ## Documentation, examples and tutorials
 
-* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html).
+* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html). 
 
 * For more examples of coding, read these  tutorials:
 
-**Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis** [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)
+**General use:**
+                     
+->  Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
+->  Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
+->  Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
-**Visualization Module in Arabica Speeds Up Text Data Exploration** [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)
+**Applications:**
 
-**Sentiment Analysis and Structural Breaks in Time-Series Text Data** [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)
+->  **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
+->  **Meta-data description:** TBA
 
 ---
 
 Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.4.1/README.md` & `arabica-1.4.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 
 Text data is often recorded as a time series with significant variability over time. Some examples of time-series text data include Twitter tweets, research article metadata, product reviews, and newspaper headlines. Arabica makes exploratory analysis of these time-series text datasets simple by providing:
 
 * **Descriptive n-gram analysis**: n-gram frequencies
 * **Time-series n-gram analysis**: n-gram frequencies over a period
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
-*  **Structural breaks identification**: Jenks Optimization Method
+* **Structural breaks identification**: Jenks Optimization Method
 
-It can apply all or a selected combination of the following cleaning operations:
+It automatically cleans data from punctuation on input. Furthermore, it can apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
-* Remove punctuation from the text
-* Remove standard list of stopwords
-* Remove an additional specific list of words
+* Remove the standard list(s) of stopwords
+* Remove an additional list of specific strings
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
 It reads dates in:
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
 * **European-style**: *DD/MM/YYYY* (2013-31-12, 09-Feb-2009, 2013-31-12 11:46:17, etc.) date and datetime formats.
@@ -57,54 +56,53 @@
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
-                 max_words: int = '',      # Max number for most frequent n-grams displayed for each period
+                 max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
                  stopwords: [],            # Languages for stop words
                  skip: [],                 # Remove additional strings
                  numbers: bool = False,    # Remove all digits
-                 punct: bool = False,      # Remove all punctuation
                  lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
 ) 
 ```
 
-**cappuccino**  enables standard cleaning operations (stop words, numbers, and punctuation removal) and provides
+**cappuccino**  enables standard cleaning operations (stop words, numbers, and punctuation removal) and provides 
 plots for descriptive (word cloud) and time-series (heatmap, line plot) text data visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
-               max_words int = '',       # Max number for most frequent n-grams displayed for each period
+               max_words int = '',       # Maximum of most frequent n-grams displayed for each period
                stopwords: [],            # Languages for stop words
                skip: [] ,                # Remove additional strings
                numbers: bool = False,    # Remove numbers
-               punct: bool = False,      # Remove punctuation
                lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
 )
 ```
-**coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment.
+**coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
 The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media.
 
-It was developed by:
+It was developed by: 
 *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14).*
 
 Structural breaks in the time series are identified with the Fisher-Jenks algorithm, or **Jenks Optimisation Method** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
+                 skip: [] ,                 # Remove additional strings
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
                  n_breaks: int =''          # Number of breaks: min. 2
 )
 ```
 
 
@@ -115,20 +113,25 @@
 ```
 
 It is possible to remove more sets of stopwords at once by `stopwords = ['language 1', 'language2','etc..']`
 
 
 ## Documentation, examples and tutorials
 
-* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html).
+* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html). 
 
 * For more examples of coding, read these  tutorials:
 
-**Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis** [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)
+**General use:**
+                     
+->  Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
+->  Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
+->  Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
-**Visualization Module in Arabica Speeds Up Text Data Exploration** [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)
+**Applications:**
 
-**Sentiment Analysis and Structural Breaks in Time-Series Text Data** [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)
+->  **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
+->  **Meta-data description:** TBA
 
 ---
 
 Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.4.1/arabica/arabica_freq.py` & `arabica-1.4.2/arabica/arabica_freq.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
                  stopwords: [],             # Languages for stop words
                  skip: [],                  # Remove additional strings
                  time_freq: str = '',       # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
                  max_words: int = '',       # Max number for most frequent n-grams displayed for each period
                  numbers: bool = False,     # Remove all digits
-                 punct: bool = False,       # Remove all punctuation
                  lower_case: bool = False   # Lowercase text before cleaning and frequency analysis
                  ):
 
     data=pd.DataFrame()
     data['text']=text
 
     if time_freq != 'ungroup':
@@ -43,19 +42,21 @@
         data['time']=data['time'].astype(str)
         data['time'] = pd.to_datetime(data['time'], dayfirst=False)
 
     data=data.set_index(data['time'])
     data.replace("", float("NaN"), inplace=True)
     data.dropna(subset = ["text"], inplace=True)
 
+    if skip is not None:
+        data['text'] = data.text.str.replace('|'.join(skip), '.', regex=True).str.strip()
+
     if lower_case is True:
         data['text'] = np.vectorize(lower_casing)(data['text'])
 
-    if punct is True:
-        data['text'] = np.vectorize(preprocess)(data['text'])
+    data['text'] = np.vectorize(preprocess)(data['text'])
 
     if stopwords is not None:
         data['text'] = data.text.map(lambda x: remove_stopwords(x,stopwords=[stopwords]))
 
     if numbers is True:
         data['text'] = np.vectorize(remove_numbers)(data['text'])
 
@@ -65,20 +66,17 @@
     trigrams_freq = []
 
     for i, row in data.iterrows():
         period = row[1]
         periods.append(period)
         word = row[0]
         token = str(word).split()
-        if skip is not None:
-            tokens_clean = [x for x in token if x not in skip]
-        else: tokens_clean = token
-        unigrams = list(ngrams(tokens_clean, 1))
-        bigrams = list(bi(tokens_clean))
-        trigrams = list(tri(tokens_clean))
+        unigrams = list(ngrams(token, 1))
+        bigrams = list(bi(token))
+        trigrams = list(tri(token))
         unigrams_freq.append(unigrams)
         bigrams_freq.append(bigrams)
         trigrams_freq.append(trigrams)
 
     df = pd.DataFrame()
     df['period'] = periods
     df['period'] = df['period'].astype(str)
```

### Comparing `arabica-1.4.1/arabica/cappuccino.py` & `arabica-1.4.2/arabica/cappuccino.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,38 +5,35 @@
 from wordcloud import WordCloud
 import matplotlib.pyplot as plt
 from matplotlib.pyplot import figure
 import pandas as pd
 import numpy as np
 
 
-
 def cappuccino(text: str,                  # Text
                time: str,                  # Time
                date_format: str,           # Date format: 'eur' - European, 'us' - American
                stopwords: [],              # Languages for stop words
                skip: [ ],                  # Remove additional strings
                plot: str = '',             # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',            # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',        # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words: int = '',        # Max number for most frequent n-grams displayed for each period
                numbers: bool = False,      # Remove numbers
-               punct: bool = False,        # Remove punctuation
                lower_case: bool = False):  # Lowercase text before cleaning and frequency analysis
 
 
     result = arabica_freq(text = text,
                           time = time,
                           date_format = date_format,
                           time_freq = time_freq,
                           max_words = max_words,
                           stopwords = stopwords,
                           skip = skip,
                           numbers = numbers,
-                          punct = punct,
                           lower_case = lower_case)
 
 
     if ngram == 1:
         if time_freq == 'ungroup':
             if plot == 'wordcloud':
                 unigrams_df = result[['unigram','unigram_freq']]
@@ -97,15 +94,15 @@
                        + scale_fill_gradient(name = "frequency",
                                              low = "#f0f4ed",
                                              high = "#496160")
                        + theme(axis_title_x=element_text(colour = "black"),
                                axis_title_y=element_text(colour="black"),
                                axis_text_x=element_text(colour = "black", rotation=45, hjust=1),
                                figure_size=(10, 5),
-                               panel_grid_major = element_line(color='grey',size = 0.1),
+                               panel_grid_major = element_line(color='black',size = 0.1),
                                panel_background = element_rect(colour = "white", fill = "white"),
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
 
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
@@ -189,15 +186,15 @@
                        + scale_fill_gradient(name = "frequency",
                                              low = "#f0f4ed",
                                              high = "#496160")
                        + theme(axis_title_x=element_text(colour = "black"),
                                axis_title_y=element_text(colour="black"),
                                axis_text_x=element_text(colour = "black", rotation=45, hjust='1'),
                                figure_size=(10, 6),
-                               panel_grid_major = element_line(color='grey',size = 0.1),
+                               panel_grid_major = element_line(color='black',size = 0.1),
                                panel_background = element_rect(colour = "white", fill = "white"),
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
 
@@ -298,15 +295,15 @@
                        + scale_fill_gradient(name = "frequency",
                                              low = "#f0f4ed",
                                              high = "#496160")
                        + theme(axis_title_x=element_text(colour = "black"),
                                axis_title_y=element_text(colour="black"),
                                axis_text_x=element_text(colour = "black", rotation=45, hjust=1),
                                figure_size=(10, 8),
-                               panel_grid_major = element_line(color='grey',size = 0.1),
+                               panel_grid_major = element_line(color='black',size = 0.1),
                                panel_background = element_rect(colour = "white", fill = "white"),
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
 
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
@@ -388,15 +385,15 @@
                        + scale_fill_gradient(name = "frequency",
                                              low = "#f0f4ed",
                                              high = "#496160")
                        + theme(axis_title_x=element_text(colour = "black"),
                                axis_title_y=element_text(colour="black"),
                                axis_text_x=element_text(colour = "black", rotation=45, hjust=1),
                                figure_size=(10, 8),
-                               panel_grid_major = element_line(color='grey',size = 0.1),
+                               panel_grid_major = element_line(color='black',size = 0.1),
                                panel_background = element_rect(colour = "white", fill = "white"),
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
 
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
```

### Comparing `arabica-1.4.1/arabica/clean_ngram.py` & `arabica-1.4.2/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.1/arabica/coffee_break.py` & `arabica-1.4.2/arabica/coffee_break.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 
 from .preprocess import *
 from .group import *
 from .sentiment import sentiment_vader
 
 
-
 def coffee_break(text: str,                  # Text column
                  time: str,                  # Time column
                  date_format: str,           # Date format: 'eur' - European, 'us' - American
+                 skip: [ ],                  # Remove additional strings
                  preprocess: bool = False,   # Clean data from numbers and punctuation
                  time_freq: int = '',        # Aggregation period: 'Y'/'M'
                  n_breaks: int = ''):        # Number of breaks: min. 2
 
 
     if n_breaks is not None:
         if n_breaks < 2:
@@ -34,14 +34,18 @@
     data['text']=text
     data['period']=time
 
     data=data.set_index(data['period'])
     data.replace("", float("NaN"), inplace=True)
     data.dropna(subset = ["text"], inplace=True)
 
+
+    if skip is not None:
+        data['text'] = data.text.str.replace('|'.join(skip), '.', regex=True).str.strip()
+
     if preprocess is True:
         data['text'] = np.vectorize(preprocess_sentiment)(data['text'])
 
 
     if time_freq == 'M':
         if date_format == 'eur':
             data['period']=data['period'].astype(str)
```

### Comparing `arabica-1.4.1/arabica/group.py` & `arabica-1.4.2/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.1/arabica/preprocess.py` & `arabica-1.4.2/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.1/arabica.egg-info/PKG-INFO` & `arabica-1.4.2/arabica.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
@@ -21,22 +21,21 @@
 
 Text data is often recorded as a time series with significant variability over time. Some examples of time-series text data include Twitter tweets, research article metadata, product reviews, and newspaper headlines. Arabica makes exploratory analysis of these time-series text datasets simple by providing:
 
 * **Descriptive n-gram analysis**: n-gram frequencies
 * **Time-series n-gram analysis**: n-gram frequencies over a period
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
-*  **Structural breaks identification**: Jenks Optimization Method
+* **Structural breaks identification**: Jenks Optimization Method
 
-It can apply all or a selected combination of the following cleaning operations:
+It automatically cleans data from punctuation on input. Furthermore, it can apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
-* Remove punctuation from the text
-* Remove standard list of stopwords
-* Remove an additional specific list of words
+* Remove the standard list(s) of stopwords
+* Remove an additional list of specific strings
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
 It reads dates in:
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
 * **European-style**: *DD/MM/YYYY* (2013-31-12, 09-Feb-2009, 2013-31-12 11:46:17, etc.) date and datetime formats.
@@ -75,54 +74,53 @@
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
-                 max_words: int = '',      # Max number for most frequent n-grams displayed for each period
+                 max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
                  stopwords: [],            # Languages for stop words
                  skip: [],                 # Remove additional strings
                  numbers: bool = False,    # Remove all digits
-                 punct: bool = False,      # Remove all punctuation
                  lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
 ) 
 ```
 
-**cappuccino**  enables standard cleaning operations (stop words, numbers, and punctuation removal) and provides
+**cappuccino**  enables standard cleaning operations (stop words, numbers, and punctuation removal) and provides 
 plots for descriptive (word cloud) and time-series (heatmap, line plot) text data visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
-               max_words int = '',       # Max number for most frequent n-grams displayed for each period
+               max_words int = '',       # Maximum of most frequent n-grams displayed for each period
                stopwords: [],            # Languages for stop words
                skip: [] ,                # Remove additional strings
                numbers: bool = False,    # Remove numbers
-               punct: bool = False,      # Remove punctuation
                lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
 )
 ```
-**coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment.
+**coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
 The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media.
 
-It was developed by:
+It was developed by: 
 *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14).*
 
 Structural breaks in the time series are identified with the Fisher-Jenks algorithm, or **Jenks Optimisation Method** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
+                 skip: [] ,                 # Remove additional strings
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
                  n_breaks: int =''          # Number of breaks: min. 2
 )
 ```
 
 
@@ -133,20 +131,25 @@
 ```
 
 It is possible to remove more sets of stopwords at once by `stopwords = ['language 1', 'language2','etc..']`
 
 
 ## Documentation, examples and tutorials
 
-* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html).
+* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html). 
 
 * For more examples of coding, read these  tutorials:
 
-**Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis** [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)
+**General use:**
+                     
+->  Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
+->  Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
+->  Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
-**Visualization Module in Arabica Speeds Up Text Data Exploration** [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)
+**Applications:**
 
-**Sentiment Analysis and Structural Breaks in Time-Series Text Data** [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)
+->  **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
+->  **Meta-data description:** TBA
 
 ---
 
 Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.4.1/pyproject.toml` & `arabica-1.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.4.1"
+version = "1.4.2"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.4.1/setup.py` & `arabica-1.4.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.4.1",
+        version="1.4.2",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
```

