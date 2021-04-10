Transformer models can perform almost any NLP task. Here, I have implemented HuggingFace [RoBERTa](https://huggingface.co/transformers/model_doc/roberta.html) transformer to predict the product categories.

* I used RoBERTa tokenizer to tokenize the product description, and used torchtext.data to create a data pre-processing pipeline and divide the pre-processed data into train, test and validation sets.

* I used pre-trained RobertaForSequence classification to implement the modelling task, and then trained it on the pre-processed data. I trained the model for 5 epochs whicch took around 1 hour 30 mintues and the validation loss decreased from 1.6168 to 0.1824.

* When I tested the model on the test set, I obtained the accuracy of 0.9642, which is very good. But we can also see that this accuracy is comparable to that of simple ML models and it took a lot of time and computation power as compared to them. So, we can conclude that even after achieveing the good results, we have better options than transformers to implement our task in the production environment.

**References**
* https://towardsdatascience.com/multi-class-text-classification-with-deep-learning-using-bert-b59ca2f5c613
* https://huggingface.co/transformers/model_doc/roberta.html
* https://huggingface.co/transformers/preprocessing.html
* https://blog.usejournal.com/why-and-how-to-make-a-requirements-txt-f329c685181e
* https://www.analyticsvidhya.com/blog/2019/04/predicting-movie-genres-nlp-multi-label-classification/ (Used for data visualization)
