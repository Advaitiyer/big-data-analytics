## Spam Detector: Regularized Natural Language Processing

Implementation of an SMS spam detector based on logistic regression. This is the same idea behind sentiment analysis, but instead of predicting positive sentiment vs negative sentiment, you are going to predict whether a SMS text is spam or not.

The initial dataset looked as follows:

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk3-step1.png?raw=true"/>

**Labeling**

Encoded the type column to be 1 for spam and 0 for ham and store the result in sms_spam2_df. After the processing, the label column was converted to binary.

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk3-step2.png?raw=true"/>

**TF-IDF and Feature Engineering**

Created a pipeline that combines a Tokenizer, CounterVectorizer, and an IDF estimator to compute the tfidf vectors of each SMS. This pipeline was fitted and assigned a variable tfidf_pipeline. The Tokenizer step created a column for words, the CounterVectorizer step created a column tf, and the IDF step created a column tfidf.

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/wk3-step3.png?raw=true"/>

**Results after model implementation**

Logistic regression using PySpark was implemented with various settings of regularization parameter (<img src="https://latex.codecogs.com/gif.latex?\lambda"/>) and elastic net mixture (<img src="https://latex.codecogs.com/gif.latex?\alpha"/>)

Positive words:

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/positive-words.png?raw=true"/>

Negative words: 

<img src="https://github.com/Advaitiyer/advaitiyer.github.io/blob/master/assets/images/big-data-analytics/negative-words.png?raw=true"/>
