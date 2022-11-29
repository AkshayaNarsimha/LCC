# LCC
CONTENTS OF THIS FILE

---------------------

* Description
* Requirements
* Installation


DESCRIPTION
-----------
This is a concept learner implemented in Python by Ludwig Wideskär and Akshaya Narsimha.
The aim of the assignment is to implement a concept learner and to verify that it works as expected using the features 
and instances given in the spambase dataset. The document discusses the implementation of the concept 
learner and the results obtained from it.



REQUIREMENTS
------------

The following requirements is needed for the program to run:

* Spambase dataset must be uploaded within the same folder
* Python intrepreter

The following Python modules needs to be installed on the system:
* numpy
* matplotlib
* pandas
* sklearn


WORKING
------------

instructions here:
DATA PREPROCESSING: For the data preprocessing of our spambase.csv data, we read the file with the help of the pandas 
and the descretization technique is used for the preprocessing with 5 bins(more like 0,1,2,3,4 intervals in the data).
The last 3 columns data is avoided as there are high value which is highly irrelevant to the data. after the decretization
the values are transformed with respective to the number of bins. 
INSTANCES: The number of instances in our dataset is number of unique values occurences in the whole dataset. There are 
14427791579676672 instances. 
HYPOTHESIS SPACE: As there are 5features in our dataset as bins are 5 and 14427791579676672 instances, the size of
Hypothesis space will be 5**14427791579676672.
With the possible instances and hypothesis space taken in to the consideration, we implemented the Least general 
generalisation algorithms. 
Algorithm 4.1:
Algorithm 4.2:

TESTING 
------------
The preprocessed data is split with the ratio of 0.8 as test data and train data. In the test data we acquire 80% of data
and in the train data we acquire remaining 20% of data. The test data should always be greater than or equal to the train
data.


ACCURACY
------------
Here train data is our hypothesis data. so by predict and true values whereas here pred value is LGG(test data) and true 
value is LGG(train data). we check if the true values and the predicted values are same. according to the percentage of 
the similarity the accuracy of the data is determined. 
In the data i split the pos values as pos_res and neg as neg_res. By running the data with respective to algorithms with
the pos_res the accuracy obtained is 0.9818181818181818.
By running the data with respective to algorithms with the neg_res the accuracy obtained is 1.0
If the whole data is considered then the accuracy is obtained as 1.0
