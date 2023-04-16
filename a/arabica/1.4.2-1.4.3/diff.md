# Comparing `tmp/arabica-1.4.2.tar.gz` & `tmp/arabica-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.4.2.tar", last modified: Sun Apr 16 22:12:54 2023, max compression
+gzip compressed data, was "arabica-1.4.3.tar", last modified: Sun Apr 16 22:46:23 2023, max compression
```

## Comparing `arabica-1.4.2.tar` & `arabica-1.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 22:12:54.102485 arabica-1.4.2/
--rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.2/LICENSE
--rw-rw-rw-   0        0        0     7913 2023-04-16 22:12:54.102485 arabica-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     7132 2023-04-16 22:11:13.000000 arabica-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 22:12:54.072851 arabica-1.4.2/arabica/
--rw-rw-rw-   0        0        0      105 2023-04-16 21:43:12.000000 arabica-1.4.2/arabica/__init__.py
--rw-rw-rw-   0        0        0    11740 2023-04-16 21:14:18.000000 arabica-1.4.2/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    29482 2023-04-16 21:15:43.000000 arabica-1.4.2/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.2/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.2/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.2/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.2/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.2/arabica/preprocess.py
--rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.2/arabica/sentiment.py
--rw-rw-rw-   0        0        0      449 2022-10-18 19:06:35.000000 arabica-1.4.2/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:12:54.102485 arabica-1.4.2/arabica.egg-info/
--rw-rw-rw-   0        0        0     7913 2023-04-16 22:12:53.000000 arabica-1.4.2/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-16 22:12:54.000000 arabica-1.4.2/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 22:12:53.000000 arabica-1.4.2/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-04-16 22:12:53.000000 arabica-1.4.2/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 22:12:54.000000 arabica-1.4.2/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-04-16 22:12:19.000000 arabica-1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 22:12:54.102485 arabica-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-04-16 22:12:19.000000 arabica-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:46:23.479610 arabica-1.4.3/
+-rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0     7944 2023-04-16 22:46:23.479610 arabica-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7162 2023-04-16 22:45:08.000000 arabica-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 22:46:23.449997 arabica-1.4.3/arabica/
+-rw-rw-rw-   0        0        0      105 2023-04-16 22:45:59.000000 arabica-1.4.3/arabica/__init__.py
+-rw-rw-rw-   0        0        0    11740 2023-04-16 21:14:18.000000 arabica-1.4.3/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    29482 2023-04-16 21:15:43.000000 arabica-1.4.3/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.3/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.3/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.3/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.3/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.3/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.3/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      449 2022-10-18 19:06:35.000000 arabica-1.4.3/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:46:23.479610 arabica-1.4.3/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7944 2023-04-16 22:46:23.000000 arabica-1.4.3/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-16 22:46:23.000000 arabica-1.4.3/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 22:46:23.000000 arabica-1.4.3/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-04-16 22:46:23.000000 arabica-1.4.3/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 22:46:23.000000 arabica-1.4.3/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-04-16 22:45:59.000000 arabica-1.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 22:46:23.489612 arabica-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-04-16 22:45:59.000000 arabica-1.4.3/setup.py
```

### Comparing `arabica-1.4.2/PKG-INFO` & `arabica-1.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.2
+Version: 1.4.3
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
@@ -65,16 +65,17 @@
 from arabica import coffee_break 
 ```
 
 
 
 * **Choose a method:**
 
-**arabica_freq** returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
-To remove stopwords, select aggregation period and choose a specific set of cleaning operations:
+**arabica_freq** enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings 
+removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
+
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
@@ -82,16 +83,16 @@
                  stopwords: [],            # Languages for stop words
                  skip: [],                 # Remove additional strings
                  numbers: bool = False,    # Remove all digits
                  lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
 ) 
 ```
 
-**cappuccino**  enables standard cleaning operations (stop words, numbers, and punctuation removal) and provides 
-plots for descriptive (word cloud) and time-series (heatmap, line plot) text data visualization.
+**cappuccino**  enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings
+removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
@@ -133,23 +134,23 @@
 It is possible to remove more sets of stopwords at once by `stopwords = ['language 1', 'language2','etc..']`
 
 
 ## Documentation, examples and tutorials
 
 * Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html). 
 
-* For more examples of coding, read these  tutorials:
+For more examples of coding, read these  tutorials:
 
 **General use:**
                      
-->  Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
-->  Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
-->  Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
+* Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
+* Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
+* Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
-->  **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
-->  **Meta-data description:** TBA
+* **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
+* **Meta-data description:** TBA
 
 ---
 
 Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.4.2/README.md` & `arabica-1.4.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -47,16 +47,17 @@
 from arabica import coffee_break 
 ```
 
 
 
 * **Choose a method:**
 
-**arabica_freq** returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
-To remove stopwords, select aggregation period and choose a specific set of cleaning operations:
+**arabica_freq** enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings 
+removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
+
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
@@ -64,16 +65,16 @@
                  stopwords: [],            # Languages for stop words
                  skip: [],                 # Remove additional strings
                  numbers: bool = False,    # Remove all digits
                  lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
 ) 
 ```
 
-**cappuccino**  enables standard cleaning operations (stop words, numbers, and punctuation removal) and provides 
-plots for descriptive (word cloud) and time-series (heatmap, line plot) text data visualization.
+**cappuccino**  enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings
+removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
@@ -115,23 +116,23 @@
 It is possible to remove more sets of stopwords at once by `stopwords = ['language 1', 'language2','etc..']`
 
 
 ## Documentation, examples and tutorials
 
 * Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html). 
 
-* For more examples of coding, read these  tutorials:
+For more examples of coding, read these  tutorials:
 
 **General use:**
                      
-->  Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
-->  Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
-->  Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
+* Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
+* Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
+* Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
-->  **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
-->  **Meta-data description:** TBA
+* **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
+* **Meta-data description:** TBA
 
 ---
 
 Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.4.2/arabica/arabica_freq.py` & `arabica-1.4.3/arabica/arabica_freq.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.2/arabica/cappuccino.py` & `arabica-1.4.3/arabica/cappuccino.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.2/arabica/clean_ngram.py` & `arabica-1.4.3/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.2/arabica/coffee_break.py` & `arabica-1.4.3/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.2/arabica/group.py` & `arabica-1.4.3/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.2/arabica/preprocess.py` & `arabica-1.4.3/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.2/arabica.egg-info/PKG-INFO` & `arabica-1.4.3/arabica.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.2
+Version: 1.4.3
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
@@ -65,16 +65,17 @@
 from arabica import coffee_break 
 ```
 
 
 
 * **Choose a method:**
 
-**arabica_freq** returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
-To remove stopwords, select aggregation period and choose a specific set of cleaning operations:
+**arabica_freq** enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings 
+removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
+
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
@@ -82,16 +83,16 @@
                  stopwords: [],            # Languages for stop words
                  skip: [],                 # Remove additional strings
                  numbers: bool = False,    # Remove all digits
                  lower_case: bool = False  # Lowercase text before cleaning and frequency analysis
 ) 
 ```
 
-**cappuccino**  enables standard cleaning operations (stop words, numbers, and punctuation removal) and provides 
-plots for descriptive (word cloud) and time-series (heatmap, line plot) text data visualization.
+**cappuccino**  enables a specific set of cleaning operations (lower casing, numbers, stop words, and additional strings
+removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
@@ -133,23 +134,23 @@
 It is possible to remove more sets of stopwords at once by `stopwords = ['language 1', 'language2','etc..']`
 
 
 ## Documentation, examples and tutorials
 
 * Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html). 
 
-* For more examples of coding, read these  tutorials:
+For more examples of coding, read these  tutorials:
 
 **General use:**
                      
-->  Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
-->  Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
-->  Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
+* Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                        
+* Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
+* Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
-->  **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
-->  **Meta-data description:** TBA
+* **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
+* **Meta-data description:** TBA
 
 ---
 
 Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.4.2/pyproject.toml` & `arabica-1.4.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.4.2"
+version = "1.4.3"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.4.2/setup.py` & `arabica-1.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.4.2",
+        version="1.4.3",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
```

