Here, I tried various Machine Learning models on the data to predict the product category.
* Initially, I observed that the product description had a lot of stop words which were adding noise to the data, so I removed them.
* Then, I divided the data into train and test sets and used Tfidf Vectorizer to vectorize the data.
* I used ML models on the data,
    1) Multinomial Naive Bayes -> accuracy - 0.84
    2) RandomForest -> accuracy - 0.93
    3) XGBoost -> accuracy - 0.96
    4) SGDClassifier -> 0.98

* The SGD classifier performed best on the data, and the other models (except NaiveBayes) gave good results as well. 

**References**
* https://towardsdatascience.com/machine-learning-nlp-text-classification-using-scikit-learn-python-and-nltk-c52b92a7c73a
* https://www.analyticsvidhya.com/blog/2019/04/predicting-movie-genres-nlp-multi-label-classification/
* https://www.analyticsvidhya.com/blog/2020/02/quick-introduction-bag-of-words-bow-tf-idf/
* https://towardsdatascience.com/methods-for-dealing-with-imbalanced-data-5b761be45a18
* https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html
* https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
* https://machinelearningmastery.com/develop-first-xgboost-model-python-scikit-learn/
* https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.SGDClassifier.html
* https://blog.usejournal.com/why-and-how-to-make-a-requirements-txt-f329c685181e
* https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html
