# Algorithms for Massive Data - Exam Project

## Amazon US Costumer Review Link Analysis

The aim of this project is to create a ranking system that could be used
in order to establish a sequence in which the reviews of Amazon products should be shown. 
The idea is to calculate the PageRank score of each customer based on the reviews he/she did of an item in common with
other customers. This is because it’s difficult that spammers (that want to inflate the rating of
their products) have reviews in common with others of many different products. \
However, in this way it
would be given more importance to customers that left many, but meaningless reviews compared
to those who left fewer, but more effective reviews. In fact, the PageRank score doesn’t give any information of the usefulness of the reviews left by users. However, on Amazon it is possible for users
to rate a review as ”useful”. This data is captured by the variable "helpful_votes" in the dataset. 
So, in addition to the PageRank score I evaluated the ”helpfulness score” and add it to PageRank, to create a new ordering. \
The data used for the project is a subset of the Amazon US Costumer Review dataset, that contains more than 100 million of rows. Due to the the size of the data Spark is used in order to parallelize the computation and to make the model scalable also for bigger datasets. 

