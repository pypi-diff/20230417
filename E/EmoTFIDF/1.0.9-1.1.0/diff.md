# Comparing `tmp/EmoTFIDF-1.0.9.tar.gz` & `tmp/EmoTFIDF-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\EmoTFIDF-1.0.9.tar", last modified: Fri Mar  5 10:20:46 2021, max compression
+gzip compressed data, was "EmoTFIDF-1.1.0.tar", last modified: Mon Apr 17 21:01:59 2023, max compression
```

## Comparing `EmoTFIDF-1.0.9.tar` & `EmoTFIDF-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/
-drwxrwxrwx   0        0        0        0 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/
--rw-rw-rw-   0        0        0        1 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3258 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        5 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/requires.txt
--rw-rw-rw-   0        0        0      189 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/EmoTFIDF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5013 2021-03-05 10:18:45.000000 EmoTFIDF-1.0.9/emotfidf.py
--rw-rw-rw-   0        0        0     3258 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1996 2021-03-05 10:15:05.000000 EmoTFIDF-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2021-03-05 10:20:46.000000 EmoTFIDF-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1363 2021-03-05 10:20:33.000000 EmoTFIDF-1.0.9/setup.py
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-17 21:01:59.100029 EmoTFIDF-1.1.0/
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-17 21:01:59.099578 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2353 2023-04-17 21:01:59.000000 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)      197 2023-04-17 21:01:59.000000 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        1 2023-04-17 21:01:59.000000 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        5 2023-04-17 21:01:59.000000 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/requires.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        9 2023-04-17 21:01:59.000000 EmoTFIDF-1.1.0/EmoTFIDF.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1091 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.0/LICENSE
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2353 2023-04-17 21:01:59.099823 EmoTFIDF-1.1.0/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1843 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.0/README.md
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     4764 2023-04-17 17:02:30.000000 EmoTFIDF-1.1.0/emotfidf.py
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)       38 2023-04-17 21:01:59.100084 EmoTFIDF-1.1.0/setup.cfg
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1386 2023-04-17 21:01:51.000000 EmoTFIDF-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `EmoTFIDF-1.0.9/emotfidf.py` & `EmoTFIDF-1.1.0/emotfidf.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,24 +30,26 @@
     # get emotions
     em_list = []
     em_dict = dict()
     em_frequencies = Counter()
     lexicon_keys = self.lexicon.keys()
     for word in self.words:
         if word in lexicon_keys:
-            em_list.extend(self.lexicon[word])
-            em_dict.update({word: self.lexicon[word]})
+            emotions_found = self.lexicon[word]
+            if emotions_found is not None:
+                if 'negative' in emotions_found:
+                    emotions_found.remove('negative')
+                elif 'positive' in emotions_found:
+                    emotions_found.remove('positive')
+                em_list.extend(emotions_found)
+                em_dict.update({word: self.lexicon[word]})
     for word in em_list:
         em_frequencies[word] += 1
     sum_values = sum(em_frequencies.values())
-    em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0, 'positive': 0.0,
-                  'negative': 0.0, 'sadness': 0.0, 'disgust': 0.0, 'joy': 0.0}
-    if self.sent_flag == 1:
-        em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0, 'sadness': 0.0,
-                      'disgust': 0.0, 'joy': 0.0}
+    em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0,'sadness': 0.0, 'disgust': 0.0, 'joy': 0.0}
     for key in em_frequencies.keys():
         em_percent.update({key: float(em_frequencies[key]) / float(sum_values)})
     self.em_list = em_list
     self.em_dict = em_dict
     self.emotion_scores = dict(em_frequencies)
     self.em_frequencies = em_percent
 
@@ -58,35 +60,32 @@
     with urllib.request.urlopen("https://raw.githubusercontent.com/mmsa/EmoTFIDF/main/emotions_lex.json") as url:
         lexicon = json.loads(url.read().decode())
 
     def set_text(self, text):
         self.text = process_message(text)
         self.words = list(nltk.word_tokenize(self.text))
         self.sentences = list(nltk.sent_tokenize(self.text))
-        self.sent_flag = 0
         get_emotions(self)
 
     def set_lexicon_path(self, path):
         self.path = path
         if path != ' ' and path != 0:
             with open(path) as jsonfile:
                 self.lexicon = json.load(jsonfile)
         else:
             with urllib.request.urlopen(
                     "https://raw.githubusercontent.com/mmsa/EmoTFIDF/main/emotions_lex.json") as url:
                 self.lexicon = json.loads(url.read().decode())
 
-    def remove_sentiments(self, sent_flag):
-        self.sent_flag = sent_flag
-
     def computeTFIDF(self, docs):
-        vectorizer = TfidfVectorizer(max_features=200, stop_words=stopwords.words('english'),
+        stop_words = stopwords.words('english')
+        vectorizer = TfidfVectorizer(max_features=200, stop_words=stop_words,
                                      token_pattern=r'(?u)\b[A-Za-z]+\b')
         vectors = vectorizer.fit_transform(docs)
-        feature_names = vectorizer.get_feature_names()
+        feature_names = vectorizer.get_feature_names_out()
         dense = vectors.todense()
         denselist = dense.tolist()
         df = pd.DataFrame(denselist, columns=feature_names)
         self.tfid = df
         self.vectorizer = vectorizer
         self.feature_names = feature_names
 
@@ -94,25 +93,22 @@
         tfidf_matrix = self.vectorizer.transform([self.text]).todense()
         feature_index = tfidf_matrix[0, :].nonzero()[1]
         tfidf_scores = zip([self.feature_names[i] for i in feature_index], [tfidf_matrix[0, x] for x in feature_index])
         self.ifidf_for_words = dict(tfidf_scores)
 
     def get_emotfidf(self):
         self.get_ifidf_for_words()
-        em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0, 'positive': 0.0,
-                      'negative': 0.0, 'sadness': 0.0, 'disgust': 0.0, 'joy': 0.0}
-        if self.sent_flag == 1:
-            em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0, 'sadness': 0.0,
-                          'disgust': 0.0, 'joy': 0.0}
+        em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0,'sadness': 0.0, 'disgust': 0.0, 'joy': 0.0}
         em_frequencies = Counter()
         for word in self.em_list:
             em_frequencies[word] += 1
         for e in self.em_dict.keys():
             if e in self.ifidf_for_words:
                 tfidf_weight = self.ifidf_for_words[e]
                 for a in self.em_dict[e]:
                     new_fre = round(em_frequencies[a] / tfidf_weight, 2)
                     em_frequencies[a] = new_fre
         sum_values = sum(em_frequencies.values())
         for key in em_frequencies.keys():
             em_percent.update({key: round(float(em_frequencies[key]) / float(sum_values), 3)})
         self.em_tfidf = em_percent
+        self.em_tfidf = em_percent
```

### Comparing `EmoTFIDF-1.0.9/README.md` & `EmoTFIDF-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -66,15 +66,8 @@
 Thanks to [artofchores](https://www.reddit.com/user/artofchores/), from Reddit for his feedback.
 
 
 Added a set_lexicon_path option if you would like to use your own lexicon
 Remember to keep the same structure as the original emotions lexicon which located [here](https://raw.githubusercontent.com/mmsa/EmoTFIDF/main/emotions_lex.json)
 ```
 emTFIDF.set_lexicon_path("other_lexicon.json")
-```
-
-##Update 1.0.8
-
-Allow users to remove the two sentiments (Positive and Negative) from the output emotions
-```
-emTFIDF.remove_sentiments(1)
-```
+```
```

### Comparing `EmoTFIDF-1.0.9/setup.py` & `EmoTFIDF-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         nltk.download('wordnet')
         nltk.download('punkt')
         nltk.download('stopwords')
 
 
 setuptools.setup(
     name="EmoTFIDF",
-    version="1.0.9",
+    version="1.1.0",
     author="mmsa12",
     author_email="mmsa12@gmail.com",
     description="A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion"
                 "2- Integrating TFIDF to add a context"
                 "Note that lexicon license is for research purposes only.",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -39,8 +39,9 @@
     package_data={'project': ['emotions_lex.json']},
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=2.7',
+    sklearn='>=1.0.x'
 )
```

