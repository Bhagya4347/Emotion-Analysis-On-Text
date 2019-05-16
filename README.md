# Emotion-Analysis-On-Text

### Objective: ###

Aim is to make machines understand and detect emotions from any textual input. A text based emotion recognition system which give an overall sentiment of the sentence/paragraph in terms of positivity/negativity and neutrality and determine the overall emotion.

### Work Done: ###

- Analyse the impact of effective words on the sentence.
- Used supervied learning models to classify the emotion classes on given sentence.
- Further work includes Emotional analysis on a given sentence/paragraph and find the relation using VAD. 

### Dependencies: ###

- Numpy
- Pandas
- NLTK
- sklearn
- Python3
- re

### Installation: ###

Use pip3 to install any missing dependencies. Such as For Naive Bayes install textblob.

$ pip install -U textblob

$ python -m textblob.download_corpora

### DataSet: ###

Twitter dataset is used which contains 40000 tweets containing basic emotion categories. 

### Papers followed: ###

EMOTION DETECTION FROM TEXT by Shiv Naresh Shivhare and Prof. Saritha Khethawat
(https://airccj.org/CSCP/vol2/csit2237.pdf)

Retracted: Recognition of Emotion with SVMs  by Zhi Teng, Fuji Ren and Shingo Kuroiwa
(https://link.springer.com/chapter/10.1007/978-3-540-37275-2_87)

### Overview: ###

Approach followed is:

1. Raw data set: It contains 40,000 tweets and 4 columns.

2. Data Pre-processing: 

 Pre - processing includes:
 - Removal of regular expressions, symbols using the 're' library
 - Removal of lemmas (Lexicon Normalization) using WordNetLemmatizer from NLTK
 - Removal of multi-letter ambiguities, e.g 'noooo' gets converted to 'no'
 - Removal of stop-words - caused decrease in f1-score as well as overall accuracy
 
3. Word Dictionary:
Words are stored in a dictionary. 

4. Word2Vec:
Vectorization is done. Words are vectorized each vector represnts the category of emotion. 

5. Training Model: 

SVM and Naive Bayes is used to train the model. 

6. Result(Accuracy):

Comparing two different algorithms of classifying the emotions and then the accuracies of those two algorithms(SVM and Naive Bayes). SVM gives slightly better accuracy on this twitter dataset than to Naive Bayes. 

### Accuracy: ###

SVM(On 10000 tweets): 33%

Naive Bayes(On 10000 tweets): 31%




