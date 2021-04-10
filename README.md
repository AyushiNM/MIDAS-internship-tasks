# MIDAS-internship-tasks

**Data Pre-processing ->** https://github.com/AyushiNM/MIDAS-internship-tasks/tree/main/Data%20Pre-processing

**Machine Learning Models ->** https://github.com/AyushiNM/MIDAS-internship-tasks/tree/main/ML%20Models

**LSTM ->** https://github.com/AyushiNM/MIDAS-internship-tasks/tree/main/LSTM

**Transformers ->** https://github.com/AyushiNM/MIDAS-internship-tasks/tree/main/Transformers%20-%20RoBERTa



**Summary of all the models that I have tried on the data.**

| Method  | Accuracy |
| ------------- | ------------- |
| NaiveBayes | 0.84 |
| RandomForest | 0.93 |
| XGBoost | 0.96 |
| SGDClassifier | 0.98 |
| LSTM | 0.923 |
| RoBERTa | 0.9642 |

* To measure the performance for each class, I have used weighted precison, recall and f1 score (which can be found in classification reports in each notebook), and to measure overall performance I have used accuracy.
* It can be observed that SGDClassifier gave the best accuracy. 
* XGBoost and RoBERTa come second. However, because of the complexity and training time of transformer models, RoBERTa would not be a very good choice for this task, especially when we're getting comparable results with simpler models. 
* To improve the performance of the models we could try hyperparameter tuning and using more data. We could also try to use other features along with product description, like product name, which could also be a good indicator of product category.
