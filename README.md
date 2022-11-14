# Naive Bayes Classiication
Naive Bayes Classifier
What is Naive Bayes algorithm?
It is a classification method built on the Bayes Theorem and predicated on the idea of predictor independence. A
Naive Bayes classifier, to put it simply, believes that the presence of one feature in a class has nothing to do
with the presence of any other feature.
A fruit might be categorized as an apple, for instance, if it is red, rounded, and around 3 inches in diameter. Even
if these characteristics depend on one another or on the presence of other characteristics, each of these traits
separately increases the likelihood that this fruit is an apple, which is why it is called "Naive."
Naive Bayes model is easy to build and particularly useful for very large data sets. Along with
simplicity, Naive Bayes is known to outperform even highly sophisticated classification methods.
Bayes theorem provides a way of calculating posterior probability P(c|x) - (read as Probability of c given x), from
P(c), P(x) and P(x|c). Look at the equation below: >

how to run the jupyter notebook file

1. use google colab

2. download the dataset from kaggle

3. upload the .pynb file and the dataset

4. run the code


Below is the process used for coding.
Merge the dataset into one. And divide the dataset as train, development and test. 

Build a vocabulary as list. 
[‘the’ ‘I’ ‘happy’ … ] 
You may omit rare words for example if the occurrence is less than five times
A reverse index as the key value might be handy
{“the”: 0, “I”:1, “happy”:2 , … }
Calculate the following probability
Probability of the occurrence
P[“the”] = num of documents containing ‘the’ / num of all documents
Conditional probability based on the sentiment
P[“the” | Positive]  = # of positive documents containing “the” / num of all positive review documents
Calculate accuracy using dev dataset  
Do following experiments
Compare the effect of Smoothing
Derive Top 10 words that predicts each class
P[class | word] 
Using the test dataset
Use the optimal hyperparameters you found in the step e, and use it to calculate the final accuracy. 
