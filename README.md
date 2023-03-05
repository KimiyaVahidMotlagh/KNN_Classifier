# Handwritten-KNN
Simple KNN algoritm Python code :)<br />
KNN is a supervised algoritm which determins a data's label, based on the k nearest training examples in the dataset. This algorithm determin the data is more likely to be in a class by the training data most similar to our test data.

## Table of Contents
- [KNN functions](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#knn-functions)  <br />
- [Loading data](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#loading-data) <br />
- [Hyperparameter tuning(K)](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#hyperpatameter-tuningk) <br />
- [KNN excution and accuracy](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#knn) <br />

## KNN functions
- **distanse calculator** <br />
Often Mechin learning data is defined by vectors. KNN algorithm searchs for the similar training data. The most srightforward function to find the neighbors is the 2D distance function.<br />
- **KNN classifier** <br />
By knowing the distance between two points, K nearest neighbors are the training points with least distance. This function would find the most labels in the neighbors and classify the test data point as the same label.
- **Accuracy calculator** <br />
Because KNN is a supervised algorithm, we actually have the test labels. The number of rightly classifide labels devided by total number of data.
- **KNN plot function** <br />

## Loading data
- Read csv file <br />
- split train and test data <br />

## Hyperpatameter tuning(K)
<br />

## KNN
execution <br />
With K=13, the only thing left is calling the function. 
accuracy <br />
accuracy calculator function checks the percentage of correct label predictions. This function has been used in hyperparameter tuning for our elbow data.
