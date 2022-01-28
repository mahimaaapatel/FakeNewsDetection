# FakeNewsDetection

Fake news which can be broadly defined as false or misleading information is asserted to have serious consequences on society. This can lead to instabilities in the country of varying magnitude, ranging from fear mongering to massive protests with serious economic and social consequences.

Our team has come up with a real time fake news detection system that uses pyspark for data processing and a machine learning algorithm  to predict whether the news is likely to be fake or real.

Pyspark is used for the pre-processing of data. Generally, Pyspark is used to handle large amounts of data that usually cannot be handled by a single system. It is also used to manipulate a given dataset and process it. In our project, we use Pyspark to remove the columns that are not required by our model. We also use it to combine the two datasets- True.csv and False.csv into one dataset. Once the datasets are combined into one, we add a 'label' column that denotes whether the particular record is fake or true.

After this comes the data cleaning process. This involves removing the unwanted words from the text such as the articles and punctuation, and leaving only the important words. Non-letters and punctuation are removed and then the stopwords are removed. Stopwords are the most common words in any natural language, for example, 'the', 'where', and 'and'.

Once the data is cleaned, the next step is to create the model and train it. In this particular project, we split the dataset as 80% training and 20% testing. We use a logistic regression model and the Naive Bayes model for training the model. Logistic Regression makes a prediction for the probability using a direct formula whereas Naive Bayes figures out how the data was generated given the results.

In the end, to visualize the results, we are printing the accuracy of the model and plotting a graph of the confusion matrix, which gives us the percentage of valid and invalid results predicted.
