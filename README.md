# Youtube_comments_classifier

This is a NLP project for classifying youtube comments into 6 classes and they are 'positive', 'negative', 'imperative', 'interrogative', 'miscellaneous' and 'corrective'.

Data Preprocessing involves :-
* changing to lowecase
* removing urls, punctuations and other symbols
* removing stop words
* applying lemmatization

Feature Extraction and modeling :-
1) using bag of words, followed by simpler models gives accuracy:-
   * MultinomialNB:      0.6481
   * RandomForest:       0.6507
   * LinearSVC:          0.6410
   * LogisticRegression: 0.6701
   * DecisionTree:       0.5914

2) using tf-idf, followed by simpler models gives accuracy:-
   * MultinomialNB:      0.6348
   * RandomForest:       0.6747
   * LinearSVC:          0.6757
   * LogisticRegression: 0.6936
   * DecisionTree:       0.5787

3) using word2vec, followed by simpler models gives accuracy:-
   * MultinomialNB:      0.4796
   * RandomForest:       0.6210
   * LinearSVC:          0.6307
   * LogisticRegression: 0.6113
   * DecisionTree:       0.4898

4) using glove, followed by LSTM gives accuracy 0.6281
5) using, following by finetunning BERT gives accuracy 0.6598

The above ipynb file contains code of mentioned steps.
