**Using LSTMs to predict the product category.**
* I used the clean version of the dataset that can be found [here](https://drive.google.com/file/d/1uM5Kr_CieByJkZiSxVeKPhSpWV-aUYTY/view?usp=sharing)
* To encode each description I created a vocabulary and used dictionaries that map the words in the vocabulary to integers.
* I padded the tokenized description with zeros upto the sequence length, and truncated the ones that exceed sequence length. I used a sequence length of 200.
* I used a single-layer LSTM model with embedding dimension of 50 and 128 hidden layers. I initialized the hidden state to zero.
* To train the model I used Adam optimizer with learning rate of 0.001. After 10 epochs, the model managed to decrease the validation loss from 1.200722 to 0.291314.
* The overall test loss was 0.243 and the accuracy was 0.923, which is pretty good.
* The performance can be improved further by hyperparameter tuning and using more data.

**References**
* https://towardsdatascience.com/multiclass-text-classification-using-lstm-in-pytorch-eac56baed8df
* https://github.com/AyushiNM/sentiment-analysis/blob/master/Sentiment_Analysis_RNN.ipynb
