Here, I have cleaned and pre-processed the initially provided data, and created a new dataset that can be found [here](https://drive.google.com/file/d/1uM5Kr_CieByJkZiSxVeKPhSpWV-aUYTY/view?usp=sharing).

* To decide the primary category for each data point, I first separated categories in the product_category_tree. Then, I observed that the minimum number of categories for a product in the given dataset is 1, which is the root category, I concluded that the root category is the primary category.

* The dataset was very imbalanced and many classes did not have sufficient data as compared to their counter parts, so I removed these categories as they were just adding noise to the data. The resultant data has 18 categories.

* To clean the product description, I

    (1) converted all the data into lower case

    (2) replaced contractions

    (3) removed all the special characters and extra space

* Then, I shuffled the data and stored the cleaned values and primary category in a new dataset.

References -
* https://www.geeksforgeeks.org/pandas-how-to-shuffle-a-dataframe-rows/
* https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.reset_index.html
* https://blog.usejournal.com/why-and-how-to-make-a-requirements-txt-f329c685181e
* https://www.analyticsvidhya.com/blog/2019/04/predicting-movie-genres-nlp-multi-label-classification/
