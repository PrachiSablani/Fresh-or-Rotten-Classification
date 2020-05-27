# Fresh-or-Rotten-Classification
Supervised Machine Learning | Text Classification | Python | Naive Bayes

The objective of this project is to implement Naive Bayes Classifier from scratch to categorize Rotten Tomatoes reviews into rotten and fresh ones and to find the optimal smoothing parameter.

The data had around 13000 reviews with some features like – Movie title, critic name, review, where it was published, link, review date.

I started with exploratory data analysis where I checked data types, missing values(23 none, less than 1% of data), numerical features, categorical features, checked the percentage of fresh and rotten (for checking imbalanced classes), duplicate reviews (236), checked missing reviews(0 length or space)

Then I proceeded with data cleaning, where I removed duplicate reviews and missing values. Then I separated my data into 2 parts – 80% training and 20% test set and converted reviews into bag of words where I extracted all the words from the text and created a vocabulary out of it by creating a vectorizer using Countvectorizer in python.

After that I calculated the prior probabilities for fresh and rotten reviews. Then I implemented Naïve Bayes classifier from scratch in Python to find the probability of a given review to be classified in fresh as well as rotten and classified into the class which has a higher probability.

To verify the results, I applied cross-validation and after testing it against test data, I got an accuracy of 70%.

Lastly, I applied Laplace smoothing and tested the model with different values of smoothing parameter called alpha and cross-validated the model each time. 
