# Comparing `tmp/arabica-1.4.3.tar.gz` & `tmp/arabica-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.4.3.tar", last modified: Sun Apr 16 22:46:23 2023, max compression
+gzip compressed data, was "arabica-1.4.4.tar", last modified: Mon Apr 17 20:25:33 2023, max compression
```

## Comparing `arabica-1.4.3.tar` & `arabica-1.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 22:46:23.479610 arabica-1.4.3/
--rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.3/LICENSE
--rw-rw-rw-   0        0        0     7944 2023-04-16 22:46:23.479610 arabica-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     7162 2023-04-16 22:45:08.000000 arabica-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 22:46:23.449997 arabica-1.4.3/arabica/
--rw-rw-rw-   0        0        0      105 2023-04-16 22:45:59.000000 arabica-1.4.3/arabica/__init__.py
--rw-rw-rw-   0        0        0    11740 2023-04-16 21:14:18.000000 arabica-1.4.3/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    29482 2023-04-16 21:15:43.000000 arabica-1.4.3/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.3/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.3/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.3/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.3/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.3/arabica/preprocess.py
--rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.3/arabica/sentiment.py
--rw-rw-rw-   0        0        0      449 2022-10-18 19:06:35.000000 arabica-1.4.3/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:46:23.479610 arabica-1.4.3/arabica.egg-info/
--rw-rw-rw-   0        0        0     7944 2023-04-16 22:46:23.000000 arabica-1.4.3/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-16 22:46:23.000000 arabica-1.4.3/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 22:46:23.000000 arabica-1.4.3/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-04-16 22:46:23.000000 arabica-1.4.3/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 22:46:23.000000 arabica-1.4.3/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-04-16 22:45:59.000000 arabica-1.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 22:46:23.489612 arabica-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-04-16 22:45:59.000000 arabica-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:25:33.409185 arabica-1.4.4/
+-rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0     7797 2023-04-17 20:25:33.413690 arabica-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7017 2023-04-17 20:12:59.000000 arabica-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 20:25:33.366803 arabica-1.4.4/arabica/
+-rw-rw-rw-   0        0        0      105 2023-04-17 20:24:20.000000 arabica-1.4.4/arabica/__init__.py
+-rw-rw-rw-   0        0        0    11740 2023-04-16 21:14:18.000000 arabica-1.4.4/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    29482 2023-04-16 21:15:43.000000 arabica-1.4.4/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.4/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.4/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.4/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.4/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.4/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.4/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      449 2022-10-18 19:06:35.000000 arabica-1.4.4/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:25:33.403589 arabica-1.4.4/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7797 2023-04-17 20:25:32.000000 arabica-1.4.4/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-17 20:25:33.000000 arabica-1.4.4/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 20:25:32.000000 arabica-1.4.4/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-04-17 20:25:32.000000 arabica-1.4.4/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 20:25:32.000000 arabica-1.4.4/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-04-17 20:23:25.000000 arabica-1.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 20:25:33.427307 arabica-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-04-17 20:23:32.000000 arabica-1.4.4/setup.py
```

### Comparing `arabica-1.4.3/PKG-INFO` & `arabica-1.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
@@ -23,15 +23,15 @@
 
 * **Descriptive n-gram analysis**: n-gram frequencies
 * **Time-series n-gram analysis**: n-gram frequencies over a period
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
 * **Structural breaks identification**: Jenks Optimization Method
 
-It automatically cleans data from punctuation on input. Furthermore, it can apply all or a selected combination of the following cleaning operations:
+It automatically cleans data from punctuation on input. It can also apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
 * Remove the standard list(s) of stopwords
 * Remove an additional list of specific strings
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
@@ -79,43 +79,41 @@
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
                  max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
                  stopwords: [],            # Languages for stop words
                  skip: [],                 # Remove additional strings
                  numbers: bool = False,    # Remove all digits
-                 lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
+                 lower_case: bool = False  # Lowercase text
 ) 
 ```
 
-**cappuccino**  enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings
+**cappuccino**  enables cleaning operations (lower casing, numbers, stop words, and additional strings
 removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
                stopwords: [],            # Languages for stop words
                skip: [] ,                # Remove additional strings
                numbers: bool = False,    # Remove numbers
-               lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
-)
+               lower_case: bool = False  # Lowercase text
 ```
+
 **coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
-The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media.
+* The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
 
-It was developed by: 
-*Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14).*
+* Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
-Structural breaks in the time series are identified with the Fisher-Jenks algorithm, or **Jenks Optimisation Method** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
                  skip: [] ,                 # Remove additional strings
                  preprocess: bool = False,  # Clean data from numbers and punctuation
@@ -132,22 +130,22 @@
 ```
 
 It is possible to remove more sets of stopwords at once by `stopwords = ['language 1', 'language2','etc..']`
 
 
 ## Documentation, examples and tutorials
 
-* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html). 
+* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html)
 
 For more examples of coding, read these  tutorials:
 
 **General use:**
-                     
-* Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
+
 * Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
+* Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                                          
 * Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
 * **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
 * **Meta-data description:** TBA
```

### Comparing `arabica-1.4.3/README.md` & `arabica-1.4.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 * **Descriptive n-gram analysis**: n-gram frequencies
 * **Time-series n-gram analysis**: n-gram frequencies over a period
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
 * **Structural breaks identification**: Jenks Optimization Method
 
-It automatically cleans data from punctuation on input. Furthermore, it can apply all or a selected combination of the following cleaning operations:
+It automatically cleans data from punctuation on input. It can also apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
 * Remove the standard list(s) of stopwords
 * Remove an additional list of specific strings
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
@@ -61,43 +61,41 @@
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
                  max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
                  stopwords: [],            # Languages for stop words
                  skip: [],                 # Remove additional strings
                  numbers: bool = False,    # Remove all digits
-                 lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
+                 lower_case: bool = False  # Lowercase text
 ) 
 ```
 
-**cappuccino**  enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings
+**cappuccino**  enables cleaning operations (lower casing, numbers, stop words, and additional strings
 removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
                stopwords: [],            # Languages for stop words
                skip: [] ,                # Remove additional strings
                numbers: bool = False,    # Remove numbers
-               lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
-)
+               lower_case: bool = False  # Lowercase text
 ```
+
 **coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
-The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media.
+* The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
 
-It was developed by: 
-*Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14).*
+* Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
-Structural breaks in the time series are identified with the Fisher-Jenks algorithm, or **Jenks Optimisation Method** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
                  skip: [] ,                 # Remove additional strings
                  preprocess: bool = False,  # Clean data from numbers and punctuation
@@ -114,22 +112,22 @@
 ```
 
 It is possible to remove more sets of stopwords at once by `stopwords = ['language 1', 'language2','etc..']`
 
 
 ## Documentation, examples and tutorials
 
-* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html). 
+* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html)
 
 For more examples of coding, read these  tutorials:
 
 **General use:**
-                     
-* Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
+
 * Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
+* Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                                          
 * Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
 * **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
 * **Meta-data description:** TBA
```

### Comparing `arabica-1.4.3/arabica/arabica_freq.py` & `arabica-1.4.4/arabica/arabica_freq.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.3/arabica/cappuccino.py` & `arabica-1.4.4/arabica/cappuccino.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.3/arabica/clean_ngram.py` & `arabica-1.4.4/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.3/arabica/coffee_break.py` & `arabica-1.4.4/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.3/arabica/group.py` & `arabica-1.4.4/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.3/arabica/preprocess.py` & `arabica-1.4.4/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.3/arabica.egg-info/PKG-INFO` & `arabica-1.4.4/arabica.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
@@ -23,15 +23,15 @@
 
 * **Descriptive n-gram analysis**: n-gram frequencies
 * **Time-series n-gram analysis**: n-gram frequencies over a period
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
 * **Structural breaks identification**: Jenks Optimization Method
 
-It automatically cleans data from punctuation on input. Furthermore, it can apply all or a selected combination of the following cleaning operations:
+It automatically cleans data from punctuation on input. It can also apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
 * Remove the standard list(s) of stopwords
 * Remove an additional list of specific strings
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
@@ -79,43 +79,41 @@
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
                  max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
                  stopwords: [],            # Languages for stop words
                  skip: [],                 # Remove additional strings
                  numbers: bool = False,    # Remove all digits
-                 lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
+                 lower_case: bool = False  # Lowercase text
 ) 
 ```
 
-**cappuccino**  enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings
+**cappuccino**  enables cleaning operations (lower casing, numbers, stop words, and additional strings
 removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
                stopwords: [],            # Languages for stop words
                skip: [] ,                # Remove additional strings
                numbers: bool = False,    # Remove numbers
-               lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
-)
+               lower_case: bool = False  # Lowercase text
 ```
+
 **coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. 
 
-The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media.
+* The implemented model is **VADER** (Valence Aware Dictionary and sEntiment Reasoner), a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See: *Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text.* Available from [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
 
-It was developed by: 
-*Hutto, & Gilbert, 2014. VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14).*
+* Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
-Structural breaks in the time series are identified with the Fisher-Jenks algorithm, or **Jenks Optimisation Method** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
                  skip: [] ,                 # Remove additional strings
                  preprocess: bool = False,  # Clean data from numbers and punctuation
@@ -132,22 +130,22 @@
 ```
 
 It is possible to remove more sets of stopwords at once by `stopwords = ['language 1', 'language2','etc..']`
 
 
 ## Documentation, examples and tutorials
 
-* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html). 
+* Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html)
 
 For more examples of coding, read these  tutorials:
 
 **General use:**
-                     
-* Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
+
 * Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
+* Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                                          
 * Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
 * **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
 * **Meta-data description:** TBA
```

### Comparing `arabica-1.4.3/pyproject.toml` & `arabica-1.4.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.4.3"
+version = "1.4.4"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.4.3/setup.py` & `arabica-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.4.3",
+        version="1.4.4",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
```

